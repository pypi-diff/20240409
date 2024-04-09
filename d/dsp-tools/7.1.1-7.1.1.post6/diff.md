# Comparing `tmp/dsp_tools-7.1.1.tar.gz` & `tmp/dsp_tools-7.1.1.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.1.1.tar", max compression
+gzip compressed data, was "dsp_tools-7.1.1.post6.tar", max compression
```

## Comparing `dsp_tools-7.1.1.tar` & `dsp_tools-7.1.1.post6.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    35149 2024-03-27 13:03:30.201465 dsp_tools-7.1.1/LICENSE
--rw-r--r--   0        0        0     4941 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/docs/index.md
--rw-r--r--   0        0        0     8246 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     7360 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    12476 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9819 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15940 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0     8065 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0      501 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0     6313 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13116 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11533 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11795 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21297 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    75692 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.217465 dsp_tools-7.1.1/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    19452 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28334 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     4200 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    14112 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0     1334 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     5428 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6751 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0      812 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      675 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     2236 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlallow.py
--rw-r--r--   0        0        0      548 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
--rw-r--r--   0        0        0     1437 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
--rw-r--r--   0        0        0     2026 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
--rw-r--r--   0        0        0     5164 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlresource.py
--rw-r--r--   0        0        0     4004 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
--rw-r--r--   0        0        0     3466 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3063 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    13023 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4585 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5724 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3068 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4237 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7727 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    22342 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0     2876 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2536 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    24358 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-03-27 13:03:30.221465 dsp_tools-7.1.1/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    44347 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    33977 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3264 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0      893 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/json_ld_util.py
--rw-r--r--   0        0        0     1157 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5751 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      545 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0     4464 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     7194 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-03-27 13:03:30.225465 dsp_tools-7.1.1/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6311 1970-01-01 00:00:00.000000 dsp_tools-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 09:09:11.738474 dsp_tools-7.1.1.post6/LICENSE
+-rw-r--r--   0        0        0     4941 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/docs/index.md
+-rw-r--r--   0        0        0     8363 2024-04-09 09:09:49.430515 dsp_tools-7.1.1.post6/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     7360 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    12476 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9819 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0     8065 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0      501 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0     6313 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13147 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11571 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21350 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    75692 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    19520 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-04-09 09:09:11.754474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28334 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     4200 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    14112 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0     1334 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     5428 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6751 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0      812 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      675 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     2236 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlallow.py
+-rw-r--r--   0        0        0      548 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1437 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
+-rw-r--r--   0        0        0     2026 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
+-rw-r--r--   0        0        0     5164 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlresource.py
+-rw-r--r--   0        0        0     4004 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
+-rw-r--r--   0        0        0     3466 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3063 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    13023 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4585 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5724 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3068 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4237 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7727 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    22348 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2536 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    24358 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-04-09 09:09:11.758474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    44347 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    33977 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3295 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0      893 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/json_ld_util.py
+-rw-r--r--   0        0        0     1157 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5751 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      545 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0     4464 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     7194 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-04-09 09:09:11.762474 dsp_tools-7.1.1.post6/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6317 1970-01-01 00:00:00.000000 dsp_tools-7.1.1.post6/PKG-INFO
```

### Comparing `dsp_tools-7.1.1/LICENSE` & `dsp_tools-7.1.1.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/docs/index.md` & `dsp_tools-7.1.1.post6/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/pyproject.toml` & `dsp_tools-7.1.1.post6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.1.1"
+version = "7.1.1.post6"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -21,46 +21,48 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.12"
 jsonpath-ng = "^1.6.1"
 argparse = "^1.4.0"
-lxml = "^5.1.0"
+lxml = "^5.2.1"
 requests = "^2.31.0"
-jsonschema = "^4.20.0"
+jsonschema = "^4.21.1"
 openpyxl = "^3.1.2"
 networkx = "^3.2.1"
-pandas = {version = "^2.1.4", extras = ["excel"]}  # extra package that contains xlrd that is necessary for reading old .xls Excel files
+pandas = {version = "^2.2.1", extras = ["excel"]}  # extra package that contains xlrd that is necessary for reading old .xls Excel files
 regex = "^2023.12.25"
 pyyaml = "^6.0.1"
-rustworkx = "^0.14.0"
+rustworkx = "^0.14.2"
 termcolor = "^2.4.0"
-packaging = "^23.2"
+packaging = "^24.0"
 loguru = "^0.7.2"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs = "^1.5.3"
-mkdocs-material = "^9.5.3"
-mkdocs-include-markdown-plugin = "^6.0.4"
-mypy = "^1.8.0"
-pytest = "^8.0.0"
-pre-commit = "^3.6.0"
+mkdocs-material = "^9.5.17"
+mkdocs-include-markdown-plugin = "^6.0.5"
+mypy = "^1.9.0"
+pytest = "^8.1.1"
+pre-commit = "^3.7.0"
 darglint = "^1.8.1"
-types-requests = "^2.31.0.20240106"
-types-lxml = ">=2023.10.21,<2025.0.0"
-types-jsonschema = "^4.20.0.20240105"
-types-openpyxl = "^3.1.0.20240106"
-types-regex = "^2023.12.25.20240106"
-types-pyyaml = "^6.0.12.12"
-pytest-unordered = "^0.5.2"
-viztracer = "^0.16.1"
-ruff = ">=0.1.12,<0.4.0"
-pytest-sugar = ">=0.9.7,<1.1.0"
+types-requests = "^2.31.0.20240403"
+types-lxml = "^2024.3.27"
+types-jsonschema = "^4.21.0.20240331"
+types-openpyxl = "^3.1.0.20240402"
+types-regex = "^2023.12.25.20240311"
+types-pyyaml = "^6.0.12.20240311"
+pytest-unordered = "^0.6.0"
+viztracer = "^0.16.2"
+ruff = "^0.3.5"
+pytest-sugar = "^1.0.0"
+pandas-stubs = "^2.2.1.240316"
+types-networkx = "^3.2.1.20240331"
 
 
 [tool.poetry.scripts]
 dsp-tools = "dsp_tools.cli.entry_point:main"  # definition of the CLI entry point
 
 
 [tool.poetry-exec-plugin.commands]
@@ -126,15 +128,14 @@
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 # see https://docs.pytest.org/en/latest/explanation/goodpractices.html#tests-outside-application-code
 pythonpath = [".", "src", "test"]
 
 
 [tool.mypy]
-ignore_missing_imports = true                                 # TODO: deactivate this
 show_column_numbers = true
 strict = true
 exclude = [
     "src/dsp_tools/models/datetimestamp.py",                  # TODO: activate this
     "src/dsp_tools/models/langstring.py",                     # TODO: activate this
     "src/dsp_tools/models/projectContext.py",                 # TODO: activate this
     "src/dsp_tools/commands/project/models/context.py",       # TODO: activate this
@@ -145,14 +146,19 @@
     "src/dsp_tools/commands/project/models/project.py",       # TODO: activate this
     "src/dsp_tools/commands/project/models/propertyclass.py", # TODO: activate this
     "src/dsp_tools/commands/project/models/resourceclass.py", # TODO: activate this
     "src/dsp_tools/commands/project/models/user.py",          # TODO: activate this
 ]
 
 
+[[tool.mypy.overrides]]
+module = ["jsonpath_ng.*", "viztracer.*"]  # For these packages, no type stubs are available yet
+ignore_missing_imports = true
+
+
 [tool.ruff]
 line-length = 120
 target-version = "py311"
 
 
 [tool.ruff.lint]
 select = [
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/cli/call_action.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/cli/create_parsers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/cli/entry_point.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/lists.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import importlib.resources
 import json
 from copy import deepcopy
 from pathlib import Path
 from typing import Any
 from typing import Optional
 from typing import Union
+from typing import cast
 
 import jsonschema
 import regex
 from openpyxl import load_workbook
 from openpyxl.cell import Cell
 from openpyxl.worksheet.worksheet import Worksheet
 
@@ -321,15 +322,15 @@
             "nodes": _list["nodes"],
         }
 
     return finished_lists
 
 
 def _read_and_check_workbook(excelpath: Path) -> Worksheet:
-    all_worksheets = load_workbook(excelpath, read_only=True).worksheets
+    all_worksheets = cast(list[Worksheet], load_workbook(excelpath, read_only=True).worksheets)
     if len(all_worksheets) != 1:
         msg = MoreThanOneSheetProblem(excelpath.name, [x.title for x in all_worksheets]).execute_error_protocol()
         raise InputError(msg)
     return all_worksheets[0]
 
 
 def validate_lists_section_with_schema(
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
             and the success status (True if everything went well)
     """
 
     property_df = _read_check_property_df(excelfile)
 
     property_df = _rename_deprecated_columnnames(df=property_df, excelfile=excelfile)
 
-    _do_property_excel_compliance(df=property_df, excelfile=excelfile)
-
     # Not all columns have to be filled, users may delete some for ease of use, but it would generate an error later
     property_df = _add_optional_columns(df=property_df)
 
+    _do_property_excel_compliance(df=property_df, excelfile=excelfile)
+
     # transform every row into a property
     props = [
         _row2prop(
             df_row=row,
             row_num=int(str(index)) + 2,  # index is a label/index/hashable, but we need an int
             excelfile=excelfile,
         )
@@ -79,15 +79,15 @@
         with open(file=path_to_output_file, mode="w", encoding="utf-8") as file:
             json.dump(props, file, indent=4, ensure_ascii=False)
             print(f"properties section was created successfully and written to file '{path_to_output_file}'")
 
     return props, True
 
 
-def _read_check_property_df(excelfile: str) -> pd.DataFrame | None:
+def _read_check_property_df(excelfile: str) -> pd.DataFrame:
     sheets_df_dict = read_and_clean_all_sheets(excelfile=excelfile)
     if len(sheets_df_dict) != 1:
         msg = MoreThanOneSheetProblem("properties.xlsx", list(sheets_df_dict.keys())).execute_error_protocol()
         raise InputError(msg)
     return next(iter(sheets_df_dict.values()))
 
 
@@ -162,36 +162,36 @@
         "comment_it",
         "comment_rm",
         "subject",
     }
     in_df_cols = set(df.columns)
     if not optional_col_set.issubset(in_df_cols):
         additional_col = list(optional_col_set.difference(in_df_cols))
-        additional_df = pd.DataFrame(columns=additional_col, index=df.index, data=pd.NA)
+        additional_df = pd.DataFrame(columns=additional_col, index=df.index)
         df = pd.concat(objs=[df, additional_df], axis=1)
     return df
 
 
 def _check_missing_values_in_row(df: pd.DataFrame) -> None | list[MissingValuesInRowProblem]:
     required_values = ["name", "super", "object", "gui_element"]
     missing_dict = check_required_values(df=df, required_values_columns=required_values)
     missing_labels = find_one_full_cell_in_cols(df=df, required_columns=language_label_col)
     if missing_labels is not None:
         missing_dict.update({"label": missing_labels})
     missing_gui_attributes = _check_compliance_gui_attributes(df=df)
     if missing_gui_attributes is not None:
         missing_dict.update(missing_gui_attributes)
     if missing_dict:
-        missing_dict = get_wrong_row_numbers(wrong_row_dict=missing_dict, true_remains=True)
-        return [MissingValuesInRowProblem(column=col, row_numbers=row_nums) for col, row_nums in missing_dict.items()]
+        missing_int_dict = get_wrong_row_numbers(wrong_row_dict=missing_dict, true_remains=True)
+        return [MissingValuesInRowProblem(col, row_nums) for col, row_nums in missing_int_dict.items()]
     else:
         return None
 
 
-def _check_compliance_gui_attributes(df: pd.DataFrame) -> dict[str, pd.Series] | None:
+def _check_compliance_gui_attributes(df: pd.DataFrame) -> dict[str, pd.Series[bool]] | None:
     mandatory_attributes = ["Spinbox", "List"]
     mandatory_check = col_must_or_not_empty_based_on_other_col(
         df=df,
         substring_list=mandatory_attributes,
         substring_colname="gui_element",
         check_empty_colname="gui_attributes",
         must_have_value=True,
@@ -204,23 +204,23 @@
         check_empty_colname="gui_attributes",
         must_have_value=False,
     )
     match mandatory_check, no_attribute_check:
         case None, None:
             return None
         case pd.Series(), pd.Series():
-            final_series = pd.Series(np.logical_or(mandatory_check, no_attribute_check))  # type: ignore[arg-type]
+            final_series: pd.Series[bool] = pd.Series(np.logical_or(mandatory_check, no_attribute_check))  # type: ignore[arg-type]
         case pd.Series(), None:
-            final_series = mandatory_check
+            final_series = mandatory_check  # type: ignore[assignment]
         case None, pd.Series:
             final_series = no_attribute_check
     return {"gui_attributes": final_series}
 
 
-def _row2prop(df_row: pd.Series, row_num: int, excelfile: str) -> dict[str, Any]:
+def _row2prop(df_row: pd.Series[Any], row_num: int, excelfile: str) -> dict[str, Any]:
     _property = {x: df_row[x] for x in mandatory_properties} | {
         "labels": get_labels(df_row=df_row),
         "super": [s.strip() for s in df_row["super"].split(",")],
     }
     if not pd.isna(df_row["subject"]):
         _property["subject"] = df_row["subject"]
 
@@ -235,15 +235,15 @@
     if comment := get_comments(df_row=df_row):
         _property["comments"] = comment
 
     return _property
 
 
 def _get_gui_attribute(
-    df_row: pd.Series,
+    df_row: pd.Series[Any],
     row_num: int,
 ) -> dict[str, int | str | float] | InvalidExcelContentProblem | None:
     if pd.isnull(df_row["gui_attributes"]):
         return None
     # If the attribute is not in the correct format, a called function may raise an IndexError
     try:
         return _format_gui_attribute(attribute_str=df_row["gui_attributes"])
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib.resources
 import json
 import warnings
 from typing import Any
 from typing import Optional
 
 import jsonpath_ng.ext
@@ -92,15 +94,15 @@
     return JsonValidationResourceProblem(
         original_msg=validation_error.message,
         message_path=validation_error.json_path,
     )
 
 
 def _row2resource(
-    class_info_row: pd.Series,
+    class_info_row: pd.Series[Any],
     class_df_with_cardinalities: pd.DataFrame,
 ) -> dict[str, Any]:
     """
     Method that reads one row from the "classes" DataFrame,
     opens the corresponding details DataFrame,
     and builds a dict object of the resource.
 
@@ -266,15 +268,15 @@
 def _validate_excel_file(classes_df: pd.DataFrame, df_dict: dict[str, pd.DataFrame]) -> list[Problem]:
     if any(classes_df.get(lang) is not None for lang in languages):
         warnings.warn(
             f"The file 'resources.xlsx' uses {languages} as column titles, which is deprecated. "
             f"Please use {[f'label_{lang}' for lang in languages]}"
         )
     problems: list[Problem] = []
-    if missing_super_rows := [int(index) + 2 for index, row in classes_df.iterrows() if not check_notna(row["super"])]:
+    if missing_super_rows := [int(str(i)) + 2 for i, row in classes_df.iterrows() if not check_notna(row["super"])]:
         problems.append(MissingValuesInRowProblem(column="super", row_numbers=missing_super_rows))
     if duplicate_check := check_column_for_duplicate(classes_df, "name"):
         problems.append(duplicate_check)
     # check that all the sheets have an entry in the names column and vice versa
     if (all_names := set(classes_df["name"].tolist())) != (all_sheets := set(df_dict)):
         problems.append(ResourcesSheetsNotAsExpected(all_names, all_sheets))
     return problems
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2json/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from pathlib import Path
+from typing import Any
 from unittest import mock
 
 import numpy as np
 import pandas as pd
 import regex
 
 from dsp_tools.commands.excel2json.models.input_error import DuplicatesInColumnProblem
@@ -113,15 +114,15 @@
             column=to_check_column,
             duplicate_values=duplicate_values,
         )
     else:
         return None
 
 
-def check_required_values(df: pd.DataFrame, required_values_columns: list[str]) -> dict[str, pd.Series]:
+def check_required_values(df: pd.DataFrame, required_values_columns: list[str]) -> dict[str, pd.Series[bool]]:
     """
     If there are any empty cells in the column, it adds the column name and a boolean pd.Series to the dictionary.
     If there are no empty cells, then it is not included in the dictionary.
     If no column has any empty cells, then it returns an empty dictionary.
 
     Args:
         df: pd.DataFrame that is checked
@@ -151,50 +152,52 @@
     """
     # If the False are required, we need to invert the array.
     if not true_remains:
         series = ~series
     return list(series[series].index)
 
 
-def get_wrong_row_numbers(wrong_row_dict: dict[str, pd.Series], true_remains: bool = True) -> dict[str, list[int]]:
+def get_wrong_row_numbers(
+    wrong_row_dict: dict[str, pd.Series[bool]], true_remains: bool = True
+) -> dict[str, list[int]]:
     """
     From the boolean pd.Series the index numbers of the True values are extracted.
     The resulting list is the new value of the dictionary.
     This new dictionary is taken and to each index number 2 is added, so that it corresponds to the Excel row number.
 
     Args:
         wrong_row_dict: The dictionary which contains column names and a boolean pd.Series
         true_remains: If True then the index of True is taken, if False then the index of False values is taken
 
     Returns:
         Dictionary with the column name as key and the row number as a list.
     """
-    wrong_row_dict = {
+    wrong_row_int_dict = {
         k: turn_bool_array_into_index_numbers(series=v, true_remains=true_remains) for k, v in wrong_row_dict.items()
     }
-    return {k: [x + 2 for x in v] for k, v in wrong_row_dict.items()}
+    return {k: [x + 2 for x in v] for k, v in wrong_row_int_dict.items()}
 
 
-def get_labels(df_row: pd.Series) -> dict[str, str]:
+def get_labels(df_row: pd.Series[Any]) -> dict[str, str]:
     """
     This function takes a pd.Series which has "label_[language tag]" in the index.
     If the value of the index is not pd.NA, the language tag and the value are added to a dictionary.
     If it is empty, it is omitted from the dictionary.
 
     Args:
         df_row: a pd.Series (usually a row of a pd.DataFrame) from which the content of the columns containing the
                 label is extracted
 
     Returns:
         A dictionary with the language tag and the content of the cell
     """
-    return {lang: df_row[f"label_{lang}"] for lang in languages if df_row[f"label_{lang}"] is not pd.NA}
+    return {lang: df_row[f"label_{lang}"] for lang in languages if not pd.isna(df_row[f"label_{lang}"])}
 
 
-def get_comments(df_row: pd.Series) -> dict[str, str] | None:
+def get_comments(df_row: pd.Series[Any]) -> dict[str, str] | None:
     """
     This function takes a pd.Series which has "comment_[language tag]" in the index.
     If the value of the index is not pd.NA, the language tag and the value are added to a dictionary.
     If it is empty, it is omitted from the dictionary.
 
     Args:
         df_row: a pd.Series (usually a row of a pd.DataFrame) from which the content of the columns containing the
@@ -203,15 +206,15 @@
     Returns:
         A dictionary with the language tag and the content of the cell
     """
     comments = {lang: df_row[f"comment_{lang}"] for lang in languages if df_row[f"comment_{lang}"] is not pd.NA}
     return comments or None
 
 
-def find_one_full_cell_in_cols(df: pd.DataFrame, required_columns: list[str]) -> pd.Series | None:
+def find_one_full_cell_in_cols(df: pd.DataFrame, required_columns: list[str]) -> pd.Series[bool] | None:
     """
     This function takes a pd.DataFrame and a list of column names where at least one cell must have a value per row.
     A pd.Series with boolean values is returned, True if any rows do not have a value in at least one column
 
     Args:
         df: The pd.DataFrame which should be checked
         required_columns: A list of column names where at least one cell per row must have a value
@@ -230,15 +233,15 @@
 
 def col_must_or_not_empty_based_on_other_col(
     df: pd.DataFrame,
     substring_list: list[str],
     substring_colname: str,
     check_empty_colname: str,
     must_have_value: bool,
-) -> pd.Series | None:
+) -> pd.Series[bool] | None:
     """
     It is presumed that the column "substring_colname" has no empty cells.
     Based on the string content of the individual rows, which is specified in the "substring_list",
     the cell in the column "check_empty_colname" is checked whether it is empty or not.
     The "substring_list" contains the different possibilities regarding the content of the cell.
     If the parameter "must_have_value" is True, then the cell in the "check_empty_colname" column must not be empty.
     If the parameter is set to False, then it must be empty.
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import warnings
 from pathlib import Path
+from typing import Any
 from typing import Callable
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 import regex
 from lxml import etree
@@ -162,15 +163,15 @@
         resources.append(resource)
 
     return resources
 
 
 def _append_bitstream_to_resource(
     resource: etree._Element,
-    row: pd.Series,
+    row: pd.Series[Any],
     row_number: int,
 ) -> etree._Element:
     """
     Create a bitstream-prop element, and append it to the resource.
     If the file permissions are missing, try to deduce them from the resource permissions.
 
     Args:
@@ -206,15 +207,15 @@
         )
     )
     return resource
 
 
 def _convert_resource_row_to_xml(
     row_number: int,
-    row: pd.Series,
+    row: pd.Series[Any],
 ) -> etree._Element:
     """
     Convert a resource-row to an XML resource element.
     First, check if the mandatory cells are present.
     Then, call the appropriate function, depending on the restype (Resource, LinkObj, Annotation, Region).
 
     Args:
@@ -287,15 +288,15 @@
                     row_number=row_number,
                 )
 
     return resource
 
 
 def _get_prop_function(
-    row: pd.Series,
+    row: pd.Series[Any],
     resource_id: str,
 ) -> Callable[..., etree._Element]:
     """
     Return the function that creates the appropriate property, depending on the proptype.
 
     Args:
         row: row of the CSV/Excel sheet that defines the property
@@ -324,15 +325,15 @@
     }
     if row.get("prop type") not in proptype_2_function:
         raise BaseError(f"Invalid prop type for property {row.get('prop name')} in resource {resource_id}")
     return proptype_2_function[row["prop type"]]
 
 
 def _convert_row_to_property_elements(
-    row: pd.Series,
+    row: pd.Series[Any],
     max_num_of_props: int,
     row_number: int,
     resource_id: str,
 ) -> list[PropertyElement]:
     """
     Every property contains i elements,
     which are represented in the Excel as groups of columns named
@@ -395,15 +396,15 @@
         )
 
     return property_elements
 
 
 def _convert_property_row_to_xml(
     row_number: int,
-    row: pd.Series,
+    row: pd.Series[Any],
     max_num_of_props: int,
     resource_id: str,
 ) -> etree._Element:
     """
     Convert a property-row of the CSV/Excel sheet to an XML element.
 
     Args:
@@ -439,15 +440,15 @@
         property_elements=property_elements,
         resource_id=resource_id,
     )
 
 
 def _create_property(
     make_prop_function: Callable[..., etree._Element],
-    row: pd.Series,
+    row: pd.Series[Any],
     property_elements: list[PropertyElement],
     resource_id: str,
 ) -> etree._Element:
     """
     Create a property based on the appropriate function and the property elements.
 
     Args:
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib.resources
 import json
 from pathlib import Path
 from typing import Any
 from typing import Union
 
 import jsonpath_ng
@@ -416,25 +418,25 @@
                         dependencies[resname][cardname] = targets
                         cardinalities[resname][cardname] = card["cardinality"]
                     else:
                         dependencies[resname][cardname].extend(targets)
     return cardinalities, dependencies
 
 
-def _make_cardinality_dependency_graph(dependencies: dict[str, dict[str, list[str]]]) -> nx.MultiDiGraph:
-    graph = nx.MultiDiGraph()
+def _make_cardinality_dependency_graph(dependencies: dict[str, dict[str, list[str]]]) -> nx.MultiDiGraph[Any]:
+    graph: nx.MultiDiGraph[Any] = nx.MultiDiGraph()
     for start, cards in dependencies.items():
         for edge, targets in cards.items():
             for target in targets:
                 graph.add_edge(start, target, edge)
     return graph
 
 
 def _find_circles_with_min_one_cardinality(
-    graph: nx.MultiDiGraph, cardinalities: dict[str, dict[str, str]], dependencies: dict[str, dict[str, list[str]]]
+    graph: nx.MultiDiGraph[Any], cardinalities: dict[str, dict[str, str]], dependencies: dict[str, dict[str, list[str]]]
 ) -> set[tuple[str, str]]:
     errors: set[tuple[str, str]] = set()
     circles = list(nx.algorithms.cycles.simple_cycles(graph))
     for circle in circles:
         for index, resource in enumerate(circle):
             target = circle[(index + 1) % len(circle)]
             prop = ""
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/start_stack.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/template.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlallow.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlpermission.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlproperty.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlresource.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/models/xmlvalue.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files 0% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         return resource_create_client.create_resource(resource, bitstream_information)
     except PermanentTimeOutError as err:
         # The following block catches all exceptions and handles them in a generic way.
         # Because the calling function needs to know that this was a PermanentTimeOutError, we need to catch and
         # raise it here.
         raise err
     except Exception as err:  # noqa: BLE001 (blind-except)
-        msg = f"{datetime.now()}: WARNING: Unable to create resource '{resource.label}' ({resource.res_id})"
+        msg = f"{datetime.now()}: WARNING: Unable to create resource '{resource.label}' (ID: '{resource.res_id}')"
         if isinstance(err, BaseError):
             msg = f"{msg}: {err.message}"
         print(msg)
         log_msg = (
             f"Unable to create resource '{resource.label}' ({resource.res_id})\n"
             f"Resource details:\n{vars(resource)}\n"
             f"Property details:\n" + "\n".join([str(vars(prop)) for prop in resource.properties])
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/models/langstring.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.1.1.post6/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
       - KNORA_WEBAPI_TRIPLESTORE_FUSEKI_PASSWORD=test
       - KNORA_WEBAPI_CACHE_SERVICE_ENABLED=true
       - KNORA_WEBAPI_CACHE_SERVICE_REDIS_HOST=redis
       - KNORA_WEBAPI_CACHE_SERVICE_REDIS_PORT=6379
       - KNORA_WEBAPI_ALLOW_RELOAD_OVER_HTTP=true
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
+      - DSP_API_LOG_LEVEL=INFO
 
   sipi:
     # on the verge of every deployment (fortnightly), take the same tag as DSP-API
     image: daschswiss/knora-sipi:v30.10.1
     ports:
       - "1024:1024"
     volumes:
```

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/connection.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/connection_live.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/json_ld_util.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/json_ld_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/shared.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/xml_validation.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.1.1.post6/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.1/PKG-INFO` & `dsp_tools-7.1.1.post6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.1.1
+Version: 7.1.1.post6
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: jsonpath-ng (>=1.6.1,<2.0.0)
-Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
+Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: packaging (>=23.2,<24.0)
-Requires-Dist: pandas[excel] (>=2.1.4,<3.0.0)
+Requires-Dist: packaging (>=24.0,<25.0)
+Requires-Dist: pandas[excel] (>=2.2.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rustworkx (>=0.14.0,<0.15.0)
+Requires-Dist: rustworkx (>=0.14.2,<0.15.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Project-URL: Documentation, https://docs.dasch.swiss/latest/DSP-TOOLS/
 Project-URL: Repository, https://github.com/dasch-swiss/dsp-tools
 Description-Content-Type: text/markdown
 
 [![](https://img.shields.io/pypi/v/dsp-tools.svg)](https://pypi.org/project/dsp-tools/) 
 [![](https://img.shields.io/pypi/l/dsp-tools.svg)](https://pypi.org/project/dsp-tools/)
```

