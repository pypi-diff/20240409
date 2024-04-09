# Comparing `tmp/cognite_neat-0.70.0.tar.gz` & `tmp/cognite_neat-0.70.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.70.0.tar", max compression
+gzip compressed data, was "cognite_neat-0.70.1.tar", max compression
```

## Comparing `cognite_neat-0.70.0.tar` & `cognite_neat-0.70.1.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    11351 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/LICENSE
--rw-r--r--   0        0        0     6775 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/README.md
--rw-r--r--   0        0        0       61 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1893 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     1805 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/core.py
--rw-r--r--   0        0        0     4646 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     6369 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    11564 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0    15406 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      629 2024-04-09 12:46:37.251779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0   344557 2024-04-09 12:46:37.255780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-04-09 12:46:37.255780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-04-09 12:46:37.255780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-04-09 12:46:37.255780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13345 2024-04-09 12:46:37.255780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1403536 2024-04-09 12:46:37.259780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js
--rw-r--r--   0        0        0     2667 2024-04-09 12:46:37.259780 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt
--rw-r--r--   0        0        0  6235494 2024-04-09 12:46:37.283779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map
--rw-r--r--   0        0        0   240334 2024-04-09 12:46:37.303779 cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
--rw-r--r--   0        0        0     1503 2024-04-09 12:46:37.307779 cognite_neat-0.70.0/cognite/neat/config.py
--rw-r--r--   0        0        0     1228 2024-04-09 12:46:37.307779 cognite_neat-0.70.0/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-04-09 12:46:37.307779 cognite_neat-0.70.0/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-04-09 12:46:37.307779 cognite_neat-0.70.0/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-04-09 12:46:37.311779 cognite_neat-0.70.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11232 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17408 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14969 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-04-09 12:46:37.315779 cognite_neat-0.70.0/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5377 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/_analysis/__init__.py
--rw-r--r--   0        0        0      674 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/_analysis/_base.py
--rw-r--r--   0        0        0    19613 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/_analysis/_information_rules.py
--rw-r--r--   0        0        0      177 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5501 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123868 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    37099 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8220 2024-04-09 12:46:37.319779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0     9688 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     9080 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19768 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     3038 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7890 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4268 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0     9138 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7674 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7304 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     5442 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0    10573 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     5856 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    11167 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     7493 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     4964 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1299 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    17145 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0    10295 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     6079 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    10635 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    49323 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    30010 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     2051 2024-04-09 12:46:37.323779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    20732 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7344 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4316 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0    11063 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3844 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2699 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26223 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    15674 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6528 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6040 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18272 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12274 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-04-09 12:46:37.327779 cognite_neat-0.70.0/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-04-09 12:46:37.331779 cognite_neat-0.70.0/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4543 2024-04-09 12:46:37.715777 cognite_neat-0.70.0/pyproject.toml
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.70.0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/README.md
+-rw-r--r--   0        0        0       61 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1893 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     1805 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/core.py
+-rw-r--r--   0        0        0     4646 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13653 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     6369 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    11564 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0    15406 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      629 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0   344557 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13345 2024-04-09 14:52:18.477890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1403536 2024-04-09 14:52:18.485890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js
+-rw-r--r--   0        0        0     2667 2024-04-09 14:52:18.485890 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt
+-rw-r--r--   0        0        0  6235494 2024-04-09 14:52:18.509889 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map
+-rw-r--r--   0        0        0   240334 2024-04-09 14:52:18.529889 cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg
+-rw-r--r--   0        0        0     1503 2024-04-09 14:52:18.533889 cognite_neat-0.70.1/cognite/neat/config.py
+-rw-r--r--   0        0        0     1228 2024-04-09 14:52:18.533889 cognite_neat-0.70.1/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-09 14:52:18.533889 cognite_neat-0.70.1/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-09 14:52:18.533889 cognite_neat-0.70.1/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-09 14:52:18.537889 cognite_neat-0.70.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractor/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractor/_base.py
+-rw-r--r--   0        0        0    11232 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractor/_dexpi.py
+-rw-r--r--   0        0        0    17408 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractor/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14872 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractor/_mock_graph_generator.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14969 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      693 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/__init__.py
+-rw-r--r--   0        0        0    23838 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/_asset_loader.py
+-rw-r--r--   0        0        0     2370 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/core/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/core/labels.py
+-rw-r--r--   0        0        0     5016 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/core/models.py
+-rw-r--r--   0        0        0    40458 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22678 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12957 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/loader/validator.py
+-rw-r--r--   0        0        0      149 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14254 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5377 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-09 14:52:18.541890 cognite_neat-0.70.1/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/graph/transformation/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/graph/transformation/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/graph/transformation/query_generator/__init__.py
+-rw-r--r--   0        0        0    18659 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/graph/transformation/query_generator/sparql.py
+-rw-r--r--   0        0        0    14673 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/graph/transformation/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/_analysis/__init__.py
+-rw-r--r--   0        0        0      674 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/_analysis/_base.py
+-rw-r--r--   0        0        0    19613 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/_analysis/_information_rules.py
+-rw-r--r--   0        0        0      177 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0     8596 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5501 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_base.py
+-rw-r--r--   0        0        0      102 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_core/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_core/rules2labels.py
+-rw-r--r--   0        0        0    37099 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2dms.py
+-rw-r--r--   0        0        0     8220 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2excel.py
+-rw-r--r--   0        0        0     6215 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2graphql.py
+-rw-r--r--   0        0        0    18414 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2ontology.py
+-rw-r--r--   0        0        0    28745 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3866 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2rules.py
+-rw-r--r--   0        0        0     1104 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2triples.py
+-rw-r--r--   0        0        0     5769 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporter/_validation.py
+-rw-r--r--   0        0        0      413 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1518 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0    12129 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     9080 2024-04-09 14:52:18.545889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19768 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     3038 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4092 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_base.py
+-rw-r--r--   0        0        0     6469 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_dict2rules.py
+-rw-r--r--   0        0        0     7890 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_dms2rules.py
+-rw-r--r--   0        0        0    12097 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9320 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10521 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1529 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      448 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_xsd2rules.py
+-rw-r--r--   0        0        0     1628 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importer/_yaml2rules.py
+-rw-r--r--   0        0        0      408 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4268 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0     9138 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12554 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6925 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11926 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7674 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7304 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     5442 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    10573 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4198 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     5856 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    11167 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     7493 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      127 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0      517 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/__init__.py
+-rw-r--r--   0        0        0     1299 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/__init__.py
+-rw-r--r--   0        0        0    17145 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/_base.py
+-rw-r--r--   0        0        0    10295 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/_field.py
+-rw-r--r--   0        0        0     6079 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/_value.py
+-rw-r--r--   0        0        0    10635 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/base.py
+-rw-r--r--   0        0        0    49379 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/dms_architect_rules.py
+-rw-r--r--   0        0        0    30229 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/dms_schema.py
+-rw-r--r--   0        0        0     2051 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/domain_rules.py
+-rw-r--r--   0        0        0    20984 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/_rules/information_rules.py
+-rw-r--r--   0        0        0    12368 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7344 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51063 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/tables.py
+-rw-r--r--   0        0        0     4316 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/rules/models/value_types.py
+-rw-r--r--   0        0        0       68 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-09 14:52:18.549889 cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0    11063 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2699 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26223 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Export DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Import DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
+-rw-r--r--   0        0        0    15674 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6528 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6040 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18272 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7327 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4785 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29390 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27269 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12274 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2345 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20657 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28072 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-09 14:52:18.553889 cognite_neat-0.70.1/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4543 2024-04-09 14:52:18.941889 cognite_neat-0.70.1/pyproject.toml
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.70.1/PKG-INFO
```

### Comparing `cognite_neat-0.70.0/LICENSE` & `cognite_neat-0.70.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/README.md` & `cognite_neat-0.70.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/configuration.py` & `cognite_neat-0.70.1/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.70.1/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.70.1/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/explorer.py` & `cognite_neat-0.70.1/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.70.1/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/routers/core.py` & `cognite_neat-0.70.1/cognite/neat/app/api/routers/core.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.70.1/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.70.1/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.70.1/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.70.1/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.70.1/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.70.1/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.70.1/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.70.1/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg` & `cognite_neat-0.70.1/cognite/neat/app/ui/neat-app/build/static/media/logo.8093b84df9ed36a174c629d6fe0b730d.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/config.py` & `cognite_neat-0.70.1/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/constants.py` & `cognite_neat-0.70.1/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/exceptions.py` & `cognite_neat-0.70.1/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.70.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.70.1/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.70.1/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/exceptions.py` & `cognite_neat-0.70.1/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.70.1/cognite/neat/graph/extractor/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.70.1/cognite/neat/graph/extractor/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.70.1/cognite/neat/graph/extractor/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.70.1/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.70.1/cognite/neat/graph/loader/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.70.1/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.70.1/cognite/neat/graph/transformation/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.70.1/cognite/neat/graph/transformation/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.70.1/cognite/neat/graph/transformation/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/_analysis/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/_analysis/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/_analysis/_information_rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/_analysis/_information_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/analysis.py` & `cognite_neat-0.70.1/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.70.1/cognite/neat/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.70.1/cognite/neat/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.70.1/cognite/neat/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.70.1/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.70.1/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exceptions.py` & `cognite_neat-0.70.1/cognite/neat/rules/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporter/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import warnings
 from collections.abc import Collection, Iterable
 from pathlib import Path
-from typing import Literal, TypeAlias
+from typing import Literal, TypeAlias, cast
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes._base import CogniteResourceList
 from cognite.client.exceptions import CogniteAPIError
 
 from cognite.neat.rules._shared import Rules
 from cognite.neat.rules.models._rules import InformationRules
-from cognite.neat.rules.models._rules.dms_architect_rules import DMSRules
+from cognite.neat.rules.models._rules.base import ExtensionCategory, SheetList
+from cognite.neat.rules.models._rules.dms_architect_rules import DMSContainer, DMSRules
 from cognite.neat.rules.models._rules.dms_schema import DMSSchema, PipelineSchema
 from cognite.neat.utils.cdf_loaders import (
     ContainerLoader,
     DataModelingLoader,
     DataModelLoader,
     RawDatabaseLoader,
     RawTableLoader,
@@ -103,22 +104,61 @@
             exclude = set()
         else:
             exclude = {"spaces", "data_models", "views", "containers"} - self.export_components
         return exclude
 
     def export(self, rules: Rules) -> DMSSchema:
         if isinstance(rules, DMSRules):
-            return rules.as_schema(self.standardize_casing, self.export_pipeline, self.instance_space)
+            dms_rules = rules
         elif isinstance(rules, InformationRules):
-            return rules.as_dms_architect_rules().as_schema(
-                self.standardize_casing, self.export_pipeline, self.instance_space
-            )
+            dms_rules = rules.as_dms_architect_rules()
         else:
             raise ValueError(f"{type(rules).__name__} cannot be exported to DMS")
 
+        is_solution_model = (
+            dms_rules.reference and dms_rules.metadata.external_id != dms_rules.reference.metadata.external_id
+        )
+        is_new_model = dms_rules.reference is None
+        if is_new_model or is_solution_model:
+            return dms_rules.as_schema(self.standardize_casing, self.export_pipeline, self.instance_space)
+
+        # This is an extension of an existing model.
+        reference_rules = cast(DMSRules, dms_rules.reference).copy(deep=True)
+        reference_schema = reference_rules.as_schema(self.standardize_casing, self.export_pipeline)
+
+        # Todo Move this to an appropriate location
+        # Merging Reference with User Rules
+        combined_rules = dms_rules.copy(deep=True)
+        existing_containers = {container.class_ for container in combined_rules.containers or []}
+        if combined_rules.containers is None:
+            combined_rules.containers = SheetList[DMSContainer](data=[])
+        for container in reference_rules.containers or []:
+            if container.class_ not in existing_containers:
+                container.reference = None
+                combined_rules.containers.append(container)
+        existing_views = {view.class_ for view in combined_rules.views}
+        for view in reference_rules.views:
+            if view.class_ not in existing_views:
+                view.reference = None
+                combined_rules.views.append(view)
+        existing_properties = {(property_.class_, property_.property_) for property_ in combined_rules.properties}
+        for property_ in reference_rules.properties:
+            if (property_.class_, property_.property_) not in existing_properties:
+                property_.reference = None
+                combined_rules.properties.append(property_)
+
+        schema = combined_rules.as_schema(self.standardize_casing, self.export_pipeline, self.instance_space)
+
+        if dms_rules.metadata.extension in (ExtensionCategory.addition, ExtensionCategory.reshape):
+            # We do not freeze views as they might be changed, even for addition,
+            # in case, for example, new properties are added. The validation will catch this.
+            schema.frozen_ids.update(set(reference_schema.containers.as_ids()))
+            schema.frozen_ids.update(set(reference_schema.node_types.as_ids()))
+        return schema
+
     def export_to_cdf(self, rules: Rules, client: CogniteClient, dry_run: bool = False) -> Iterable[UploadResult]:
         schema = self.export(rules)
         to_export: list[tuple[CogniteResourceList, ResourceLoader]] = []
         if self.export_components.intersection({"all", "spaces"}):
             to_export.append((schema.spaces, SpaceLoader(client)))
         if self.export_components.intersection({"all", "containers"}):
             to_export.append((schema.containers, ContainerLoader(client)))
@@ -132,15 +172,17 @@
             to_export.append((schema.transformations, TransformationLoader(client)))
 
         # The conversion from DMS to GraphQL does not seem to be triggered even if the views
         # are changed. This is a workaround to force the conversion.
         redeploy_data_model = False
 
         for items, loader in to_export:
-            item_ids = loader.get_ids(items)
+            all_item_ids = loader.get_ids(items)
+            skipped = sum(1 for item_id in all_item_ids if item_id in schema.frozen_ids)
+            item_ids = [item_id for item_id in all_item_ids if item_id not in schema.frozen_ids]
             cdf_items = loader.retrieve(item_ids)
             cdf_item_by_id = {loader.get_id(item): item for item in cdf_items}
             to_create, to_update, unchanged, to_delete = [], [], [], []
             is_redeploying = loader.resource_name == "data_models" and redeploy_data_model
             for item in items:
                 if (
                     isinstance(loader, DataModelingLoader)
@@ -159,15 +201,14 @@
                     unchanged.append(item)
                 else:
                     to_update.append(item)
 
             created = len(to_create)
             failed_created = 0
 
-            skipped = 0
             if self.existing_handling in ["update", "force"]:
                 changed = len(to_update)
                 failed_changed = 0
             elif self.existing_handling == "skip":
                 changed = 0
                 failed_changed = 0
                 skipped += len(to_update)
```

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.70.1/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importer/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/base.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.70.1/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/dms_architect_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
     reference: ReferenceType = Field(alias="Reference", default=None)
     constraint: ContainerListType | None = Field(None, alias="Constraint")
 
     def as_container(self, default_space: str, standardize_casing: bool = True) -> dm.ContainerApply:
         container_id = self.container.as_id(default_space, standardize_casing)
         constraints: dict[str, dm.Constraint] = {}
         for constraint in self.constraint or []:
-            requires = dm.RequiresConstraint(constraint.as_id(default_space))
+            requires = dm.RequiresConstraint(constraint.as_id(default_space, standardize_casing))
             constraints[f"{constraint.space}_{constraint.external_id}"] = requires
 
         return dm.ContainerApply(
             space=container_id.space,
             external_id=container_id.external_id,
             name=self.name or None,
             description=self.description,
@@ -792,15 +792,15 @@
                 prop_name = to_camel(prop.view_property) if self.standardize_casing else prop.view_property
                 view.properties[prop_name] = view_property
 
         node_types = dm.NodeApplyList([])
         parent_views = {parent for view in views for parent in view.implements or []}
         node_type_flag = False
         for view in views:
-            ref_containers = view.referenced_containers()
+            ref_containers = sorted(view.referenced_containers(), key=lambda c: c.as_tuple())
             has_data = dm.filters.HasData(containers=list(ref_containers)) if ref_containers else None
             node_type = dm.filters.Equals(["node", "type"], {"space": view.space, "externalId": view.external_id})
             if view.as_id() in parent_views:
                 view.filter = has_data
             elif has_data is None:
                 # Child filter without container properties
                 if node_type_flag:
```

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/dms_schema.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/dms_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 @dataclass
 class DMSSchema:
     spaces: dm.SpaceApplyList = field(default_factory=lambda: dm.SpaceApplyList([]))
     data_models: dm.DataModelApplyList = field(default_factory=lambda: dm.DataModelApplyList([]))
     views: dm.ViewApplyList = field(default_factory=lambda: dm.ViewApplyList([]))
     containers: dm.ContainerApplyList = field(default_factory=lambda: dm.ContainerApplyList([]))
     node_types: dm.NodeApplyList = field(default_factory=lambda: dm.NodeApplyList([]))
+    # The frozen ids are parts of the schema that should not be modified or deleted.
+    # This is used the exporting the schema.
+    frozen_ids: set[dm.ViewId | dm.ContainerId | dm.NodeId] = field(default_factory=set)
 
     _FIELD_NAME_BY_RESOURCE_TYPE: ClassVar[dict[str, str]] = {
         "container": "containers",
         "view": "views",
         "datamodel": "data_models",
         "space": "spaces",
         "node": "node_types",
```

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/_rules/information_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
         return self
 
     @model_serializer(mode="plain", when_used="always")
     def information_rules_serializer(self, info: SerializationInfo) -> dict[str, Any]:
         kwargs = vars(info)
         default_prefix = f"{self.metadata.prefix}:" if self.metadata.prefix else ""
 
-        field_names = ["Class"] if info.by_alias else ["class_"]
+        field_names = ["Class", "Value Type"] if info.by_alias else ["class_", "value_type"]
         properties = []
         for prop in self.properties:
             dumped = prop.model_dump(**kwargs)
             for field_name in field_names:
                 if value := dumped.get(field_name):
                     dumped[field_name] = value.removeprefix(default_prefix)
             properties.append(dumped)
@@ -388,15 +388,15 @@
             properties_by_class[prop.class_.versioned_id].append(self._as_dms_property(prop))
 
         views: list[DMSView] = [
             DMSView(
                 class_=cls_.class_,
                 view=ViewPropEntity(prefix=cls_.class_.prefix, suffix=cls_.class_.suffix, version=cls_.class_.version),
                 description=cls_.description,
-                implements=self._get_view_implements(cls_),
+                implements=self._get_view_implements(cls_, info_metadata),
             )
             for cls_ in self.information.classes
         ]
 
         classes_without_properties: set[str] = set()
         for class_ in self.information.classes:
             properties: list[DMSProperty] = properties_by_class.get(class_.class_.versioned_id, [])
@@ -503,19 +503,23 @@
                 ContainerEntity(prefix=prop.reference.prefix, suffix=prop.reference.suffix),
                 prop.reference.property_ or prop.property_,
             )
         else:
             return ContainerEntity(prefix=prop.class_.prefix, suffix=prop.class_.suffix), prop.property_
 
     @classmethod
-    def _get_view_implements(cls, cls_: InformationClass) -> list[ViewEntity]:
-        if isinstance(cls_.reference, ReferenceEntity):
-            return [
-                ViewPropEntity(
-                    prefix=cls_.reference.prefix, suffix=cls_.reference.suffix, version=cls_.reference.version
-                )
+    def _get_view_implements(cls, cls_: InformationClass, metadata: InformationMetadata) -> list[ViewEntity]:
+        if isinstance(cls_.reference, ReferenceEntity) and cls_.reference.prefix != metadata.prefix:
+            # We use the reference for implements if it is in a different namespace
+            implements = [
+                ViewEntity(prefix=cls_.reference.prefix, suffix=cls_.reference.suffix, version=cls_.reference.version)
             ]
         else:
-            return [
+            implements = []
+
+        implements.extend(
+            [
                 ViewEntity(prefix=parent.prefix, suffix=parent.suffix, version=parent.version)
                 for parent in cls_.parent or []
             ]
+        )
+        return implements
```

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/rules.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.70.1/cognite/neat/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/cdf.py` & `cognite_neat-0.70.1/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.70.1/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/exceptions.py` & `cognite_neat-0.70.1/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.70.1/cognite/neat/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/text.py` & `cognite_neat-0.70.1/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/utils.py` & `cognite_neat-0.70.1/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/utils/xml.py` & `cognite_neat-0.70.1/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.70.1/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/base.py` & `cognite_neat-0.70.1/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.70.1/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Export DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Import DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Validate Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.70.1/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/manager.py` & `cognite_neat-0.70.1/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.70.1/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.70.1/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/model.py` & `cognite_neat-0.70.1/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.70.1/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/tasks.py` & `cognite_neat-0.70.1/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/cognite/neat/workflows/triggers.py` & `cognite_neat-0.70.1/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.70.0/pyproject.toml` & `cognite_neat-0.70.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.70.0"
+version = "0.70.1"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.70.0/PKG-INFO` & `cognite_neat-0.70.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.70.0
+Version: 0.70.1
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```
