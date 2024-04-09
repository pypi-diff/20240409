# Comparing `tmp/semantha_sdk-6.8.0.tar.gz` & `tmp/semantha_sdk-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-6.8.0.tar", max compression
+gzip compressed data, was "semantha_sdk-6.9.0.tar", max compression
```

## Comparing `semantha_sdk-6.8.0.tar` & `semantha_sdk-6.9.0.tar`

### file list

```diff
@@ -1,236 +1,236 @@
--rw-r--r--   0        0        0     4920 2024-02-09 13:13:46.949533 semantha_sdk-6.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    14295 2024-02-02 10:08:22.192283 semantha_sdk-6.8.0/DOCU.md
--rw-r--r--   0        0        0    11545 2023-08-25 14:25:28.084953 semantha_sdk-6.8.0/LICENSE
--rw-r--r--   0        0        0     1697 2024-01-30 09:55:05.647416 semantha_sdk-6.8.0/pyproject.toml
--rw-r--r--   0        0        0     4900 2023-10-27 15:25:37.958117 semantha_sdk-6.8.0/README.md
--rw-r--r--   0        0        0     2671 2024-02-02 10:08:22.224282 semantha_sdk-6.8.0/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 10:09:00.937800 semantha_sdk-6.8.0/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     2015 2024-02-02 10:09:00.939800 semantha_sdk-6.8.0/semantha_sdk/api/answers.py
--rw-r--r--   0        0        0      942 2024-02-02 10:09:00.941798 semantha_sdk-6.8.0/semantha_sdk/api/bulk.py
--rw-r--r--   0        0        0      765 2024-02-02 10:09:00.944798 semantha_sdk-6.8.0/semantha_sdk/api/bulk_domains.py
--rw-r--r--   0        0        0      749 2024-02-02 10:09:00.946797 semantha_sdk-6.8.0/semantha_sdk/api/bulk_model.py
--rw-r--r--   0        0        0     1777 2024-02-02 10:09:00.948798 semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_documentclasses.py
--rw-r--r--   0        0        0     1484 2024-02-02 10:09:00.951799 semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_documenttypes.py
--rw-r--r--   0        0        0     1823 2024-02-02 10:09:00.953796 semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_domain.py
--rw-r--r--   0        0        0     4084 2024-02-02 10:09:00.955798 semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_referencedocuments.py
--rw-r--r--   0        0        0     3221 2024-02-02 10:09:00.958799 semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_references.py
--rw-r--r--   0        0        0     1284 2024-02-02 10:09:00.960799 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_boostwords.py
--rw-r--r--   0        0        0      855 2024-02-02 10:09:00.963798 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_class.py
--rw-r--r--   0        0        0     1898 2024-02-02 10:09:00.965798 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_classes.py
--rw-r--r--   0        0        0     1720 2024-02-02 10:09:00.967799 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_dataproperties.py
--rw-r--r--   0        0        0     2998 2024-02-02 10:09:00.970799 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_domain.py
--rw-r--r--   0        0        0      762 2024-02-02 10:09:00.972802 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_domains.py
--rw-r--r--   0        0        0     1647 2024-02-02 10:09:00.975803 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_instances.py
--rw-r--r--   0        0        0     1693 2024-02-02 10:09:00.977805 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_metadata.py
--rw-r--r--   0        0        0     1311 2024-02-02 10:09:00.980805 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_namedentities.py
--rw-r--r--   0        0        0     1588 2024-02-02 10:09:00.982832 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_rules.py
--rw-r--r--   0        0        0     1198 2024-02-02 10:09:00.984832 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_stopwords.py
--rw-r--r--   0        0        0     1260 2024-02-02 10:09:00.986800 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_synonyms.py
--rw-r--r--   0        0        0     1124 2024-02-02 10:09:00.989800 semantha_sdk-6.8.0/semantha_sdk/api/bulkmodelclass_instances.py
--rw-r--r--   0        0        0      965 2024-02-02 10:09:00.991799 semantha_sdk-6.8.0/semantha_sdk/api/celltypes.py
--rw-r--r--   0        0        0     1188 2024-02-02 10:09:00.994799 semantha_sdk-6.8.0/semantha_sdk/api/child_extractorclasses.py
--rw-r--r--   0        0        0     1256 2024-02-02 10:19:05.165213 semantha_sdk-6.8.0/semantha_sdk/api/clone.py
--rw-r--r--   0        0        0     6276 2024-02-08 07:35:59.946903 semantha_sdk-6.8.0/semantha_sdk/api/clusters.py
--rw-r--r--   0        0        0     1197 2024-02-02 10:09:01.000801 semantha_sdk-6.8.0/semantha_sdk/api/currentuser.py
--rw-r--r--   0        0        0     1361 2024-02-02 10:09:01.003831 semantha_sdk-6.8.0/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     1093 2024-02-02 10:09:01.005819 semantha_sdk-6.8.0/semantha_sdk/api/docclass_customfields.py
--rw-r--r--   0        0        0     2217 2024-02-02 10:09:01.007800 semantha_sdk-6.8.0/semantha_sdk/api/docclass_documentclasses.py
--rw-r--r--   0        0        0     1705 2024-02-02 10:09:01.010799 semantha_sdk-6.8.0/semantha_sdk/api/docclass_referencedocuments.py
--rw-r--r--   0        0        0     3968 2024-02-02 10:19:05.171396 semantha_sdk-6.8.0/semantha_sdk/api/documentannotations.py
--rw-r--r--   0        0        0     2505 2024-02-02 10:09:01.015836 semantha_sdk-6.8.0/semantha_sdk/api/documentclass.py
--rw-r--r--   0        0        0     1969 2024-02-02 10:09:01.017835 semantha_sdk-6.8.0/semantha_sdk/api/documentclasses.py
--rw-r--r--   0        0        0     9757 2024-02-08 07:35:59.947902 semantha_sdk-6.8.0/semantha_sdk/api/documents.py
--rw-r--r--   0        0        0     1975 2024-02-02 10:19:05.185908 semantha_sdk-6.8.0/semantha_sdk/api/documenttype.py
--rw-r--r--   0        0        0     2041 2024-02-02 10:19:05.192622 semantha_sdk-6.8.0/semantha_sdk/api/documenttypes.py
--rw-r--r--   0        0        0     4816 2024-02-02 10:09:01.027833 semantha_sdk-6.8.0/semantha_sdk/api/domain.py
--rw-r--r--   0        0        0     1234 2024-02-02 10:09:01.029834 semantha_sdk-6.8.0/semantha_sdk/api/domains.py
--rw-r--r--   0        0        0      930 2024-02-02 10:09:01.032833 semantha_sdk-6.8.0/semantha_sdk/api/info.py
--rw-r--r--   0        0        0     1675 2024-02-02 10:09:01.034799 semantha_sdk-6.8.0/semantha_sdk/api/languages.py
--rw-r--r--   0        0        0     1545 2024-02-02 10:09:01.036798 semantha_sdk-6.8.0/semantha_sdk/api/model.py
--rw-r--r--   0        0        0     1044 2024-02-02 10:09:01.038833 semantha_sdk-6.8.0/semantha_sdk/api/model_attributes.py
--rw-r--r--   0        0        0      961 2024-02-02 10:09:01.041799 semantha_sdk-6.8.0/semantha_sdk/api/model_backups.py
--rw-r--r--   0        0        0     1485 2024-02-02 10:09:01.043800 semantha_sdk-6.8.0/semantha_sdk/api/model_boostword.py
--rw-r--r--   0        0        0     1896 2024-02-02 10:09:01.045799 semantha_sdk-6.8.0/semantha_sdk/api/model_boostwords.py
--rw-r--r--   0        0        0     2060 2024-02-02 10:09:01.048798 semantha_sdk-6.8.0/semantha_sdk/api/model_dataproperties.py
--rw-r--r--   0        0        0     1530 2024-02-02 10:09:01.050800 semantha_sdk-6.8.0/semantha_sdk/api/model_dataproperty.py
--rw-r--r--   0        0        0      865 2024-02-02 10:09:01.053832 semantha_sdk-6.8.0/semantha_sdk/api/model_datatypes.py
--rw-r--r--   0        0        0     5886 2024-02-02 10:09:01.055834 semantha_sdk-6.8.0/semantha_sdk/api/model_domain.py
--rw-r--r--   0        0        0      742 2024-02-02 10:09:01.057832 semantha_sdk-6.8.0/semantha_sdk/api/model_domains.py
--rw-r--r--   0        0        0     1861 2024-02-02 10:09:01.060799 semantha_sdk-6.8.0/semantha_sdk/api/model_extractorclass.py
--rw-r--r--   0        0        0     2476 2024-02-02 10:09:01.062800 semantha_sdk-6.8.0/semantha_sdk/api/model_extractorclasses.py
--rw-r--r--   0        0        0      976 2024-02-02 10:09:01.064799 semantha_sdk-6.8.0/semantha_sdk/api/model_extractors.py
--rw-r--r--   0        0        0      880 2024-02-02 10:09:01.067800 semantha_sdk-6.8.0/semantha_sdk/api/model_extractortypes.py
--rw-r--r--   0        0        0      994 2024-02-02 10:09:01.069799 semantha_sdk-6.8.0/semantha_sdk/api/model_formatters.py
--rw-r--r--   0        0        0     1933 2024-02-02 10:09:01.071799 semantha_sdk-6.8.0/semantha_sdk/api/model_metadata.py
--rw-r--r--   0        0        0      877 2024-02-02 10:09:01.078798 semantha_sdk-6.8.0/semantha_sdk/api/model_metadatatypes.py
--rw-r--r--   0        0        0     1942 2024-02-02 10:09:01.080798 semantha_sdk-6.8.0/semantha_sdk/api/model_namedentities.py
--rw-r--r--   0        0        0     1519 2024-02-02 10:09:01.083800 semantha_sdk-6.8.0/semantha_sdk/api/model_namedentity.py
--rw-r--r--   0        0        0     1007 2024-02-02 10:09:01.086798 semantha_sdk-6.8.0/semantha_sdk/api/model_objectproperties.py
--rw-r--r--   0        0        0     1518 2024-02-02 10:09:01.088801 semantha_sdk-6.8.0/semantha_sdk/api/model_onemetadata.py
--rw-r--r--   0        0        0     1426 2024-02-02 10:09:01.091801 semantha_sdk-6.8.0/semantha_sdk/api/model_regex.py
--rw-r--r--   0        0        0     1822 2024-02-02 10:09:01.093798 semantha_sdk-6.8.0/semantha_sdk/api/model_regexes.py
--rw-r--r--   0        0        0     1469 2024-02-02 10:09:01.096802 semantha_sdk-6.8.0/semantha_sdk/api/model_relation.py
--rw-r--r--   0        0        0     1874 2024-02-02 10:09:01.098835 semantha_sdk-6.8.0/semantha_sdk/api/model_relations.py
--rw-r--r--   0        0        0     1413 2024-02-02 10:09:01.101798 semantha_sdk-6.8.0/semantha_sdk/api/model_rule.py
--rw-r--r--   0        0        0     1024 2024-02-02 10:09:01.103833 semantha_sdk-6.8.0/semantha_sdk/api/model_rulefunctions.py
--rw-r--r--   0        0        0     1934 2024-02-02 10:09:01.106799 semantha_sdk-6.8.0/semantha_sdk/api/model_rules.py
--rw-r--r--   0        0        0     1474 2024-02-02 10:09:01.108834 semantha_sdk-6.8.0/semantha_sdk/api/model_stopword.py
--rw-r--r--   0        0        0     1879 2024-02-02 10:09:01.111801 semantha_sdk-6.8.0/semantha_sdk/api/model_stopwords.py
--rw-r--r--   0        0        0     1455 2024-02-02 10:09:01.113835 semantha_sdk-6.8.0/semantha_sdk/api/model_synonym.py
--rw-r--r--   0        0        0     1854 2024-02-02 10:09:01.116805 semantha_sdk-6.8.0/semantha_sdk/api/model_synonyms.py
--rw-r--r--   0        0        0     1242 2024-02-02 10:09:01.118833 semantha_sdk-6.8.0/semantha_sdk/api/modelclasses.py
--rw-r--r--   0        0        0     3854 2024-02-02 10:09:01.121799 semantha_sdk-6.8.0/semantha_sdk/api/modelinstances.py
--rw-r--r--   0        0        0     1417 2024-02-02 10:09:01.123834 semantha_sdk-6.8.0/semantha_sdk/api/modelont_attribute.py
--rw-r--r--   0        0        0     1852 2024-02-02 10:09:01.126802 semantha_sdk-6.8.0/semantha_sdk/api/modelont_attributes.py
--rw-r--r--   0        0        0     1946 2024-02-02 10:09:01.128802 semantha_sdk-6.8.0/semantha_sdk/api/modelont_class.py
--rw-r--r--   0        0        0     2462 2024-02-02 10:09:01.131800 semantha_sdk-6.8.0/semantha_sdk/api/modelont_classes.py
--rw-r--r--   0        0        0     1475 2024-02-02 10:09:01.133801 semantha_sdk-6.8.0/semantha_sdk/api/modelont_instance.py
--rw-r--r--   0        0        0     2608 2024-02-02 10:09:01.136798 semantha_sdk-6.8.0/semantha_sdk/api/modelont_instances.py
--rw-r--r--   0        0        0     1218 2024-02-02 10:09:01.138801 semantha_sdk-6.8.0/semantha_sdk/api/modelontclass_instances.py
--rw-r--r--   0        0        0     1797 2024-02-08 07:35:59.949912 semantha_sdk-6.8.0/semantha_sdk/api/namedentities.py
--rw-r--r--   0        0        0     1780 2024-02-08 07:35:59.951919 semantha_sdk-6.8.0/semantha_sdk/api/paragraph.py
--rw-r--r--   0        0        0      718 2024-02-02 10:09:01.146798 semantha_sdk-6.8.0/semantha_sdk/api/paragraphs.py
--rw-r--r--   0        0        0     2526 2024-02-08 07:35:59.953901 semantha_sdk-6.8.0/semantha_sdk/api/referencedocument.py
--rw-r--r--   0        0        0    16151 2024-02-08 07:35:59.955904 semantha_sdk-6.8.0/semantha_sdk/api/referencedocuments.py
--rw-r--r--   0        0        0    22237 2024-02-02 10:09:01.154799 semantha_sdk-6.8.0/semantha_sdk/api/references.py
--rw-r--r--   0        0        0      870 2024-02-02 10:09:01.156800 semantha_sdk-6.8.0/semantha_sdk/api/roles.py
--rw-r--r--   0        0        0     2430 2024-02-02 10:09:01.159798 semantha_sdk-6.8.0/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0     1019 2024-02-08 07:35:59.957901 semantha_sdk-6.8.0/semantha_sdk/api/sentence.py
--rw-r--r--   0        0        0      712 2024-02-02 10:09:01.164839 semantha_sdk-6.8.0/semantha_sdk/api/sentences.py
--rw-r--r--   0        0        0     1643 2024-02-02 10:09:01.167806 semantha_sdk-6.8.0/semantha_sdk/api/settings.py
--rw-r--r--   0        0        0     5025 2024-02-02 10:09:01.170807 semantha_sdk-6.8.0/semantha_sdk/api/similaritymatrix.py
--rw-r--r--   0        0        0     3871 2024-02-02 10:09:01.173807 semantha_sdk-6.8.0/semantha_sdk/api/similaritymatrix_cluster.py
--rw-r--r--   0        0        0     1015 2024-02-02 10:09:01.175800 semantha_sdk-6.8.0/semantha_sdk/api/statistic.py
--rw-r--r--   0        0        0     1485 2024-02-02 10:09:01.178834 semantha_sdk-6.8.0/semantha_sdk/api/summarizations.py
--rw-r--r--   0        0        0      863 2024-02-02 10:09:01.180834 semantha_sdk-6.8.0/semantha_sdk/api/tag.py
--rw-r--r--   0        0        0     1310 2024-02-02 10:09:01.183800 semantha_sdk-6.8.0/semantha_sdk/api/tag_referencedocuments.py
--rw-r--r--   0        0        0     1043 2024-02-02 10:09:01.186834 semantha_sdk-6.8.0/semantha_sdk/api/tags.py
--rw-r--r--   0        0        0     1528 2024-02-08 07:35:59.959900 semantha_sdk-6.8.0/semantha_sdk/api/transactions.py
--rw-r--r--   0        0        0     1310 2024-02-02 10:09:01.191801 semantha_sdk-6.8.0/semantha_sdk/api/validation.py
--rw-r--r--   0        0        0     6476 2024-02-02 10:08:22.147281 semantha_sdk-6.8.0/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      570 2024-02-02 10:08:21.828952 semantha_sdk-6.8.0/semantha_sdk/model/annotation_cell.py
--rw-r--r--   0        0        0      656 2024-02-02 10:08:21.833959 semantha_sdk-6.8.0/semantha_sdk/model/annotation_page.py
--rw-r--r--   0        0        0      528 2024-02-02 10:08:21.932958 semantha_sdk-6.8.0/semantha_sdk/model/answer.py
--rw-r--r--   0        0        0      508 2024-02-02 10:08:21.935959 semantha_sdk-6.8.0/semantha_sdk/model/answer_reference.py
--rw-r--r--   0        0        0      378 2024-02-02 10:08:21.801960 semantha_sdk-6.8.0/semantha_sdk/model/area.py
--rw-r--r--   0        0        0      611 2024-02-02 10:08:21.905956 semantha_sdk-6.8.0/semantha_sdk/model/argument.py
--rw-r--r--   0        0        0      853 2024-02-02 10:08:22.069280 semantha_sdk-6.8.0/semantha_sdk/model/attribute.py
--rw-r--r--   0        0        0      500 2024-02-02 10:08:22.121276 semantha_sdk-6.8.0/semantha_sdk/model/attribute_overview.py
--rw-r--r--   0        0        0      548 2024-02-02 10:08:21.763959 semantha_sdk-6.8.0/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      369 2024-02-02 10:08:21.805956 semantha_sdk-6.8.0/semantha_sdk/model/cell_type.py
--rw-r--r--   0        0        0     1005 2024-02-02 10:08:21.770971 semantha_sdk-6.8.0/semantha_sdk/model/class_bulk.py
--rw-r--r--   0        0        0      587 2024-02-02 10:08:22.075285 semantha_sdk-6.8.0/semantha_sdk/model/classes_overview.py
--rw-r--r--   0        0        0      828 2024-02-02 10:08:22.072293 semantha_sdk-6.8.0/semantha_sdk/model/clazz.py
--rw-r--r--   0        0        0      578 2024-02-02 10:08:22.014955 semantha_sdk-6.8.0/semantha_sdk/model/clustered_document.py
--rw-r--r--   0        0        0      663 2024-02-02 10:08:22.018959 semantha_sdk-6.8.0/semantha_sdk/model/clustering_response.py
--rw-r--r--   0        0        0     1217 2024-02-02 10:08:21.978952 semantha_sdk-6.8.0/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      587 2024-02-02 10:08:21.907957 semantha_sdk-6.8.0/semantha_sdk/model/condition.py
--rw-r--r--   0        0        0      533 2024-02-02 10:08:21.909951 semantha_sdk-6.8.0/semantha_sdk/model/condition_value.py
--rw-r--r--   0        0        0      464 2024-02-02 10:08:21.927953 semantha_sdk-6.8.0/semantha_sdk/model/current_user.py
--rw-r--r--   0        0        0      380 2024-02-02 10:08:21.792951 semantha_sdk-6.8.0/semantha_sdk/model/custom_field.py
--rw-r--r--   0        0        0      599 2024-02-02 10:08:21.789961 semantha_sdk-6.8.0/semantha_sdk/model/data_property.py
--rw-r--r--   0        0        0      366 2024-02-02 10:08:21.929961 semantha_sdk-6.8.0/semantha_sdk/model/difference.py
--rw-r--r--   0        0        0      492 2024-02-02 10:08:21.837968 semantha_sdk-6.8.0/semantha_sdk/model/distance.py
--rw-r--r--   0        0        0     1417 2024-02-02 10:08:21.844968 semantha_sdk-6.8.0/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1146 2024-02-02 10:08:21.939951 semantha_sdk-6.8.0/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      880 2024-02-02 10:08:21.796956 semantha_sdk-6.8.0/semantha_sdk/model/document_class_bulk.py
--rw-r--r--   0        0        0      679 2024-02-02 10:08:21.942958 semantha_sdk-6.8.0/semantha_sdk/model/document_class_node.py
--rw-r--r--   0        0        0      671 2024-02-02 10:08:22.022952 semantha_sdk-6.8.0/semantha_sdk/model/document_cluster.py
--rw-r--r--   0        0        0     1172 2024-02-02 10:08:21.946970 semantha_sdk-6.8.0/semantha_sdk/model/document_information.py
--rw-r--r--   0        0        0      456 2024-02-02 10:08:21.949949 semantha_sdk-6.8.0/semantha_sdk/model/document_meta_data.py
--rw-r--r--   0        0        0      451 2024-02-02 10:08:21.852958 semantha_sdk-6.8.0/semantha_sdk/model/document_named_entity.py
--rw-r--r--   0        0        0      472 2024-02-02 10:08:21.855960 semantha_sdk-6.8.0/semantha_sdk/model/document_table.py
--rw-r--r--   0        0        0      656 2024-02-02 10:08:21.816970 semantha_sdk-6.8.0/semantha_sdk/model/document_type.py
--rw-r--r--   0        0        0      823 2024-02-02 10:08:21.956954 semantha_sdk-6.8.0/semantha_sdk/model/document_type_change.py
--rw-r--r--   0        0        0     1189 2024-02-02 10:08:21.810957 semantha_sdk-6.8.0/semantha_sdk/model/document_type_config.py
--rw-r--r--   0        0        0      421 2024-02-02 10:08:21.959958 semantha_sdk-6.8.0/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      378 2024-02-02 10:08:21.967950 semantha_sdk-6.8.0/semantha_sdk/model/domain_info.py
--rw-r--r--   0        0        0      393 2024-02-02 10:08:21.858954 semantha_sdk-6.8.0/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      644 2024-02-02 10:08:21.913959 semantha_sdk-6.8.0/semantha_sdk/model/expression.py
--rw-r--r--   0        0        0      550 2024-02-02 10:08:21.980958 semantha_sdk-6.8.0/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      752 2024-02-02 10:08:21.983950 semantha_sdk-6.8.0/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      499 2024-02-02 10:08:21.986958 semantha_sdk-6.8.0/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      752 2024-02-02 10:08:22.089282 semantha_sdk-6.8.0/semantha_sdk/model/extractor.py
--rw-r--r--   0        0        0      770 2024-02-02 10:08:22.081282 semantha_sdk-6.8.0/semantha_sdk/model/extractor_attribute.py
--rw-r--r--   0        0        0      884 2024-02-02 10:08:22.085288 semantha_sdk-6.8.0/semantha_sdk/model/extractor_class.py
--rw-r--r--   0        0        0      681 2024-02-02 10:08:22.098297 semantha_sdk-6.8.0/semantha_sdk/model/extractor_class_overview.py
--rw-r--r--   0        0        0      905 2024-02-02 10:08:21.863956 semantha_sdk-6.8.0/semantha_sdk/model/features.py
--rw-r--r--   0        0        0      344 2024-02-02 10:08:21.916956 semantha_sdk-6.8.0/semantha_sdk/model/field.py
--rw-r--r--   0        0        0      475 2024-02-02 10:08:21.988959 semantha_sdk-6.8.0/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      461 2024-02-02 10:08:21.990951 semantha_sdk-6.8.0/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      441 2024-02-02 10:08:22.102288 semantha_sdk-6.8.0/semantha_sdk/model/formatter.py
--rw-r--r--   0        0        0      393 2024-02-02 10:08:22.062739 semantha_sdk-6.8.0/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      877 2024-02-02 10:08:21.782962 semantha_sdk-6.8.0/semantha_sdk/model/instance.py
--rw-r--r--   0        0        0      493 2024-02-02 10:08:21.778953 semantha_sdk-6.8.0/semantha_sdk/model/instance_child.py
--rw-r--r--   0        0        0      535 2024-02-02 10:08:22.105281 semantha_sdk-6.8.0/semantha_sdk/model/instance_overview.py
--rw-r--r--   0        0        0      347 2024-02-02 10:08:21.773959 semantha_sdk-6.8.0/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      371 2024-02-02 10:08:22.065276 semantha_sdk-6.8.0/semantha_sdk/model/language_detection.py
--rw-r--r--   0        0        0      462 2024-02-02 10:08:21.866960 semantha_sdk-6.8.0/semantha_sdk/model/link.py
--rw-r--r--   0        0        0      548 2024-02-02 10:08:21.992952 semantha_sdk-6.8.0/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      436 2024-02-02 10:08:21.994958 semantha_sdk-6.8.0/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      416 2024-02-02 10:08:22.092281 semantha_sdk-6.8.0/semantha_sdk/model/matcher.py
--rw-r--r--   0        0        0      564 2024-02-02 10:08:21.970951 semantha_sdk-6.8.0/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      462 2024-02-02 10:08:22.024953 semantha_sdk-6.8.0/semantha_sdk/model/meta_info_page.py
--rw-r--r--   0        0        0      356 2024-02-02 10:08:21.997973 semantha_sdk-6.8.0/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      369 2024-02-02 10:08:21.776961 semantha_sdk-6.8.0/semantha_sdk/model/metadata_value.py
--rw-r--r--   0        0        0      510 2024-02-02 10:08:21.973961 semantha_sdk-6.8.0/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1590 2024-02-02 10:08:22.001960 semantha_sdk-6.8.0/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      467 2024-02-02 10:08:21.821957 semantha_sdk-6.8.0/semantha_sdk/model/model_metadata.py
--rw-r--r--   0        0        0      328 2024-02-02 10:08:21.952956 semantha_sdk-6.8.0/semantha_sdk/model/name.py
--rw-r--r--   0        0        0      441 2024-02-02 10:08:21.824953 semantha_sdk-6.8.0/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      437 2024-02-02 10:08:22.078286 semantha_sdk-6.8.0/semantha_sdk/model/overview.py
--rw-r--r--   0        0        0      804 2024-02-02 10:08:21.875965 semantha_sdk-6.8.0/semantha_sdk/model/page.py
--rw-r--r--   0        0        0      490 2024-02-02 10:08:21.870958 semantha_sdk-6.8.0/semantha_sdk/model/page_content.py
--rw-r--r--   0        0        0     1066 2024-02-02 10:08:21.880965 semantha_sdk-6.8.0/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      439 2024-02-02 10:08:22.052777 semantha_sdk-6.8.0/semantha_sdk/model/paragraph_update.py
--rw-r--r--   0        0        0      484 2024-02-02 10:08:22.027953 semantha_sdk-6.8.0/semantha_sdk/model/plotly_chart.py
--rw-r--r--   0        0        0      540 2024-02-02 10:08:22.003955 semantha_sdk-6.8.0/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      452 2024-02-08 07:35:59.961903 semantha_sdk-6.8.0/semantha_sdk/model/range.py
--rw-r--r--   0        0        0      393 2024-02-02 10:08:21.884954 semantha_sdk-6.8.0/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      847 2024-02-02 10:08:21.889952 semantha_sdk-6.8.0/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0      700 2024-02-02 10:08:22.055983 semantha_sdk-6.8.0/semantha_sdk/model/reference_documents_response_container.py
--rw-r--r--   0        0        0      406 2024-02-02 10:08:22.107284 semantha_sdk-6.8.0/semantha_sdk/model/regex.py
--rw-r--r--   0        0        0      651 2024-02-02 10:08:22.112283 semantha_sdk-6.8.0/semantha_sdk/model/relation.py
--rw-r--r--   0        0        0      446 2024-02-02 10:08:22.110283 semantha_sdk-6.8.0/semantha_sdk/model/relation_condition.py
--rw-r--r--   0        0        0      676 2024-02-02 10:08:22.030950 semantha_sdk-6.8.0/semantha_sdk/model/response_meta_info.py
--rw-r--r--   0        0        0      462 2024-02-02 10:08:21.892988 semantha_sdk-6.8.0/semantha_sdk/model/row.py
--rw-r--r--   0        0        0      637 2024-02-02 10:08:21.919953 semantha_sdk-6.8.0/semantha_sdk/model/rule.py
--rw-r--r--   0        0        0      514 2024-02-02 10:08:22.114282 semantha_sdk-6.8.0/semantha_sdk/model/rule_function.py
--rw-r--r--   0        0        0      551 2024-02-02 10:08:22.118292 semantha_sdk-6.8.0/semantha_sdk/model/rule_overview.py
--rw-r--r--   0        0        0      865 2024-02-02 10:08:22.006954 semantha_sdk-6.8.0/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      471 2024-02-02 10:08:22.039954 semantha_sdk-6.8.0/semantha_sdk/model/semi_super_vised_document.py
--rw-r--r--   0        0        0      804 2024-02-02 10:08:21.898955 semantha_sdk-6.8.0/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0     1978 2024-02-02 10:08:21.964956 semantha_sdk-6.8.0/semantha_sdk/model/settings.py
--rw-r--r--   0        0        0      396 2024-02-02 10:08:21.785955 semantha_sdk-6.8.0/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      648 2024-02-02 10:08:22.034953 semantha_sdk-6.8.0/semantha_sdk/model/smart_cluster_response_container.py
--rw-r--r--   0        0        0      873 2024-02-02 10:08:22.042953 semantha_sdk-6.8.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
--rw-r--r--   0        0        0      451 2024-02-02 10:08:22.037959 semantha_sdk-6.8.0/semantha_sdk/model/source_document.py
--rw-r--r--   0        0        0      549 2024-02-02 10:08:22.045957 semantha_sdk-6.8.0/semantha_sdk/model/statistic.py
--rw-r--r--   0        0        0      436 2024-02-02 10:08:21.922965 semantha_sdk-6.8.0/semantha_sdk/model/stop_word.py
--rw-r--r--   0        0        0      404 2024-02-02 10:08:22.058487 semantha_sdk-6.8.0/semantha_sdk/model/summarization.py
--rw-r--r--   0        0        0      544 2024-02-02 10:08:21.925961 semantha_sdk-6.8.0/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      389 2024-02-02 10:08:21.902955 semantha_sdk-6.8.0/semantha_sdk/model/table_cell.py
--rw-r--r--   0        0        0      518 2024-02-02 10:08:22.009957 semantha_sdk-6.8.0/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      415 2024-02-02 10:08:22.048232 semantha_sdk-6.8.0/semantha_sdk/model/tag_docs.py
--rw-r--r--   0        0        0      429 2024-02-02 10:08:22.060580 semantha_sdk-6.8.0/semantha_sdk/model/transaction_summary.py
--rw-r--r--   0        0        0      417 2024-02-02 10:08:22.011953 semantha_sdk-6.8.0/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       37 2023-08-25 14:25:29.323155 semantha_sdk-6.8.0/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0    11138 2023-12-21 12:20:15.820140 semantha_sdk-6.8.0/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0     4540 2023-08-25 14:25:29.334695 semantha_sdk-6.8.0/semantha_sdk/semantha/__init__.py
--rw-r--r--   0        0        0     1741 2023-09-05 07:36:38.109289 semantha_sdk-6.8.0/semantha_sdk/semantha/compare/__init__.py
--rw-r--r--   0        0        0     1199 2023-09-05 07:36:38.111796 semantha_sdk-6.8.0/semantha_sdk/semantha/customization.py
--rw-r--r--   0        0        0     1765 2023-09-05 07:36:38.115839 semantha_sdk-6.8.0/semantha_sdk/semantha/domain/__init__.py
--rw-r--r--   0        0        0      423 2023-09-05 07:36:38.118835 semantha_sdk-6.8.0/semantha_sdk/semantha/domain/settings.py
--rw-r--r--   0        0        0      155 2023-09-05 07:36:38.122358 semantha_sdk-6.8.0/semantha_sdk/semantha/files.py
--rw-r--r--   0        0        0    10217 2023-09-05 07:36:38.125374 semantha_sdk-6.8.0/semantha_sdk/semantha/library/__init__.py
--rw-r--r--   0        0        0     3192 2023-09-05 07:36:38.129372 semantha_sdk-6.8.0/semantha_sdk/semantha/library/document.py
--rw-r--r--   0        0        0     2165 2023-09-05 07:36:38.132907 semantha_sdk-6.8.0/semantha_sdk/semantha/library/documentiter.py
--rw-r--r--   0        0        0     1210 2023-09-05 07:36:38.136721 semantha_sdk-6.8.0/semantha_sdk/semantha/library/documenttags.py
--rw-r--r--   0        0        0     1319 2023-09-05 07:36:38.140251 semantha_sdk-6.8.0/semantha_sdk/semantha/library/metadata.py
--rw-r--r--   0        0        0      799 2023-09-05 07:36:38.142780 semantha_sdk-6.8.0/semantha_sdk/semantha/library/reference.py
--rw-r--r--   0        0        0      652 2023-09-05 07:36:38.146794 semantha_sdk-6.8.0/semantha_sdk/semantha/library/tags.py
--rw-r--r--   0        0        0      393 2023-08-25 14:25:29.381114 semantha_sdk-6.8.0/semantha_sdk/semantha/ranking/__init__.py
--rw-r--r--   0        0        0      311 2023-09-05 07:36:38.149799 semantha_sdk-6.8.0/semantha_sdk/semantha/ranking/dense.py
--rw-r--r--   0        0        0      925 2023-09-05 07:36:38.154332 semantha_sdk-6.8.0/semantha_sdk/semantha/ranking/hybrid.py
--rw-r--r--   0        0        0      533 2023-09-05 07:36:38.158345 semantha_sdk-6.8.0/semantha_sdk/semantha/ranking/sparse.py
--rw-r--r--   0        0        0    24602 1970-01-01 00:00:00.000000 semantha_sdk-6.8.0/PKG-INFO
+-rw-r--r--   0        0        0     5341 2024-02-23 12:28:45.661170 semantha_sdk-6.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0    14448 2024-02-22 15:44:34.330565 semantha_sdk-6.9.0/DOCU.md
+-rw-r--r--   0        0        0    11545 2024-02-15 07:17:08.779557 semantha_sdk-6.9.0/LICENSE
+-rw-r--r--   0        0        0     1697 2024-02-23 12:29:08.215526 semantha_sdk-6.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4900 2024-02-15 07:17:08.790597 semantha_sdk-6.9.0/README.md
+-rw-r--r--   0        0        0     2671 2024-02-15 12:50:37.536314 semantha_sdk-6.9.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-15 07:17:08.875358 semantha_sdk-6.9.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0     1962 2024-02-15 12:52:34.537486 semantha_sdk-6.9.0/semantha_sdk/api/answers.py
+-rw-r--r--   0        0        0      942 2024-02-15 12:50:37.242080 semantha_sdk-6.9.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      765 2024-02-15 12:50:37.243080 semantha_sdk-6.9.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      749 2024-02-15 12:50:37.269146 semantha_sdk-6.9.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1724 2024-02-15 12:52:34.539486 semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1484 2024-02-15 12:50:37.261601 semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_documenttypes.py
+-rw-r--r--   0        0        0     1823 2024-02-15 12:50:37.245081 semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     4808 2024-02-22 10:08:57.548045 semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3139 2024-02-15 12:52:34.542483 semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1241 2024-02-15 12:52:34.544484 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      855 2024-02-15 12:50:37.275147 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1839 2024-02-15 12:52:34.545484 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1667 2024-02-15 12:52:34.548491 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2998 2024-02-15 12:50:37.271148 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      762 2024-02-15 12:50:37.270145 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1594 2024-02-15 12:52:34.550486 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1640 2024-02-15 12:52:34.551484 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1268 2024-02-15 12:52:34.552485 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1535 2024-02-15 12:52:34.554485 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_rules.py
+-rw-r--r--   0        0        0     1198 2024-02-15 12:50:37.283147 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1217 2024-02-15 12:52:34.555485 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0     1088 2024-02-15 12:52:34.556484 semantha_sdk-6.9.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0      965 2024-02-15 12:50:37.285148 semantha_sdk-6.9.0/semantha_sdk/api/celltypes.py
+-rw-r--r--   0        0        0     1188 2024-02-15 12:50:37.353223 semantha_sdk-6.9.0/semantha_sdk/api/child_extractorclasses.py
+-rw-r--r--   0        0        0     1256 2024-02-15 12:50:37.305149 semantha_sdk-6.9.0/semantha_sdk/api/clone.py
+-rw-r--r--   0        0        0     6276 2024-02-15 12:50:37.312147 semantha_sdk-6.9.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1197 2024-02-15 12:50:37.286145 semantha_sdk-6.9.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1361 2024-02-15 12:50:37.288145 semantha_sdk-6.9.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     1093 2024-02-15 12:50:37.296149 semantha_sdk-6.9.0/semantha_sdk/api/docclass_customfields.py
+-rw-r--r--   0        0        0     2217 2024-02-15 12:50:37.298147 semantha_sdk-6.9.0/semantha_sdk/api/docclass_documentclasses.py
+-rw-r--r--   0        0        0     1705 2024-02-15 12:50:37.299148 semantha_sdk-6.9.0/semantha_sdk/api/docclass_referencedocuments.py
+-rw-r--r--   0        0        0     3874 2024-02-15 12:52:34.558485 semantha_sdk-6.9.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     2505 2024-02-15 12:50:37.295147 semantha_sdk-6.9.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1969 2024-02-15 12:50:37.294149 semantha_sdk-6.9.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     9610 2024-02-15 12:52:34.559486 semantha_sdk-6.9.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     1975 2024-02-15 12:50:37.304150 semantha_sdk-6.9.0/semantha_sdk/api/documenttype.py
+-rw-r--r--   0        0        0     2041 2024-02-15 12:50:37.303146 semantha_sdk-6.9.0/semantha_sdk/api/documenttypes.py
+-rw-r--r--   0        0        0     4816 2024-02-15 12:50:37.291145 semantha_sdk-6.9.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1234 2024-02-15 12:50:37.289146 semantha_sdk-6.9.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      930 2024-02-15 12:50:37.332702 semantha_sdk-6.9.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1630 2024-02-15 12:52:34.560490 semantha_sdk-6.9.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1545 2024-02-15 12:50:37.333702 semantha_sdk-6.9.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1044 2024-02-15 12:50:37.338708 semantha_sdk-6.9.0/semantha_sdk/api/model_attributes.py
+-rw-r--r--   0        0        0      961 2024-02-15 12:50:37.339707 semantha_sdk-6.9.0/semantha_sdk/api/model_backups.py
+-rw-r--r--   0        0        0     1485 2024-02-15 12:50:37.341707 semantha_sdk-6.9.0/semantha_sdk/api/model_boostword.py
+-rw-r--r--   0        0        0     1896 2024-02-15 12:50:37.340709 semantha_sdk-6.9.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0     2060 2024-02-15 12:50:37.349217 semantha_sdk-6.9.0/semantha_sdk/api/model_dataproperties.py
+-rw-r--r--   0        0        0     1530 2024-02-15 12:50:37.349217 semantha_sdk-6.9.0/semantha_sdk/api/model_dataproperty.py
+-rw-r--r--   0        0        0      865 2024-02-15 12:50:37.334707 semantha_sdk-6.9.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     5886 2024-02-15 12:50:37.337709 semantha_sdk-6.9.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      742 2024-02-15 12:50:37.335708 semantha_sdk-6.9.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0     1861 2024-02-15 12:50:37.352224 semantha_sdk-6.9.0/semantha_sdk/api/model_extractorclass.py
+-rw-r--r--   0        0        0     2476 2024-02-15 12:50:37.351225 semantha_sdk-6.9.0/semantha_sdk/api/model_extractorclasses.py
+-rw-r--r--   0        0        0      976 2024-02-15 12:50:37.354223 semantha_sdk-6.9.0/semantha_sdk/api/model_extractors.py
+-rw-r--r--   0        0        0      880 2024-02-15 12:50:37.375224 semantha_sdk-6.9.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      994 2024-02-15 12:50:37.355224 semantha_sdk-6.9.0/semantha_sdk/api/model_formatters.py
+-rw-r--r--   0        0        0     1933 2024-02-15 12:50:37.359225 semantha_sdk-6.9.0/semantha_sdk/api/model_metadata.py
+-rw-r--r--   0        0        0      877 2024-02-15 12:50:37.376225 semantha_sdk-6.9.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1942 2024-02-15 12:50:37.360224 semantha_sdk-6.9.0/semantha_sdk/api/model_namedentities.py
+-rw-r--r--   0        0        0     1519 2024-02-15 12:50:37.362227 semantha_sdk-6.9.0/semantha_sdk/api/model_namedentity.py
+-rw-r--r--   0        0        0     1007 2024-02-15 12:50:37.363226 semantha_sdk-6.9.0/semantha_sdk/api/model_objectproperties.py
+-rw-r--r--   0        0        0     1518 2024-02-15 12:50:37.359225 semantha_sdk-6.9.0/semantha_sdk/api/model_onemetadata.py
+-rw-r--r--   0        0        0     1426 2024-02-15 12:50:37.365225 semantha_sdk-6.9.0/semantha_sdk/api/model_regex.py
+-rw-r--r--   0        0        0     1822 2024-02-15 12:50:37.364227 semantha_sdk-6.9.0/semantha_sdk/api/model_regexes.py
+-rw-r--r--   0        0        0     1469 2024-02-15 12:50:37.367225 semantha_sdk-6.9.0/semantha_sdk/api/model_relation.py
+-rw-r--r--   0        0        0     1874 2024-02-15 12:50:37.365225 semantha_sdk-6.9.0/semantha_sdk/api/model_relations.py
+-rw-r--r--   0        0        0     1413 2024-02-15 12:50:37.370224 semantha_sdk-6.9.0/semantha_sdk/api/model_rule.py
+-rw-r--r--   0        0        0     1024 2024-02-15 12:50:37.367225 semantha_sdk-6.9.0/semantha_sdk/api/model_rulefunctions.py
+-rw-r--r--   0        0        0     1934 2024-02-15 12:50:37.369224 semantha_sdk-6.9.0/semantha_sdk/api/model_rules.py
+-rw-r--r--   0        0        0     1474 2024-02-15 12:50:37.372227 semantha_sdk-6.9.0/semantha_sdk/api/model_stopword.py
+-rw-r--r--   0        0        0     1879 2024-02-15 12:50:37.371224 semantha_sdk-6.9.0/semantha_sdk/api/model_stopwords.py
+-rw-r--r--   0        0        0     1455 2024-02-15 12:50:37.375224 semantha_sdk-6.9.0/semantha_sdk/api/model_synonym.py
+-rw-r--r--   0        0        0     1854 2024-02-15 12:50:37.374227 semantha_sdk-6.9.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1242 2024-02-15 12:50:37.306148 semantha_sdk-6.9.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     5033 2024-02-22 10:08:57.549045 semantha_sdk-6.9.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1417 2024-02-15 12:50:37.346708 semantha_sdk-6.9.0/semantha_sdk/api/modelont_attribute.py
+-rw-r--r--   0        0        0     1852 2024-02-15 12:50:37.345706 semantha_sdk-6.9.0/semantha_sdk/api/modelont_attributes.py
+-rw-r--r--   0        0        0     1946 2024-02-15 12:50:37.344712 semantha_sdk-6.9.0/semantha_sdk/api/modelont_class.py
+-rw-r--r--   0        0        0     2462 2024-02-15 12:50:37.342707 semantha_sdk-6.9.0/semantha_sdk/api/modelont_classes.py
+-rw-r--r--   0        0        0     1475 2024-02-15 12:50:37.358225 semantha_sdk-6.9.0/semantha_sdk/api/modelont_instance.py
+-rw-r--r--   0        0        0     2608 2024-02-15 12:50:37.357224 semantha_sdk-6.9.0/semantha_sdk/api/modelont_instances.py
+-rw-r--r--   0        0        0     1218 2024-02-15 12:50:37.347708 semantha_sdk-6.9.0/semantha_sdk/api/modelontclass_instances.py
+-rw-r--r--   0        0        0     1753 2024-02-15 12:52:34.562488 semantha_sdk-6.9.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1780 2024-02-15 12:50:37.317701 semantha_sdk-6.9.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      718 2024-02-15 12:50:37.316706 semantha_sdk-6.9.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0     2526 2024-02-15 12:50:37.315702 semantha_sdk-6.9.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0    16643 2024-02-22 10:08:57.551386 semantha_sdk-6.9.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0    21928 2024-02-15 12:52:34.565490 semantha_sdk-6.9.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      870 2024-02-15 12:50:37.287145 semantha_sdk-6.9.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2430 2024-02-15 12:50:37.539314 semantha_sdk-6.9.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0     1019 2024-02-15 12:50:37.318705 semantha_sdk-6.9.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      712 2024-02-15 12:50:37.318705 semantha_sdk-6.9.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1643 2024-02-15 12:50:37.322703 semantha_sdk-6.9.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     4943 2024-02-15 12:52:34.566490 semantha_sdk-6.9.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4442 2024-02-15 12:52:34.567487 semantha_sdk-6.9.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0     1015 2024-02-15 12:50:37.314702 semantha_sdk-6.9.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0     1485 2024-02-15 12:50:37.326703 semantha_sdk-6.9.0/semantha_sdk/api/summarizations.py
+-rw-r--r--   0        0        0      863 2024-02-15 12:50:37.328703 semantha_sdk-6.9.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1310 2024-02-15 12:50:37.329701 semantha_sdk-6.9.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0     1043 2024-02-15 12:50:37.327704 semantha_sdk-6.9.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1528 2024-02-15 12:50:37.330702 semantha_sdk-6.9.0/semantha_sdk/api/transactions.py
+-rw-r--r--   0        0        0     1265 2024-02-15 12:52:34.569485 semantha_sdk-6.9.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     6476 2024-02-15 12:50:37.518305 semantha_sdk-6.9.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      570 2024-02-15 12:50:37.443233 semantha_sdk-6.9.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      656 2024-02-15 12:50:37.444232 semantha_sdk-6.9.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      528 2024-02-15 12:50:37.464304 semantha_sdk-6.9.0/semantha_sdk/model/answer.py
+-rw-r--r--   0        0        0      508 2024-02-15 12:50:37.465305 semantha_sdk-6.9.0/semantha_sdk/model/answer_reference.py
+-rw-r--r--   0        0        0      378 2024-02-15 12:50:37.437234 semantha_sdk-6.9.0/semantha_sdk/model/area.py
+-rw-r--r--   0        0        0      611 2024-02-15 12:50:37.458305 semantha_sdk-6.9.0/semantha_sdk/model/argument.py
+-rw-r--r--   0        0        0      853 2024-02-15 12:50:37.500303 semantha_sdk-6.9.0/semantha_sdk/model/attribute.py
+-rw-r--r--   0        0        0      500 2024-02-15 12:50:37.512308 semantha_sdk-6.9.0/semantha_sdk/model/attribute_overview.py
+-rw-r--r--   0        0        0      548 2024-02-15 12:50:37.428223 semantha_sdk-6.9.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      369 2024-02-15 12:50:37.438235 semantha_sdk-6.9.0/semantha_sdk/model/cell_type.py
+-rw-r--r--   0        0        0     1005 2024-02-15 12:50:37.430225 semantha_sdk-6.9.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      587 2024-02-15 12:50:37.501307 semantha_sdk-6.9.0/semantha_sdk/model/classes_overview.py
+-rw-r--r--   0        0        0      828 2024-02-15 12:50:37.501307 semantha_sdk-6.9.0/semantha_sdk/model/clazz.py
+-rw-r--r--   0        0        0      578 2024-02-15 12:50:37.487306 semantha_sdk-6.9.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      663 2024-02-15 12:50:37.488307 semantha_sdk-6.9.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0     1217 2024-02-15 12:50:37.477306 semantha_sdk-6.9.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      587 2024-02-15 12:50:37.459305 semantha_sdk-6.9.0/semantha_sdk/model/condition.py
+-rw-r--r--   0        0        0      533 2024-02-15 12:50:37.459305 semantha_sdk-6.9.0/semantha_sdk/model/condition_value.py
+-rw-r--r--   0        0        0      464 2024-02-15 12:50:37.463303 semantha_sdk-6.9.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      380 2024-02-15 12:50:37.436232 semantha_sdk-6.9.0/semantha_sdk/model/custom_field.py
+-rw-r--r--   0        0        0      599 2024-02-15 12:50:37.435232 semantha_sdk-6.9.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      366 2024-02-15 12:50:37.464304 semantha_sdk-6.9.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      492 2024-02-15 12:50:37.445233 semantha_sdk-6.9.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1417 2024-02-15 12:50:37.446231 semantha_sdk-6.9.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0     1146 2024-02-15 12:50:37.466303 semantha_sdk-6.9.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      880 2024-02-15 12:50:37.437234 semantha_sdk-6.9.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      679 2024-02-15 12:50:37.467307 semantha_sdk-6.9.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      671 2024-02-15 12:50:37.489304 semantha_sdk-6.9.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1172 2024-02-15 12:50:37.468304 semantha_sdk-6.9.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      456 2024-02-15 12:50:37.469306 semantha_sdk-6.9.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      451 2024-02-15 12:50:37.448229 semantha_sdk-6.9.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      472 2024-02-15 12:50:37.449232 semantha_sdk-6.9.0/semantha_sdk/model/document_table.py
+-rw-r--r--   0        0        0      656 2024-02-15 12:50:37.441232 semantha_sdk-6.9.0/semantha_sdk/model/document_type.py
+-rw-r--r--   0        0        0      823 2024-02-15 12:50:37.471303 semantha_sdk-6.9.0/semantha_sdk/model/document_type_change.py
+-rw-r--r--   0        0        0     1189 2024-02-15 12:50:37.439232 semantha_sdk-6.9.0/semantha_sdk/model/document_type_config.py
+-rw-r--r--   0        0        0      421 2024-02-15 12:50:37.471303 semantha_sdk-6.9.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      378 2024-02-15 12:50:37.474304 semantha_sdk-6.9.0/semantha_sdk/model/domain_info.py
+-rw-r--r--   0        0        0      393 2024-02-15 12:50:37.449232 semantha_sdk-6.9.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      644 2024-02-15 12:50:37.460305 semantha_sdk-6.9.0/semantha_sdk/model/expression.py
+-rw-r--r--   0        0        0      550 2024-02-15 12:50:37.478307 semantha_sdk-6.9.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      752 2024-02-15 12:50:37.479306 semantha_sdk-6.9.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      499 2024-02-15 12:50:37.479306 semantha_sdk-6.9.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      752 2024-02-15 12:50:37.504305 semantha_sdk-6.9.0/semantha_sdk/model/extractor.py
+-rw-r--r--   0        0        0      770 2024-02-15 12:50:37.502307 semantha_sdk-6.9.0/semantha_sdk/model/extractor_attribute.py
+-rw-r--r--   0        0        0      884 2024-02-15 12:50:37.503306 semantha_sdk-6.9.0/semantha_sdk/model/extractor_class.py
+-rw-r--r--   0        0        0      681 2024-02-15 12:50:37.507304 semantha_sdk-6.9.0/semantha_sdk/model/extractor_class_overview.py
+-rw-r--r--   0        0        0      905 2024-02-15 12:50:37.450303 semantha_sdk-6.9.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      344 2024-02-15 12:50:37.461306 semantha_sdk-6.9.0/semantha_sdk/model/field.py
+-rw-r--r--   0        0        0      475 2024-02-15 12:50:37.480304 semantha_sdk-6.9.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      461 2024-02-15 12:50:37.481305 semantha_sdk-6.9.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      441 2024-02-15 12:50:37.508305 semantha_sdk-6.9.0/semantha_sdk/model/formatter.py
+-rw-r--r--   0        0        0      393 2024-02-15 12:50:37.498308 semantha_sdk-6.9.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      877 2024-02-15 12:50:37.434225 semantha_sdk-6.9.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      493 2024-02-15 12:50:37.433223 semantha_sdk-6.9.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      535 2024-02-15 12:50:37.508305 semantha_sdk-6.9.0/semantha_sdk/model/instance_overview.py
+-rw-r--r--   0        0        0      347 2024-02-15 12:50:37.431225 semantha_sdk-6.9.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      371 2024-02-15 12:50:37.499307 semantha_sdk-6.9.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      462 2024-02-15 12:50:37.451304 semantha_sdk-6.9.0/semantha_sdk/model/link.py
+-rw-r--r--   0        0        0      548 2024-02-15 12:50:37.481305 semantha_sdk-6.9.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      436 2024-02-15 12:50:37.482304 semantha_sdk-6.9.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      416 2024-02-15 12:50:37.505307 semantha_sdk-6.9.0/semantha_sdk/model/matcher.py
+-rw-r--r--   0        0        0      564 2024-02-15 12:50:37.475305 semantha_sdk-6.9.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      462 2024-02-15 12:50:37.489304 semantha_sdk-6.9.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      356 2024-02-15 12:50:37.483305 semantha_sdk-6.9.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      369 2024-02-15 12:50:37.432225 semantha_sdk-6.9.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      510 2024-02-15 12:50:37.476303 semantha_sdk-6.9.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1590 2024-02-15 12:50:37.484303 semantha_sdk-6.9.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      467 2024-02-15 12:50:37.442231 semantha_sdk-6.9.0/semantha_sdk/model/model_metadata.py
+-rw-r--r--   0        0        0      328 2024-02-15 12:50:37.469306 semantha_sdk-6.9.0/semantha_sdk/model/name.py
+-rw-r--r--   0        0        0      441 2024-02-15 12:50:37.443233 semantha_sdk-6.9.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      437 2024-02-15 12:50:37.502307 semantha_sdk-6.9.0/semantha_sdk/model/overview.py
+-rw-r--r--   0        0        0      804 2024-02-15 12:50:37.453306 semantha_sdk-6.9.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      490 2024-02-15 12:50:37.452307 semantha_sdk-6.9.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0     1066 2024-02-15 12:50:37.453306 semantha_sdk-6.9.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      439 2024-02-15 12:50:37.496307 semantha_sdk-6.9.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      484 2024-02-15 12:50:37.490304 semantha_sdk-6.9.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      540 2024-02-15 12:50:37.484303 semantha_sdk-6.9.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      452 2024-02-15 12:50:37.506304 semantha_sdk-6.9.0/semantha_sdk/model/range.py
+-rw-r--r--   0        0        0      393 2024-02-15 12:50:37.454307 semantha_sdk-6.9.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      847 2024-02-15 12:50:37.455306 semantha_sdk-6.9.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      700 2024-02-15 12:50:37.497306 semantha_sdk-6.9.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      406 2024-02-15 12:50:37.509308 semantha_sdk-6.9.0/semantha_sdk/model/regex.py
+-rw-r--r--   0        0        0      651 2024-02-15 12:50:37.510306 semantha_sdk-6.9.0/semantha_sdk/model/relation.py
+-rw-r--r--   0        0        0      446 2024-02-15 12:50:37.509308 semantha_sdk-6.9.0/semantha_sdk/model/relation_condition.py
+-rw-r--r--   0        0        0      676 2024-02-15 12:50:37.491304 semantha_sdk-6.9.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      462 2024-02-15 12:50:37.456304 semantha_sdk-6.9.0/semantha_sdk/model/row.py
+-rw-r--r--   0        0        0      637 2024-02-15 12:50:37.462305 semantha_sdk-6.9.0/semantha_sdk/model/rule.py
+-rw-r--r--   0        0        0      514 2024-02-15 12:50:37.511305 semantha_sdk-6.9.0/semantha_sdk/model/rule_function.py
+-rw-r--r--   0        0        0      551 2024-02-15 12:50:37.512308 semantha_sdk-6.9.0/semantha_sdk/model/rule_overview.py
+-rw-r--r--   0        0        0      865 2024-02-15 12:50:37.485304 semantha_sdk-6.9.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      471 2024-02-15 12:50:37.493306 semantha_sdk-6.9.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      804 2024-02-15 12:50:37.457308 semantha_sdk-6.9.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1978 2024-02-15 12:50:37.473305 semantha_sdk-6.9.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      396 2024-02-15 12:50:37.434225 semantha_sdk-6.9.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      648 2024-02-15 12:50:37.492307 semantha_sdk-6.9.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      873 2024-02-15 12:50:37.494304 semantha_sdk-6.9.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      451 2024-02-15 12:50:37.492307 semantha_sdk-6.9.0/semantha_sdk/model/source_document.py
+-rw-r--r--   0        0        0      549 2024-02-15 12:50:37.495307 semantha_sdk-6.9.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      436 2024-02-15 12:50:37.462305 semantha_sdk-6.9.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      404 2024-02-15 12:50:37.497306 semantha_sdk-6.9.0/semantha_sdk/model/summarization.py
+-rw-r--r--   0        0        0      544 2024-02-15 12:50:37.463303 semantha_sdk-6.9.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      389 2024-02-15 12:50:37.458305 semantha_sdk-6.9.0/semantha_sdk/model/table_cell.py
+-rw-r--r--   0        0        0      518 2024-02-15 12:50:37.486304 semantha_sdk-6.9.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      415 2024-02-15 12:50:37.495307 semantha_sdk-6.9.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      429 2024-02-15 12:50:37.498308 semantha_sdk-6.9.0/semantha_sdk/model/transaction_summary.py
+-rw-r--r--   0        0        0      417 2024-02-15 12:50:37.486304 semantha_sdk-6.9.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       37 2024-02-15 07:17:10.205537 semantha_sdk-6.9.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0    11138 2024-02-15 07:17:10.216993 semantha_sdk-6.9.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0     4540 2024-02-15 07:17:10.219714 semantha_sdk-6.9.0/semantha_sdk/semantha/__init__.py
+-rw-r--r--   0        0        0     1741 2024-02-15 07:17:10.222581 semantha_sdk-6.9.0/semantha_sdk/semantha/compare/__init__.py
+-rw-r--r--   0        0        0     1199 2024-02-15 07:17:10.225256 semantha_sdk-6.9.0/semantha_sdk/semantha/customization.py
+-rw-r--r--   0        0        0     1765 2024-02-15 07:17:10.227908 semantha_sdk-6.9.0/semantha_sdk/semantha/domain/__init__.py
+-rw-r--r--   0        0        0      423 2024-02-15 07:17:10.231318 semantha_sdk-6.9.0/semantha_sdk/semantha/domain/settings.py
+-rw-r--r--   0        0        0      155 2024-02-15 07:17:10.234064 semantha_sdk-6.9.0/semantha_sdk/semantha/files.py
+-rw-r--r--   0        0        0    10217 2024-02-15 07:17:10.236771 semantha_sdk-6.9.0/semantha_sdk/semantha/library/__init__.py
+-rw-r--r--   0        0        0     3192 2024-02-15 07:17:10.240060 semantha_sdk-6.9.0/semantha_sdk/semantha/library/document.py
+-rw-r--r--   0        0        0     2165 2024-02-15 07:17:10.242820 semantha_sdk-6.9.0/semantha_sdk/semantha/library/documentiter.py
+-rw-r--r--   0        0        0     1210 2024-02-15 07:17:10.244394 semantha_sdk-6.9.0/semantha_sdk/semantha/library/documenttags.py
+-rw-r--r--   0        0        0     1319 2024-02-15 07:17:10.247190 semantha_sdk-6.9.0/semantha_sdk/semantha/library/metadata.py
+-rw-r--r--   0        0        0      799 2024-02-15 07:17:10.249912 semantha_sdk-6.9.0/semantha_sdk/semantha/library/reference.py
+-rw-r--r--   0        0        0      652 2024-02-15 07:17:10.252642 semantha_sdk-6.9.0/semantha_sdk/semantha/library/tags.py
+-rw-r--r--   0        0        0      393 2024-02-15 07:17:10.255365 semantha_sdk-6.9.0/semantha_sdk/semantha/ranking/__init__.py
+-rw-r--r--   0        0        0      311 2024-02-15 07:17:10.257893 semantha_sdk-6.9.0/semantha_sdk/semantha/ranking/dense.py
+-rw-r--r--   0        0        0      925 2024-02-15 07:17:10.260181 semantha_sdk-6.9.0/semantha_sdk/semantha/ranking/hybrid.py
+-rw-r--r--   0        0        0      533 2024-02-15 07:17:10.262320 semantha_sdk-6.9.0/semantha_sdk/semantha/ranking/sparse.py
+-rw-r--r--   0        0        0    25163 1970-01-01 00:00:00.000000 semantha_sdk-6.9.0/PKG-INFO
```

### Comparing `semantha_sdk-6.8.0/CHANGELOG.md` & `semantha_sdk-6.9.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog for the Python SDK for the semantha platform
 
+## [6.9.0] 2024-02-23
+### Added
+Added implementation method "post_json" for "overloaded" services where we have content type multipart/form-data as well as application/json: 
+ - **/bulk/domains/{domainname}/referencedocuments** **POST**
+ - **/domains/{domainname}/modelinstances** **POST**
+ - **/domains/{domainname}/referencedocuments** **POST**
+ - **/domains/{domainname}/similaritymatrix/cluster** **POST**
+
+
 ## [6.8.0] 2024-02-09
 ### Removed
 - Removed two setting values: similarity_matcher and similarity_threshold for endpoint: **/domains/{domainname}/settings** **GET**
 
 ### Improved
 - More method and parameter comments
 - Endpoint **/domains** **GET** returns DomainInfo object now instead of Domain
```

### Comparing `semantha_sdk-6.8.0/DOCU.md` & `semantha_sdk-6.9.0/DOCU.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/documenttypes** -> BulkdomainsDocumenttypesEndpoint
     - [x] **GET** -> List[DocumentType]
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
+    - [x] **POST** -> None
     - [x] **DELETE** -> None
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
 - [x] **/bulk/model/domains** -> BulkmodelDomainsEndpoint
 - [x] **/bulk/model/domains/{domainname}** -> BulkmodelDomainEndpoint
 - [x] **/bulk/model/domains/{domainname}/boostwords** -> BulkmodelBoostwordsEndpoint
@@ -97,19 +98,21 @@
     - [x] **PATCH** -> DocumentType
 - [x] **/domains/{domainname}/documenttypes/{id}/clone** -> CloneEndpoint
     - [x] **POST** -> DocumentType
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
+    - [x] **POST** -> SemanticModel
     - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
     - [x] **GET** (Accept: xlsx) -> IOBase
     - [x] **POST** -> List[DocumentInformation]
+    - [x] **POST** -> List[DocumentInformation]
     - [x] **DELETE** -> None
     - [x] **PATCH** -> None
 - [x] **/domains/{domainname}/referencedocuments/clusters** -> ClustersEndpoint
     - [x] **GET** -> SmartClusterResponseContainer
     - [x] **PUT** -> SmartClusterResponseContainer
 - [x] **/domains/{domainname}/referencedocuments/namedentities** -> NamedentitiesEndpoint
     - [x] **GET** -> List[DocumentNamedEntity]
@@ -135,14 +138,15 @@
 - [x] **/domains/{domainname}/settings** -> SettingsEndpoint
     - [x] **GET** -> Settings
     - [x] **PATCH** -> Settings
 - [x] **/domains/{domainname}/similaritymatrix** -> SimilaritymatrixEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/similaritymatrix/cluster** -> SimilaritymatrixClusterEndpoint
     - [x] **POST** -> List[MatrixRow]
+    - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/summarizations** -> SummarizationsEndpoint
     - [x] **POST** -> Summarization
 - [x] **/domains/{domainname}/tags** -> TagsEndpoint
     - [x] **GET** -> List[str]
 - [x] **/domains/{domainname}/tags/{tagname}** -> TagEndpoint
 - [x] **/domains/{domainname}/tags/{tagname}/referencedocuments** -> TagReferencedocumentsEndpoint
     - [x] **GET** -> List[DocumentInformation]
```

### Comparing `semantha_sdk-6.8.0/LICENSE` & `semantha_sdk-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/pyproject.toml` & `semantha_sdk-6.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "6.8.0"
+version = "6.9.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
```

### Comparing `semantha_sdk-6.8.0/README.md` & `semantha_sdk-6.9.0/README.md`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/__init__.py` & `semantha_sdk-6.9.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/answers.py` & `semantha_sdk-6.9.0/semantha_sdk/api/answers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from semantha_sdk.model.answer import Answer
-from semantha_sdk.model.answer import AnswerSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-
-class AnswersEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/answers"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post(
-        self,
-        question: str = None,
-        maxreferences: int = None,
-        similaritythreshold: float = None,
-        language: str = None,
-    ) -> Answer:
-        """
+from semantha_sdk.model.answer import Answer
+from semantha_sdk.model.answer import AnswerSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+
+class AnswersEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/answers"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        question: str = None,
+        maxreferences: int = None,
+        similaritythreshold: float = None,
+        language: str = None,
+    ) -> Answer:
+        """
         Finds references in library for a given question and uses references to generate an answer.
-            The 'maxReferences' parameter determines how many library items are used. The language of the answer can be changed via the 'language' parameter.
-        Args:
-        question (str): The text to find in the library.
-    maxreferences (int): Maximum number of returned results.
+            The 'maxReferences' parameter determines how many library items are used. The language of the answer can be changed via the 'language' parameter.
+        Args:
+        question (str): The text to find in the library.
+    maxreferences (int): Maximum number of returned results.
     similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-            In general, the higher the threshold, the more precise the results.
-    language (str): The language for the answer text.
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "question": question,
-                "maxreferences": maxreferences,
-                "similaritythreshold": similaritythreshold,
-                "language": language,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(AnswerSchema)
-
-    
-    
+            In general, the higher the threshold, the more precise the results.
+    language (str): The language for the answer text.
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "question": question,
+                "maxreferences": maxreferences,
+                "similaritythreshold": similaritythreshold,
+                "language": language,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(AnswerSchema)
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulk.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulk_domains.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulk_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulk_model.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulk_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_documentclasses.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_boostwords.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,69 @@
-from semantha_sdk.model.document_class_bulk import DocumentClassBulk
-from semantha_sdk.model.document_class_bulk import DocumentClassBulkSchema
+from semantha_sdk.api.model_boostword import ModelBoostwordEndpoint
+from semantha_sdk.model.boost_word import BoostWord
+from semantha_sdk.model.boost_word import BoostWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkdomainsDocumentclassesEndpoint(RestEndpoint):
+class ModelBoostwordsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/documentclasses"
+        return self._parent_endpoint + "/boostwords"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelBoostwordEndpoint:
+        return ModelBoostwordEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> List[DocumentClassBulk]:
+    ) -> List[BoostWord]:
         """
-        Get all document classes
-            This is the quiet version of  'get /api/domains/{domainname}/documentclasses'
+        Get all boostwords
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DocumentClassBulkSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(BoostWordSchema)
 
     def post(
         self,
-        body: List[DocumentClassBulk] = None,
-    ) -> None:
+        body: BoostWord = None,
+    ) -> BoostWord:
         """
-        Create one or more document classes
-            This is the quiet version of  'post /api/domains/{domainname}/documentclasses'
+        Create a boostword
         Args:
-        body (List[DocumentClassBulk]): 
+        body (BoostWord): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=DocumentClassBulkSchema().dump(body, many=True),
+            json=BoostWordSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.as_none()
+        return response.to(BoostWordSchema)
 
     
-    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete all boostwords
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_documenttypes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_documenttypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_domain.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_referencedocuments.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_referencedocuments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,131 @@
-from io import IOBase
-from semantha_sdk.model.document import Document
-from semantha_sdk.model.document import DocumentSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class BulkdomainsReferencedocumentsEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/referencedocuments"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    def get(
-        self,
-        withsentences: bool = None,
-    ) -> List[Document]:
-        """
+from io import IOBase
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkdomainsReferencedocumentsEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/referencedocuments"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def get(
+        self,
+        withsentences: bool = None,
+    ) -> List[Document]:
+        """
         Get all reference documents
-            This is the quiet version of  'get /api/domains/{domainname}/referencedocuments'
-        Args:
-        withsentences bool: 
-        """
-        q_params = {}
-        if withsentences is not None:
-            q_params["withsentences"] = withsentences
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DocumentSchema)
-
-    def post(
-        self,
-        name: str = None,
-        tags: str = None,
-        metadata: str = None,
-        file: IOBase = None,
-        text: str = None,
-        documenttype: str = None,
-        color: str = None,
-        comment: str = None,
-        documentclassid: str = None,
-        addparagraphsasdocuments: bool = None,
-        detectlanguage: bool = None,
-        linkclasses: bool = None,
-    ) -> None:
-        """
+            This is the quiet version of  'get /api/domains/{domainname}/referencedocuments'
+        Args:
+        withsentences bool: 
+        """
+        q_params = {}
+        if withsentences is not None:
+            q_params["withsentences"] = withsentences
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DocumentSchema)
+
+    def post(
+        self,
+        name: str = None,
+        tags: str = None,
+        metadata: str = None,
+        file: IOBase = None,
+        text: str = None,
+        documenttype: str = None,
+        color: str = None,
+        comment: str = None,
+        documentclassid: str = None,
+        addparagraphsasdocuments: bool = None,
+        detectlanguage: bool = None,
+        linkclasses: bool = None,
+    ) -> None:
+        """
         Upload reference document
-            This is the quiet version of  'post /api/domains/{domainname}/referencedocuments'
-        Args:
-        name (str): The document name in your library (in contrast to the file name being used during upload).
-    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    metadata (str): Filter by metadata
-    file (IOBase): Input document (left document).
-    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
-    comment (str): Use this parameter to add a comment to your reference document.
-    documentclassid (str): List of documentclass ID for the target. The limit here is 1 ID.
-    addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
-        """
-        q_params = {}
-        if detectlanguage is not None:
-            q_params["detectlanguage"] = detectlanguage
-        if linkclasses is not None:
-            q_params["linkclasses"] = linkclasses
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "name": name,
-                "tags": tags,
-                "metadata": metadata,
-                "file": file,
-                "text": text,
-                "documenttype": documenttype,
-                "color": color,
-                "comment": comment,
-                "documentclassid": documentclassid,
-                "addparagraphsasdocuments": addparagraphsasdocuments,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
-
-    
-    def delete(
-        self,
-        body: List[str],
-    ) -> None:
-        """
-        
-        """
-        self._session.delete(
-            url=self._endpoint,
-            json=body
-        ).execute()
-
+            This is the quiet version of  'post /api/domains/{domainname}/referencedocuments'
+        Args:
+        name (str): The document name in your library (in contrast to the file name being used during upload).
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    metadata (str): Filter by metadata
+    file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
+    comment (str): Use this parameter to add a comment to your reference document.
+    documentclassid (str): List of documentclass ID for the target. The limit here is 1 ID.
+    addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
+        """
+        q_params = {}
+        if detectlanguage is not None:
+            q_params["detectlanguage"] = detectlanguage
+        if linkclasses is not None:
+            q_params["linkclasses"] = linkclasses
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "name": name,
+                "tags": tags,
+                "metadata": metadata,
+                "file": file,
+                "text": text,
+                "documenttype": documenttype,
+                "color": color,
+                "comment": comment,
+                "documentclassid": documentclassid,
+                "addparagraphsasdocuments": addparagraphsasdocuments,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+    def post_json(
+        self,
+        body: List[Document] = None,
+        detectlanguage: bool = None,
+        linkclasses: bool = None,
+    ) -> None:
+        """
+        Upload reference document
+            This is the quiet version of  'post /api/domains/{domainname}/referencedocuments'
+        Args:
+        body (List[Document]): 
+        """
+        q_params = {}
+        if detectlanguage is not None:
+            q_params["detectlanguage"] = detectlanguage
+        if linkclasses is not None:
+            q_params["linkclasses"] = linkclasses
+        response = self._session.post(
+            url=self._endpoint,
+            json=DocumentSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+    def delete(
+        self,
+        body: List[str],
+    ) -> None:
+        """
+        
+        """
+        self._session.delete(
+            url=self._endpoint,
+            json=body
+        ).execute()
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkdomains_references.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkdomains_references.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-from semantha_sdk.model.document import Document
-from semantha_sdk.model.document import DocumentSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class BulkdomainsReferencesEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/references"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post(
-        self,
-        body: List[Document] = None,
-        referencedocumentids: str = None,
-        tags: str = None,
-        documentclassids: str = None,
-        similaritythreshold: float = None,
-        synonymousthreshold: float = None,
-        marknomatch: bool = None,
-        withreferencetext: bool = None,
-        withareas: bool = None,
-        mode: str = None,
-        detectlanguage: bool = None,
-        maxreferences: int = None,
-        considertexttype: bool = None,
-        resizeparagraphs: bool = None,
-    ) -> List[Document]:
-        """
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkdomainsReferencesEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/references"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        body: List[Document] = None,
+        referencedocumentids: str = None,
+        tags: str = None,
+        documentclassids: str = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+        withareas: bool = None,
+        mode: str = None,
+        detectlanguage: bool = None,
+        maxreferences: int = None,
+        considertexttype: bool = None,
+        resizeparagraphs: bool = None,
+    ) -> List[Document]:
+        """
         Determine references with several input documents
-            Matches several input documents ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
-        Args:
-        body (List[Document]): 
-        """
-        q_params = {}
-        if referencedocumentids is not None:
-            q_params["referencedocumentids"] = referencedocumentids
-        if tags is not None:
-            q_params["tags"] = tags
-        if documentclassids is not None:
-            q_params["documentclassids"] = documentclassids
-        if similaritythreshold is not None:
-            q_params["similaritythreshold"] = similaritythreshold
-        if synonymousthreshold is not None:
-            q_params["synonymousthreshold"] = synonymousthreshold
-        if marknomatch is not None:
-            q_params["marknomatch"] = marknomatch
-        if withreferencetext is not None:
-            q_params["withreferencetext"] = withreferencetext
-        if withareas is not None:
-            q_params["withareas"] = withareas
-        if mode is not None:
-            q_params["mode"] = mode
-        if detectlanguage is not None:
-            q_params["detectlanguage"] = detectlanguage
-        if maxreferences is not None:
-            q_params["maxreferences"] = maxreferences
-        if considertexttype is not None:
-            q_params["considertexttype"] = considertexttype
-        if resizeparagraphs is not None:
-            q_params["resizeparagraphs"] = resizeparagraphs
-        response = self._session.post(
-            url=self._endpoint,
-            json=DocumentSchema().dump(body, many=True),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(DocumentSchema)
-
-    
-    
+            Matches several input documents ('file' parameter, as an alternative 'text' can be used) to a set of 'referencedocument' if set or internal library. If you match against internal library the 'tags' parameter can be used to filter the library.
+        Args:
+        body (List[Document]): 
+        """
+        q_params = {}
+        if referencedocumentids is not None:
+            q_params["referencedocumentids"] = referencedocumentids
+        if tags is not None:
+            q_params["tags"] = tags
+        if documentclassids is not None:
+            q_params["documentclassids"] = documentclassids
+        if similaritythreshold is not None:
+            q_params["similaritythreshold"] = similaritythreshold
+        if synonymousthreshold is not None:
+            q_params["synonymousthreshold"] = synonymousthreshold
+        if marknomatch is not None:
+            q_params["marknomatch"] = marknomatch
+        if withreferencetext is not None:
+            q_params["withreferencetext"] = withreferencetext
+        if withareas is not None:
+            q_params["withareas"] = withareas
+        if mode is not None:
+            q_params["mode"] = mode
+        if detectlanguage is not None:
+            q_params["detectlanguage"] = detectlanguage
+        if maxreferences is not None:
+            q_params["maxreferences"] = maxreferences
+        if considertexttype is not None:
+            q_params["considertexttype"] = considertexttype
+        if resizeparagraphs is not None:
+            q_params["resizeparagraphs"] = resizeparagraphs
+        response = self._session.post(
+            url=self._endpoint,
+            json=DocumentSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(DocumentSchema)
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_boostwords.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_datatypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-from semantha_sdk.model.boost_word import BoostWord
-from semantha_sdk.model.boost_word import BoostWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkmodelBoostwordsEndpoint(RestEndpoint):
+class ModelDatatypesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/boostwords"
+        return self._parent_endpoint + "/datatypes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
-    
-    def post(
+    def get(
         self,
-        body: List[BoostWord] = None,
-    ) -> None:
+    ) -> List[str]:
         """
-        Create one or more boostwords
-            This is the quiet version of  'post /api/domains/{domainname}/boostwords'
+        Get all datatypes
         Args:
-        body (List[BoostWord]): 
-        """
+            """
         q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=BoostWordSchema().dump(body, many=True),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
 
     
     
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_class.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_classes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_classes.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from semantha_sdk.api.bulkmodel_class import BulkmodelClassEndpoint
-from semantha_sdk.model.class_bulk import ClassBulk
-from semantha_sdk.model.class_bulk import ClassBulkSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class BulkmodelClassesEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/classes"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-    def __call__(
-            self,
-            classid: str,
-    ) -> BulkmodelClassEndpoint:
-        return BulkmodelClassEndpoint(self._session, self._endpoint, classid)
-
-    def get(
-        self,
-    ) -> List[ClassBulk]:
-        """
+from semantha_sdk.api.bulkmodel_class import BulkmodelClassEndpoint
+from semantha_sdk.model.class_bulk import ClassBulk
+from semantha_sdk.model.class_bulk import ClassBulkSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkmodelClassesEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/classes"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+    def __call__(
+            self,
+            classid: str,
+    ) -> BulkmodelClassEndpoint:
+        return BulkmodelClassEndpoint(self._session, self._endpoint, classid)
+
+    def get(
+        self,
+    ) -> List[ClassBulk]:
+        """
         Get all classes
-            This is the quiet version of  'get /api/domains/{domainname}/classes'
-        Args:
-            """
-        q_params = {}
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ClassBulkSchema)
-
-    def post(
-        self,
-        body: List[ClassBulk] = None,
-    ) -> None:
-        """
+            This is the quiet version of  'get /api/domains/{domainname}/classes'
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ClassBulkSchema)
+
+    def post(
+        self,
+        body: List[ClassBulk] = None,
+    ) -> None:
+        """
         Create one or more classes
-            This is the quiet version of  'post /api/domains/{domainname}/classes'
-        Args:
-        body (List[ClassBulk]): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=ClassBulkSchema().dump(body, many=True),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
-
-    
-    
+            This is the quiet version of  'post /api/domains/{domainname}/classes'
+        Args:
+        body (List[ClassBulk]): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=ClassBulkSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_dataproperties.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_stopwords.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,43 @@
-from semantha_sdk.model.data_property import DataProperty
-from semantha_sdk.model.data_property import DataPropertySchema
+from semantha_sdk.model.stop_word import StopWord
+from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkmodelDatapropertiesEndpoint(RestEndpoint):
+class BulkmodelStopwordsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/dataproperties"
+        return self._parent_endpoint + "/stopwords"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
-    def get(
-        self,
-    ) -> List[DataProperty]:
-        """
-        Get all dataproperties
-            This is the quiet version of  'get /api/domains/{domainname}/dataproperties'
-        Args:
-            """
-        q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DataPropertySchema)
-
     def post(
         self,
-        body: List[DataProperty] = None,
+        body: List[StopWord] = None,
     ) -> None:
         """
-        Create one or more dataproperties
-            This is the quiet version of  'post /api/domains/{domainname}/dataproperties'
+        Add a list of stop words to your domain
         Args:
-        body (List[DataProperty]): 
+        body (List[StopWord]): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=DataPropertySchema().dump(body, many=True),
+            json=StopWordSchema().dump(body, many=True),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_domain.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_domains.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_instances.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_regexes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,69 @@
-from semantha_sdk.model.instance import Instance
-from semantha_sdk.model.instance import InstanceSchema
+from semantha_sdk.api.model_regex import ModelRegexEndpoint
+from semantha_sdk.model.regex import Regex
+from semantha_sdk.model.regex import RegexSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkmodelInstancesEndpoint(RestEndpoint):
+class ModelRegexesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/instances"
+        return self._parent_endpoint + "/regexes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelRegexEndpoint:
+        return ModelRegexEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> List[Instance]:
+    ) -> List[Regex]:
         """
-        Get all instances
-            This is the quiet version of  'get /api/domains/{domainname}/instances'
+        Get all regexes
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(RegexSchema)
 
     def post(
         self,
-        body: List[Instance] = None,
-    ) -> None:
+        body: Regex = None,
+    ) -> Regex:
         """
-        Create an instance
-            This is the quiet version of 'post /api/model/domains/{domainname}/instances'
+        Create a new regex
         Args:
-        body (List[Instance]): 
+        body (Regex): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=InstanceSchema().dump(body, many=True),
+            json=RegexSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.as_none()
+        return response.to(RegexSchema)
 
     
-    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete all regexes
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_metadata.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_metadata.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from semantha_sdk.model.model_metadata import ModelMetadata
-from semantha_sdk.model.model_metadata import ModelMetadataSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class BulkmodelMetadataEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/metadata"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    def get(
-        self,
-    ) -> List[ModelMetadata]:
-        """
+from semantha_sdk.model.model_metadata import ModelMetadata
+from semantha_sdk.model.model_metadata import ModelMetadataSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkmodelMetadataEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/metadata"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def get(
+        self,
+    ) -> List[ModelMetadata]:
+        """
         Get all metadata
-            This is the quiet version of  'get /api/domains/{domainname}/metadata'
-        Args:
-            """
-        q_params = {}
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ModelMetadataSchema)
-
-    def post(
-        self,
-        body: List[ModelMetadata] = None,
-    ) -> None:
-        """
+            This is the quiet version of  'get /api/domains/{domainname}/metadata'
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ModelMetadataSchema)
+
+    def post(
+        self,
+        body: List[ModelMetadata] = None,
+    ) -> None:
+        """
         Create one or more metadata
-            This is the quiet version of  'post /api/domains/{domainname}/metadata'
-        Args:
-        body (List[ModelMetadata]): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=ModelMetadataSchema().dump(body, many=True),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
-
-    
-    
+            This is the quiet version of  'post /api/domains/{domainname}/metadata'
+        Args:
+        body (List[ModelMetadata]): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=ModelMetadataSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_namedentities.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_synonyms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,69 @@
-from semantha_sdk.model.named_entity import NamedEntity
-from semantha_sdk.model.named_entity import NamedEntitySchema
+from semantha_sdk.api.model_synonym import ModelSynonymEndpoint
+from semantha_sdk.model.synonym import Synonym
+from semantha_sdk.model.synonym import SynonymSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkmodelNamedentitiesEndpoint(RestEndpoint):
+class ModelSynonymsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/namedentities"
+        return self._parent_endpoint + "/synonyms"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelSynonymEndpoint:
+        return ModelSynonymEndpoint(self._session, self._endpoint, id)
 
+    def get(
+        self,
+    ) -> List[Synonym]:
+        """
+        Get all synonyms
+        Args:
+            """
+        q_params = {}
     
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(SynonymSchema)
+
     def post(
         self,
-        body: List[NamedEntity] = None,
-    ) -> None:
+        body: Synonym = None,
+    ) -> Synonym:
         """
-        Create one or more named entities
-            This is the quiet version of  'post /api/domains/{domainname}/namedentities'
+        Create a synonym
         Args:
-        body (List[NamedEntity]): 
+        body (Synonym): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=NamedEntitySchema().dump(body, many=True),
+            json=SynonymSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.as_none()
+        return response.to(SynonymSchema)
 
     
-    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete all synonyms
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_rules.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_stopwords.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,69 @@
-from semantha_sdk.model.rule import Rule
-from semantha_sdk.model.rule import RuleSchema
+from semantha_sdk.api.model_stopword import ModelStopwordEndpoint
+from semantha_sdk.model.stop_word import StopWord
+from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkmodelRulesEndpoint(RestEndpoint):
+class ModelStopwordsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/rules"
+        return self._parent_endpoint + "/stopwords"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelStopwordEndpoint:
+        return ModelStopwordEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> List[Rule]:
+    ) -> List[StopWord]:
         """
-        Get a rule
-            This is the quiet version of 'get /api/model/domains/{domainname}/rules'
+        Get all stop words
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(RuleSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(StopWordSchema)
 
     def post(
         self,
-        body: List[Rule] = None,
-    ) -> None:
+        body: StopWord = None,
+    ) -> StopWord:
         """
-        Create a rule
-            This is the quiet version of 'post /api/model/domains/{domainname}/rules'
+        Create a stop word
         Args:
-        body (List[Rule]): 
+        body (StopWord): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=RuleSchema().dump(body, many=True),
+            json=StopWordSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.as_none()
+        return response.to(StopWordSchema)
 
     
-    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete all stop words
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_stopwords.py` & `semantha_sdk-6.9.0/semantha_sdk/api/roles.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-from semantha_sdk.model.stop_word import StopWord
-from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class BulkmodelStopwordsEndpoint(RestEndpoint):
+class RolesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/stopwords"
+        return self._parent_endpoint + "/roles"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
-    
-    def post(
+    def get(
         self,
-        body: List[StopWord] = None,
-    ) -> None:
+    ) -> List[str]:
         """
-        Add a list of stop words to your domain
+        Get the role/s of the current user.
         Args:
-        body (List[StopWord]): 
-        """
+            """
         q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=StopWordSchema().dump(body, many=True),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
 
     
     
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodel_synonyms.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_backups.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-from semantha_sdk.model.synonym import Synonym
-from semantha_sdk.model.synonym import SynonymSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class BulkmodelSynonymsEndpoint(RestEndpoint):
+class ModelBackupsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/synonyms"
+        return self._parent_endpoint + "/backups"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     
     def post(
         self,
-        body: List[Synonym] = None,
     ) -> None:
         """
-        Create one or more synonyms
-            This is the quiet version of  'post /api/domains/{domainname}/synonyms'
+        Create a backup for the ontology
         Args:
-        body (List[Synonym]): 
-        """
+            """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=SynonymSchema().dump(body, many=True),
+            body={
+            },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.as_none()
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/bulkmodelclass_instances.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_boostword.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,57 @@
-from semantha_sdk.model.instance import Instance
-from semantha_sdk.model.instance import InstanceSchema
+from semantha_sdk.model.boost_word import BoostWord
+from semantha_sdk.model.boost_word import BoostWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class BulkmodelclassInstancesEndpoint(RestEndpoint):
+class ModelBoostwordEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/instances"
+        return self._parent_endpoint + f"/{self._id}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
+        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+        self._id = id
 
     def get(
         self,
-    ) -> List[Instance]:
+    ) -> BoostWord:
         """
-        Get all instances of the classes by class id
-            This is the quiet version of 'get /api/model/domains/{domainname}/classes/{id}/instances'
+        Get a boostword by id
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(BoostWordSchema)
 
     
     
-    
-    
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete a boostword by id
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
+    def put(
+        self,
+        body: BoostWord
+    ) -> BoostWord:
+        """
+        Update a boostword by id
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=BoostWordSchema().dump(body)
+        ).execute().to(BoostWordSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/celltypes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/celltypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/child_extractorclasses.py` & `semantha_sdk-6.9.0/semantha_sdk/api/child_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/clone.py` & `semantha_sdk-6.9.0/semantha_sdk/api/clone.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/clusters.py` & `semantha_sdk-6.9.0/semantha_sdk/api/clusters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/currentuser.py` & `semantha_sdk-6.9.0/semantha_sdk/api/currentuser.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/diff.py` & `semantha_sdk-6.9.0/semantha_sdk/api/diff.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/docclass_customfields.py` & `semantha_sdk-6.9.0/semantha_sdk/api/docclass_customfields.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/docclass_documentclasses.py` & `semantha_sdk-6.9.0/semantha_sdk/api/docclass_documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/docclass_referencedocuments.py` & `semantha_sdk-6.9.0/semantha_sdk/api/docclass_referencedocuments.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/documentannotations.py` & `semantha_sdk-6.9.0/semantha_sdk/api/documentannotations.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from io import IOBase
-from semantha_sdk.model.document import Document
-from semantha_sdk.model.document import DocumentSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-
-class DocumentannotationsEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/documentannotations"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post_as_docx(
-        self,
-        file: IOBase = None,
-        document: Document = None,
-        similaritythreshold: float = None,
-        synonymousthreshold: float = None,
-        marknomatch: bool = None,
-        withreferencetext: bool = None,
-    ) -> IOBase:
-        """
-        Download the original input document (pdf or docx) with the referenced document/library matches as annotated comments
-        Args:
-        file (IOBase): Input document (left document).
-    document (Document): 
+from io import IOBase
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+
+class DocumentannotationsEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/documentannotations"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post_as_docx(
+        self,
+        file: IOBase = None,
+        document: Document = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+    ) -> IOBase:
+        """
+        Download the original input document (pdf or docx) with the referenced document/library matches as annotated comments
+        Args:
+        file (IOBase): Input document (left document).
+    document (Document): 
     similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-            In general, the higher the threshold, the more precise the results.
-    synonymousthreshold (float): Threshold for good matches.
-    marknomatch (bool): Marks the paragraphs that have not matched
-    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-                "document": document,
-                "similaritythreshold": similaritythreshold,
-                "synonymousthreshold": synonymousthreshold,
-                "marknomatch": marknomatch,
-                "withreferencetext": withreferencetext,
-            },
-            headers=RestClient.to_header(MediaType.DOCX),
-            q_params=q_params
-        ).execute()
-        return response.as_bytesio()
-    def post_as_pdf(
-        self,
-        file: IOBase = None,
-        document: Document = None,
-        similaritythreshold: float = None,
-        synonymousthreshold: float = None,
-        marknomatch: bool = None,
-        withreferencetext: bool = None,
-    ) -> IOBase:
-        """
-        Download the original input document (pdf or docx) with the referenced document/library matches as annotated comments
-        Args:
-        file (IOBase): Input document (left document).
-    document (Document): 
+            In general, the higher the threshold, the more precise the results.
+    synonymousthreshold (float): Threshold for good matches.
+    marknomatch (bool): Marks the paragraphs that have not matched
+    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "document": document,
+                "similaritythreshold": similaritythreshold,
+                "synonymousthreshold": synonymousthreshold,
+                "marknomatch": marknomatch,
+                "withreferencetext": withreferencetext,
+            },
+            headers=RestClient.to_header(MediaType.DOCX),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
+    def post_as_pdf(
+        self,
+        file: IOBase = None,
+        document: Document = None,
+        similaritythreshold: float = None,
+        synonymousthreshold: float = None,
+        marknomatch: bool = None,
+        withreferencetext: bool = None,
+    ) -> IOBase:
+        """
+        Download the original input document (pdf or docx) with the referenced document/library matches as annotated comments
+        Args:
+        file (IOBase): Input document (left document).
+    document (Document): 
     similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-            In general, the higher the threshold, the more precise the results.
-    synonymousthreshold (float): Threshold for good matches.
-    marknomatch (bool): Marks the paragraphs that have not matched
-    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-                "document": document,
-                "similaritythreshold": similaritythreshold,
-                "synonymousthreshold": synonymousthreshold,
-                "marknomatch": marknomatch,
-                "withreferencetext": withreferencetext,
-            },
-            headers=RestClient.to_header(MediaType.PDF),
-            q_params=q_params
-        ).execute()
-        return response.as_bytesio()
-
-    
-    
+            In general, the higher the threshold, the more precise the results.
+    synonymousthreshold (float): Threshold for good matches.
+    marknomatch (bool): Marks the paragraphs that have not matched
+    withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "document": document,
+                "similaritythreshold": similaritythreshold,
+                "synonymousthreshold": synonymousthreshold,
+                "marknomatch": marknomatch,
+                "withreferencetext": withreferencetext,
+            },
+            headers=RestClient.to_header(MediaType.PDF),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/documentclass.py` & `semantha_sdk-6.9.0/semantha_sdk/api/documentclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/documentclasses.py` & `semantha_sdk-6.9.0/semantha_sdk/api/documentclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/documents.py` & `semantha_sdk-6.9.0/semantha_sdk/api/documents.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from io import IOBase
-from semantha_sdk.model.document import Document
-from semantha_sdk.model.document import DocumentSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class DocumentsEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/documents"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post(
-        self,
-        file: IOBase = None,
-        text: str = None,
-        type: str = None,
-        documenttype: str = None,
-        withareas: bool = None,
-        withcontextparagraphs: bool = None,
-        mode: str = None,
-        withparagraphtype: bool = None,
-    ) -> List[Document]:
-        """
+from io import IOBase
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class DocumentsEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/documents"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        text: str = None,
+        type: str = None,
+        documenttype: str = None,
+        withareas: bool = None,
+        withcontextparagraphs: bool = None,
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> List[Document]:
+        """
         Creates a list of document models from an input document (pdf, docx, txt, zip, xlsx)
-            This service can be used with different accept headers which return the document model as json, pdf or docx. You can send a docx and return it as pdf which is based on the document model.
-        Args:
-        file (IOBase): Input document (left document).
-    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    withareas (bool): Gives back the coordinates of referenced area.
-    withcontextparagraphs (bool): 
+            This service can be used with different accept headers which return the document model as json, pdf or docx. You can send a docx and return it as pdf which is based on the document model.
+        Args:
+        file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    withareas (bool): Gives back the coordinates of referenced area.
+    withcontextparagraphs (bool): 
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    withparagraphtype (bool): The type of the paragraph, for example heading, text
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-                "text": text,
-                "type": type,
-                "documenttype": documenttype,
-                "withareas": withareas,
-                "withcontextparagraphs": withcontextparagraphs,
-                "mode": mode,
-                "withparagraphtype": withparagraphtype,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(DocumentSchema)
-    def post_as_xlsx(
-        self,
-        file: IOBase = None,
-        text: str = None,
-        type: str = None,
-        documenttype: str = None,
-        withareas: bool = None,
-        withcontextparagraphs: bool = None,
-        mode: str = None,
-        withparagraphtype: bool = None,
-    ) -> IOBase:
-        """
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "text": text,
+                "type": type,
+                "documenttype": documenttype,
+                "withareas": withareas,
+                "withcontextparagraphs": withcontextparagraphs,
+                "mode": mode,
+                "withparagraphtype": withparagraphtype,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(DocumentSchema)
+    def post_as_xlsx(
+        self,
+        file: IOBase = None,
+        text: str = None,
+        type: str = None,
+        documenttype: str = None,
+        withareas: bool = None,
+        withcontextparagraphs: bool = None,
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> IOBase:
+        """
         Creates a list of document models from an input document (pdf, docx, txt, zip, xlsx)
-            This service can be used with different accept headers which return the document model as json, pdf or docx. You can send a docx and return it as pdf which is based on the document model.
-        Args:
-        file (IOBase): Input document (left document).
-    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    withareas (bool): Gives back the coordinates of referenced area.
-    withcontextparagraphs (bool): 
+            This service can be used with different accept headers which return the document model as json, pdf or docx. You can send a docx and return it as pdf which is based on the document model.
+        Args:
+        file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    withareas (bool): Gives back the coordinates of referenced area.
+    withcontextparagraphs (bool): 
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    withparagraphtype (bool): The type of the paragraph, for example heading, text
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-                "text": text,
-                "type": type,
-                "documenttype": documenttype,
-                "withareas": withareas,
-                "withcontextparagraphs": withcontextparagraphs,
-                "mode": mode,
-                "withparagraphtype": withparagraphtype,
-            },
-            headers=RestClient.to_header(MediaType.XLSX),
-            q_params=q_params
-        ).execute()
-        return response.as_bytesio()
-    def post_as_docx(
-        self,
-        file: IOBase = None,
-        text: str = None,
-        type: str = None,
-        documenttype: str = None,
-        withareas: bool = None,
-        withcontextparagraphs: bool = None,
-        mode: str = None,
-        withparagraphtype: bool = None,
-    ) -> IOBase:
-        """
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "text": text,
+                "type": type,
+                "documenttype": documenttype,
+                "withareas": withareas,
+                "withcontextparagraphs": withcontextparagraphs,
+                "mode": mode,
+                "withparagraphtype": withparagraphtype,
+            },
+            headers=RestClient.to_header(MediaType.XLSX),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
+    def post_as_docx(
+        self,
+        file: IOBase = None,
+        text: str = None,
+        type: str = None,
+        documenttype: str = None,
+        withareas: bool = None,
+        withcontextparagraphs: bool = None,
+        mode: str = None,
+        withparagraphtype: bool = None,
+    ) -> IOBase:
+        """
         Creates a list of document models from an input document (pdf, docx, txt, zip, xlsx)
-            This service can be used with different accept headers which return the document model as json, pdf or docx. You can send a docx and return it as pdf which is based on the document model.
-        Args:
-        file (IOBase): Input document (left document).
-    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    withareas (bool): Gives back the coordinates of referenced area.
-    withcontextparagraphs (bool): 
+            This service can be used with different accept headers which return the document model as json, pdf or docx. You can send a docx and return it as pdf which is based on the document model.
+        Args:
+        file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    type (str): Choose the structure of a document for similarity or extraction. The type depends on the Use Case you're in.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    withareas (bool): Gives back the coordinates of referenced area.
+    withcontextparagraphs (bool): 
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    withparagraphtype (bool): The type of the paragraph, for example heading, text
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-                "text": text,
-                "type": type,
-                "documenttype": documenttype,
-                "withareas": withareas,
-                "withcontextparagraphs": withcontextparagraphs,
-                "mode": mode,
-                "withparagraphtype": withparagraphtype,
-            },
-            headers=RestClient.to_header(MediaType.DOCX),
-            q_params=q_params
-        ).execute()
-        return response.as_bytesio()
-
-    
-    
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    withparagraphtype (bool): The type of the paragraph, for example heading, text
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "text": text,
+                "type": type,
+                "documenttype": documenttype,
+                "withareas": withareas,
+                "withcontextparagraphs": withcontextparagraphs,
+                "mode": mode,
+                "withparagraphtype": withparagraphtype,
+            },
+            headers=RestClient.to_header(MediaType.DOCX),
+            q_params=q_params
+        ).execute()
+        return response.as_bytesio()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/documenttype.py` & `semantha_sdk-6.9.0/semantha_sdk/api/documenttype.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/documenttypes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/documenttypes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/domain.py` & `semantha_sdk-6.9.0/semantha_sdk/api/domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/domains.py` & `semantha_sdk-6.9.0/semantha_sdk/api/domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/info.py` & `semantha_sdk-6.9.0/semantha_sdk/api/info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/languages.py` & `semantha_sdk-6.9.0/semantha_sdk/api/summarizations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-from io import IOBase
-from semantha_sdk.model.language_detection import LanguageDetection
-from semantha_sdk.model.language_detection import LanguageDetectionSchema
+from semantha_sdk.model.summarization import Summarization
+from semantha_sdk.model.summarization import SummarizationSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
 
-class LanguagesEndpoint(RestEndpoint):
+class SummarizationsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/languages"
+        return self._parent_endpoint + "/summarizations"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     
     def post(
         self,
-        file: IOBase = None,
-    ) -> LanguageDetection:
+        texts: List[str] = None,
+        topic: str = None,
+        language: str = None,
+    ) -> Summarization:
         """
-        Identifies the language of the document and sends it back
-            Input: Support of all input formats (pdf, docx, txt, json (DocumentModel)
-            
-            Output: Detected Language
-            
-            Supported Languages:
-            "ar", "cs", "da", "de", "en", "es", "el", "fr", "fi", "hu", "hr",
-            "it", "ja", "ko", "nl", "no", "pl", "pt", "ro", "ru", "sk", "sl",
-            "sv", "tr", "zh-CN"
+        Generates a summary for given number of texts. If topic is supplied summarization is generated for this topic
         Args:
-        file (IOBase): Input document (left document).
+        texts (List[str]): 
+    topic (str): 
+    language (str): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
             body={
-                "file": file,
+                "texts": texts,
+                "topic": topic,
+                "language": language,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.to(LanguageDetectionSchema)
+        return response.to(SummarizationSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_attributes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_attributes.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_backups.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_extractors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,37 @@
+from semantha_sdk.model.entity import Entity
+from semantha_sdk.model.entity import EntitySchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
 
-class ModelBackupsEndpoint(RestEndpoint):
+class ModelExtractorsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/backups"
+        return self._parent_endpoint + "/extractors"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
-    
-    def post(
+    def get(
         self,
-    ) -> None:
+    ) -> List[Entity]:
         """
-        Create a backup for the ontology
+        Get all extractors
         Args:
             """
         q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.as_none()
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(EntitySchema)
 
     
     
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_boostword.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_onemetadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from semantha_sdk.model.boost_word import BoostWord
-from semantha_sdk.model.boost_word import BoostWordSchema
+from semantha_sdk.model.model_metadata import ModelMetadata
+from semantha_sdk.model.model_metadata import ModelMetadataSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 
-class ModelBoostwordEndpoint(RestEndpoint):
+class ModelOnemetadataEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
@@ -19,39 +19,39 @@
         id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
         self._id = id
 
     def get(
         self,
-    ) -> BoostWord:
+    ) -> ModelMetadata:
         """
-        Get a boostword by id
+        Get metadata by id
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(BoostWordSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ModelMetadataSchema)
 
     
     
     def delete(
         self,
     ) -> None:
         """
-        Delete a boostword by id
+        Delete metadata by id
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
     def put(
         self,
-        body: BoostWord
-    ) -> BoostWord:
+        body: ModelMetadata
+    ) -> ModelMetadata:
         """
-        Update a boostword by id
+        Update metadata by id
         """
         return self._session.put(
             url=self._endpoint,
-            json=BoostWordSchema().dump(body)
-        ).execute().to(BoostWordSchema)
+            json=ModelMetadataSchema().dump(body)
+        ).execute().to(ModelMetadataSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_boostwords.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_stopword.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,57 @@
-from semantha_sdk.api.model_boostword import ModelBoostwordEndpoint
-from semantha_sdk.model.boost_word import BoostWord
-from semantha_sdk.model.boost_word import BoostWordSchema
+from semantha_sdk.model.stop_word import StopWord
+from semantha_sdk.model.stop_word import StopWordSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class ModelBoostwordsEndpoint(RestEndpoint):
+class ModelStopwordEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/boostwords"
+        return self._parent_endpoint + f"/{self._id}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
+        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-    def __call__(
-            self,
-            id: str,
-    ) -> ModelBoostwordEndpoint:
-        return ModelBoostwordEndpoint(self._session, self._endpoint, id)
+        self._id = id
 
     def get(
         self,
-    ) -> List[BoostWord]:
+    ) -> StopWord:
         """
-        Get all boostwords
+        Get a stop word by id
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(BoostWordSchema)
-
-    def post(
-        self,
-        body: BoostWord = None,
-    ) -> BoostWord:
-        """
-        Create a boostword
-        Args:
-        body (BoostWord): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=BoostWordSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(BoostWordSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(StopWordSchema)
 
     
+    
     def delete(
         self,
     ) -> None:
         """
-        Delete all boostwords
+        Delete a stop word by id
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
-    
+    def put(
+        self,
+        body: StopWord
+    ) -> StopWord:
+        """
+        Update a stop word by id
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=StopWordSchema().dump(body)
+        ).execute().to(StopWordSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_dataproperties.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_dataproperties.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_dataproperty.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_dataproperty.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_datatypes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_metadatatypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class ModelDatatypesEndpoint(RestEndpoint):
+class ModelMetadatatypesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/datatypes"
+        return self._parent_endpoint + "/metadatatypes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     def get(
         self,
     ) -> List[str]:
         """
-        Get all datatypes
+        Get all metadatatypes
         Args:
             """
         q_params = {}
     
         return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_domain.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_domain.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_domains.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_domains.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_extractorclass.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_extractorclass.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_extractorclasses.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_extractorclasses.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_extractors.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_extractortypes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from semantha_sdk.model.entity import Entity
-from semantha_sdk.model.entity import EntitySchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class ModelExtractorsEndpoint(RestEndpoint):
+class ModelExtractortypesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/extractors"
+        return self._parent_endpoint + "/extractortypes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     def get(
         self,
-    ) -> List[Entity]:
+    ) -> List[str]:
         """
-        Get all extractors
+        Get all extractortypes
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(EntitySchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_extractortypes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_objectproperties.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
+from semantha_sdk.model.overview import Overview
+from semantha_sdk.model.overview import OverviewSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class ModelExtractortypesEndpoint(RestEndpoint):
+class ModelObjectpropertiesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/extractortypes"
+        return self._parent_endpoint + "/objectproperties"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     def get(
         self,
-    ) -> List[str]:
+    ) -> List[Overview]:
         """
-        Get all extractortypes
+        Get all object properties
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(OverviewSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_formatters.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_formatters.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_metadata.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_metadatatypes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelclasses.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,41 @@
+from semantha_sdk.model.model_class import ModelClass
+from semantha_sdk.model.model_class import ModelClassSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class ModelMetadatatypesEndpoint(RestEndpoint):
+class ModelclassesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/metadatatypes"
+        return self._parent_endpoint + "/modelclasses"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     def get(
         self,
-    ) -> List[str]:
+        uilanguage: str = None,
+    ) -> List[ModelClass]:
         """
-        Get all metadatatypes
+        Get all model classes
         Args:
-            """
+        uilanguage str: Selects the language of the labels in the JSON response; useful with multi-language domain models.
+        """
         q_params = {}
+        if uilanguage is not None:
+            q_params["uilanguage"] = uilanguage
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ModelClassSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_namedentities.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_namedentities.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_namedentity.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_namedentity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_objectproperties.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelont_attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,57 @@
-from semantha_sdk.model.overview import Overview
-from semantha_sdk.model.overview import OverviewSchema
+from semantha_sdk.model.attribute import Attribute
+from semantha_sdk.model.attribute import AttributeSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class ModelObjectpropertiesEndpoint(RestEndpoint):
+class ModelontAttributeEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/objectproperties"
+        return self._parent_endpoint + f"/{self._id}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
+        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+        self._id = id
 
     def get(
         self,
-    ) -> List[Overview]:
+    ) -> Attribute:
         """
-        Get all object properties
+        
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(OverviewSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(AttributeSchema)
 
     
     
-    
-    
+    def delete(
+        self,
+    ) -> None:
+        """
+        
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
+    def put(
+        self,
+        body: Attribute
+    ) -> Attribute:
+        """
+        
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=AttributeSchema().dump(body)
+        ).execute().to(AttributeSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_onemetadata.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelont_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-from semantha_sdk.model.model_metadata import ModelMetadata
-from semantha_sdk.model.model_metadata import ModelMetadataSchema
+from semantha_sdk.api.modelont_attributes import ModelontAttributesEndpoint
+from semantha_sdk.api.modelontclass_instances import ModelontclassInstancesEndpoint
+from semantha_sdk.model.clazz import Clazz
+from semantha_sdk.model.clazz import ClazzSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 
-class ModelOnemetadataEndpoint(RestEndpoint):
+class ModelontClassEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + f"/{self._classid}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        id: str,
+        classid: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._id = id
+        self._classid = classid
+        self.__attributes = ModelontAttributesEndpoint(session, self._endpoint)
+        self.__instances = ModelontclassInstancesEndpoint(session, self._endpoint)
+    
+    @property
+    def attributes(self) -> ModelontAttributesEndpoint:
+        return self.__attributes
+    
+    @property
+    def instances(self) -> ModelontclassInstancesEndpoint:
+        return self.__instances
 
     def get(
         self,
-    ) -> ModelMetadata:
+    ) -> Clazz:
         """
-        Get metadata by id
+        
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ModelMetadataSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ClazzSchema)
 
     
     
     def delete(
         self,
     ) -> None:
         """
-        Delete metadata by id
+        
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
     def put(
         self,
-        body: ModelMetadata
-    ) -> ModelMetadata:
+        body: Clazz
+    ) -> Clazz:
         """
-        Update metadata by id
+        
         """
         return self._session.put(
             url=self._endpoint,
-            json=ModelMetadataSchema().dump(body)
-        ).execute().to(ModelMetadataSchema)
+            json=ClazzSchema().dump(body)
+        ).execute().to(ClazzSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_regex.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_regex.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_regexes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_synonym.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,57 @@
-from semantha_sdk.api.model_regex import ModelRegexEndpoint
-from semantha_sdk.model.regex import Regex
-from semantha_sdk.model.regex import RegexSchema
+from semantha_sdk.model.synonym import Synonym
+from semantha_sdk.model.synonym import SynonymSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class ModelRegexesEndpoint(RestEndpoint):
+class ModelSynonymEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/regexes"
+        return self._parent_endpoint + f"/{self._id}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
+        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-    def __call__(
-            self,
-            id: str,
-    ) -> ModelRegexEndpoint:
-        return ModelRegexEndpoint(self._session, self._endpoint, id)
+        self._id = id
 
     def get(
         self,
-    ) -> List[Regex]:
+    ) -> Synonym:
         """
-        Get all regexes
+        Get a synonym by id
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(RegexSchema)
-
-    def post(
-        self,
-        body: Regex = None,
-    ) -> Regex:
-        """
-        Create a new regex
-        Args:
-        body (Regex): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=RegexSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(RegexSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(SynonymSchema)
 
     
+    
     def delete(
         self,
     ) -> None:
         """
-        Delete all regexes
+        Delete a synonym by id
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
-    
+    def put(
+        self,
+        body: Synonym
+    ) -> Synonym:
+        """
+        Update a synonym by id
+        """
+        return self._session.put(
+            url=self._endpoint,
+            json=SynonymSchema().dump(body)
+        ).execute().to(SynonymSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_relation.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_relations.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_relations.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_rule.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_rulefunctions.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_rulefunctions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_rules.py` & `semantha_sdk-6.9.0/semantha_sdk/api/model_rules.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_stopword.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelont_attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-from semantha_sdk.model.stop_word import StopWord
-from semantha_sdk.model.stop_word import StopWordSchema
+from semantha_sdk.api.modelont_attribute import ModelontAttributeEndpoint
+from semantha_sdk.model.attribute import Attribute
+from semantha_sdk.model.attribute import AttributeSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
 
-class ModelStopwordEndpoint(RestEndpoint):
+class ModelontAttributesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/attributes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._id = id
+    def __call__(
+            self,
+            id: str,
+    ) -> ModelontAttributeEndpoint:
+        return ModelontAttributeEndpoint(self._session, self._endpoint, id)
 
     def get(
         self,
-    ) -> StopWord:
+    ) -> List[Attribute]:
         """
-        Get a stop word by id
+        
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(StopWordSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(AttributeSchema)
 
-    
-    
-    def delete(
+    def post(
         self,
-    ) -> None:
+        body: Attribute = None,
+    ) -> Attribute:
         """
-        Delete a stop word by id
+        
+        Args:
+        body (Attribute): 
         """
-        self._session.delete(
+        q_params = {}
+        response = self._session.post(
             url=self._endpoint,
+            json=AttributeSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
         ).execute()
+        return response.to(AttributeSchema)
 
-    def put(
+    
+    def delete(
         self,
-        body: StopWord
-    ) -> StopWord:
+    ) -> None:
         """
-        Update a stop word by id
+        
         """
-        return self._session.put(
+        self._session.delete(
             url=self._endpoint,
-            json=StopWordSchema().dump(body)
-        ).execute().to(StopWordSchema)
+        ).execute()
+
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_stopwords.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelont_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,79 @@
-from semantha_sdk.api.model_stopword import ModelStopwordEndpoint
-from semantha_sdk.model.stop_word import StopWord
-from semantha_sdk.model.stop_word import StopWordSchema
+from semantha_sdk.api.modelont_class import ModelontClassEndpoint
+from semantha_sdk.model.classes_overview import ClassesOverview
+from semantha_sdk.model.classes_overview import ClassesOverviewSchema
+from semantha_sdk.model.clazz import Clazz
+from semantha_sdk.model.clazz import ClazzSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class ModelStopwordsEndpoint(RestEndpoint):
+class ModelontClassesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/stopwords"
+        return self._parent_endpoint + "/classes"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
     def __call__(
             self,
-            id: str,
-    ) -> ModelStopwordEndpoint:
-        return ModelStopwordEndpoint(self._session, self._endpoint, id)
+            classid: str,
+    ) -> ModelontClassEndpoint:
+        return ModelontClassEndpoint(self._session, self._endpoint, classid)
 
     def get(
         self,
-    ) -> List[StopWord]:
+        withattributes: bool = None,
+        withobjectproperties: bool = None,
+    ) -> List[ClassesOverview]:
         """
-        Get all stop words
+        Get all classes
         Args:
-            """
+        withattributes bool: Select if the classes are delivered with attributes
+    withobjectproperties bool: Select if the classes are delivered with object properties
+        """
         q_params = {}
+        if withattributes is not None:
+            q_params["withattributes"] = withattributes
+        if withobjectproperties is not None:
+            q_params["withobjectproperties"] = withobjectproperties
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(StopWordSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ClassesOverviewSchema)
 
     def post(
         self,
-        body: StopWord = None,
-    ) -> StopWord:
+        body: Clazz = None,
+    ) -> Clazz:
         """
-        Create a stop word
+        Create a class
         Args:
-        body (StopWord): 
+        body (Clazz): 
         """
         q_params = {}
         response = self._session.post(
             url=self._endpoint,
-            json=StopWordSchema().dump(body),
+            json=ClazzSchema().dump(body),
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
-        return response.to(StopWordSchema)
+        return response.to(ClazzSchema)
 
     
     def delete(
         self,
     ) -> None:
         """
-        Delete all stop words
+        Delete all classes
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_synonym.py` & `semantha_sdk-6.9.0/semantha_sdk/api/tag_referencedocuments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,46 @@
-from semantha_sdk.model.synonym import Synonym
-from semantha_sdk.model.synonym import SynonymSchema
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.document_information import DocumentInformationSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
 
-class ModelSynonymEndpoint(RestEndpoint):
+class TagReferencedocumentsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/referencedocuments"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._id = id
 
     def get(
         self,
-    ) -> Synonym:
+    ) -> List[DocumentInformation]:
         """
-        Get a synonym by id
+        Get all reference documents with a specific tag
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(SynonymSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DocumentInformationSchema)
 
     
     
     def delete(
         self,
     ) -> None:
         """
-        Delete a synonym by id
+        Delete reference documents with a specific tag
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
-    def put(
-        self,
-        body: Synonym
-    ) -> Synonym:
-        """
-        Update a synonym by id
-        """
-        return self._session.put(
-            url=self._endpoint,
-            json=SynonymSchema().dump(body)
-        ).execute().to(SynonymSchema)
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/model_synonyms.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_synonyms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,45 @@
-from semantha_sdk.api.model_synonym import ModelSynonymEndpoint
-from semantha_sdk.model.synonym import Synonym
-from semantha_sdk.model.synonym import SynonymSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class ModelSynonymsEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/synonyms"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-    def __call__(
-            self,
-            id: str,
-    ) -> ModelSynonymEndpoint:
-        return ModelSynonymEndpoint(self._session, self._endpoint, id)
-
-    def get(
-        self,
-    ) -> List[Synonym]:
-        """
-        Get all synonyms
-        Args:
-            """
-        q_params = {}
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(SynonymSchema)
-
-    def post(
-        self,
-        body: Synonym = None,
-    ) -> Synonym:
-        """
-        Create a synonym
-        Args:
-        body (Synonym): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=SynonymSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(SynonymSchema)
-
-    
-    def delete(
-        self,
-    ) -> None:
-        """
-        Delete all synonyms
-        """
-        self._session.delete(
-            url=self._endpoint,
-        ).execute()
-
+from semantha_sdk.model.synonym import Synonym
+from semantha_sdk.model.synonym import SynonymSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkmodelSynonymsEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/synonyms"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        body: List[Synonym] = None,
+    ) -> None:
+        """
+        Create one or more synonyms
+            This is the quiet version of  'post /api/domains/{domainname}/synonyms'
+        Args:
+        body (List[Synonym]): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=SynonymSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelclasses.py` & `semantha_sdk-6.9.0/semantha_sdk/api/statistic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-from semantha_sdk.model.model_class import ModelClass
-from semantha_sdk.model.model_class import ModelClassSchema
+from semantha_sdk.model.statistic import Statistic
+from semantha_sdk.model.statistic import StatisticSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class ModelclassesEndpoint(RestEndpoint):
+class StatisticEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/modelclasses"
+        return self._parent_endpoint + "/statistic"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
 
     def get(
         self,
-        uilanguage: str = None,
-    ) -> List[ModelClass]:
+    ) -> Statistic:
         """
-        Get all model classes
+        Returns statistical information about the reference documents a.k.a. library.
         Args:
-        uilanguage str: Selects the language of the labels in the JSON response; useful with multi-language domain models.
-        """
+            """
         q_params = {}
-        if uilanguage is not None:
-            q_params["uilanguage"] = uilanguage
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ModelClassSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(StatisticSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelinstances.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelinstances.py`

 * *Files 19% similar despite different names*

```diff
@@ -57,14 +57,46 @@
                 "documentextractor": documentextractor,
                 "applymatchersfordocumentextractor": applymatchersfordocumentextractor,
             },
             headers=RestClient.to_header(MediaType.JSON),
             q_params=q_params
         ).execute()
         return response.to(SemanticModelSchema)
+    def post_json(
+        self,
+        body: SemanticModel = None,
+        withimages: bool = None,
+        withdocument: bool = None,
+        withadditionalroots: bool = None,
+        documenttype: str = None,
+        uilanguage: str = None,
+    ) -> SemanticModel:
+        """
+        Extract semantic model for a list of documents
+        Args:
+        body (SemanticModel): 
+        """
+        q_params = {}
+        if withimages is not None:
+            q_params["withimages"] = withimages
+        if withdocument is not None:
+            q_params["withdocument"] = withdocument
+        if withadditionalroots is not None:
+            q_params["withadditionalroots"] = withadditionalroots
+        if documenttype is not None:
+            q_params["documenttype"] = documenttype
+        if uilanguage is not None:
+            q_params["uilanguage"] = uilanguage
+        response = self._session.post(
+            url=self._endpoint,
+            json=SemanticModelSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(SemanticModelSchema)
     def post_as_xlsx(
         self,
         file: IOBase = None,
         documentextractor: str = None,
         applymatchersfordocumentextractor: bool = None,
         withimages: bool = None,
         withdocument: bool = None,
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelont_attribute.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelont_instance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from semantha_sdk.model.attribute import Attribute
-from semantha_sdk.model.attribute import AttributeSchema
+from semantha_sdk.model.instance import Instance
+from semantha_sdk.model.instance import InstanceSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 
-class ModelontAttributeEndpoint(RestEndpoint):
+class ModelontInstanceEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
         return self._parent_endpoint + f"/{self._id}"
@@ -19,39 +19,39 @@
         id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
         self._id = id
 
     def get(
         self,
-    ) -> Attribute:
+    ) -> Instance:
         """
-        
+        Get an instance by id
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(AttributeSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
 
     
     
     def delete(
         self,
     ) -> None:
         """
-        
+        Delete an instance by id
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
     def put(
         self,
-        body: Attribute
-    ) -> Attribute:
+        body: Instance
+    ) -> Instance:
         """
-        
+        Update an instance by id
         """
         return self._session.put(
             url=self._endpoint,
-            json=AttributeSchema().dump(body)
-        ).execute().to(AttributeSchema)
+            json=InstanceSchema().dump(body)
+        ).execute().to(InstanceSchema)
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelont_attributes.py` & `semantha_sdk-6.9.0/semantha_sdk/api/semantha_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,73 @@
-from semantha_sdk.api.modelont_attribute import ModelontAttributeEndpoint
-from semantha_sdk.model.attribute import Attribute
-from semantha_sdk.model.attribute import AttributeSchema
-from semantha_sdk.rest.rest_client import MediaType
+from __future__ import annotations
+
+from io import IOBase
+
+from semantha_sdk.api.bulk import BulkEndpoint
+from semantha_sdk.api.celltypes import CelltypesEndpoint
+from semantha_sdk.api.currentuser import CurrentuserEndpoint
+from semantha_sdk.api.diff import DiffEndpoint
+from semantha_sdk.api.domains import DomainsEndpoint
+from semantha_sdk.api.info import InfoEndpoint
+from semantha_sdk.api.languages import LanguagesEndpoint
+from semantha_sdk.api.model import ModelEndpoint
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
 
-class ModelontAttributesEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
+
+class SemanthaAPI(RestEndpoint):
+    """ Entry point to the Semantha API.
+
+        author semantha, this is a generated class do not change manually!
+        Calls the /bulk, /celltypes, /currentuser, /diff, /domains, /info, /languages, /model,  endpoints.
+
+        Note:
+            The __init__ method is not meant to be invoked directly
+            use `login()` with your credentials instead.
     """
 
+    def __init__(self, session: RestClient, parent_endpoint: str):
+        super().__init__(session, parent_endpoint)
+        self.__bulk = BulkEndpoint(session, self._endpoint)
+        self.__celltypes = CelltypesEndpoint(session, self._endpoint)
+        self.__currentuser = CurrentuserEndpoint(session, self._endpoint)
+        self.__diff = DiffEndpoint(session, self._endpoint)
+        self.__domains = DomainsEndpoint(session, self._endpoint)
+        self.__info = InfoEndpoint(session, self._endpoint)
+        self.__languages = LanguagesEndpoint(session, self._endpoint)
+        self.__model = ModelEndpoint(session, self._endpoint)
+
     @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/attributes"
+    def _endpoint(self):
+        return self._parent_endpoint
 
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-    def __call__(
-            self,
-            id: str,
-    ) -> ModelontAttributeEndpoint:
-        return ModelontAttributeEndpoint(self._session, self._endpoint, id)
-
-    def get(
-        self,
-    ) -> List[Attribute]:
-        """
-        
-        Args:
-            """
-        q_params = {}
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(AttributeSchema)
-
-    def post(
-        self,
-        body: Attribute = None,
-    ) -> Attribute:
-        """
-        
-        Args:
-        body (Attribute): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            json=AttributeSchema().dump(body),
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(AttributeSchema)
-
-    
-    def delete(
-        self,
-    ) -> None:
-        """
-        
-        """
-        self._session.delete(
-            url=self._endpoint,
-        ).execute()
+    @property
+    def bulk(self) -> BulkEndpoint:
+        return self.__bulk
+
+    @property
+    def celltypes(self) -> CelltypesEndpoint:
+        return self.__celltypes
+
+    @property
+    def currentuser(self) -> CurrentuserEndpoint:
+        return self.__currentuser
+
+    @property
+    def diff(self) -> DiffEndpoint:
+        return self.__diff
+
+    @property
+    def domains(self) -> DomainsEndpoint:
+        return self.__domains
+
+    @property
+    def info(self) -> InfoEndpoint:
+        return self.__info
+
+    @property
+    def languages(self) -> LanguagesEndpoint:
+        return self.__languages
+
+    @property
+    def model(self) -> ModelEndpoint:
+        return self.__model
 
-
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelont_class.py` & `semantha_sdk-6.9.0/semantha_sdk/api/referencedocument.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-from semantha_sdk.api.modelont_attributes import ModelontAttributesEndpoint
-from semantha_sdk.api.modelontclass_instances import ModelontclassInstancesEndpoint
-from semantha_sdk.model.clazz import Clazz
-from semantha_sdk.model.clazz import ClazzSchema
+from semantha_sdk.api.paragraphs import ParagraphsEndpoint
+from semantha_sdk.api.sentences import SentencesEndpoint
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.document_information import DocumentInformationSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 
-class ModelontClassEndpoint(RestEndpoint):
+class ReferencedocumentEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._classid}"
+        return self._parent_endpoint + f"/{self._documentid}"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        classid: str,
+        documentid: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._classid = classid
-        self.__attributes = ModelontAttributesEndpoint(session, self._endpoint)
-        self.__instances = ModelontclassInstancesEndpoint(session, self._endpoint)
+        self._documentid = documentid
+        self.__paragraphs = ParagraphsEndpoint(session, self._endpoint)
+        self.__sentences = SentencesEndpoint(session, self._endpoint)
     
     @property
-    def attributes(self) -> ModelontAttributesEndpoint:
-        return self.__attributes
+    def paragraphs(self) -> ParagraphsEndpoint:
+        return self.__paragraphs
     
     @property
-    def instances(self) -> ModelontclassInstancesEndpoint:
-        return self.__instances
+    def sentences(self) -> SentencesEndpoint:
+        return self.__sentences
 
     def get(
         self,
-    ) -> Clazz:
+        querybyname: bool = None,
+    ) -> Document:
         """
-        
+        Returns one reference document by ID.
         Args:
-            """
+        querybyname bool: If true, documentid is treated as name and we search for a document with a given name.
+        """
         q_params = {}
+        if querybyname is not None:
+            q_params["querybyname"] = querybyname
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ClazzSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DocumentSchema)
 
     
-    
-    def delete(
+    def patch(
         self,
-    ) -> None:
+        body: DocumentInformation
+    ) -> DocumentInformation:
         """
-        
+        Change one reference document. Needs roles: 'Domain Admin' or 'Expert User'
         """
-        self._session.delete(
+        return self._session.patch(
             url=self._endpoint,
-        ).execute()
+            json=DocumentInformationSchema().dump(body)
+        ).execute().to(DocumentInformationSchema)
 
-    def put(
+    def delete(
         self,
-        body: Clazz
-    ) -> Clazz:
+    ) -> None:
         """
-        
+        Delete one reference document. Needs roles: 'Domain Admin' or 'Expert User'
         """
-        return self._session.put(
+        self._session.delete(
             url=self._endpoint,
-            json=ClazzSchema().dump(body)
-        ).execute().to(ClazzSchema)
+        ).execute()
+
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelont_instance.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelontclass_instances.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 from semantha_sdk.model.instance import Instance
 from semantha_sdk.model.instance import InstanceSchema
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
 
-class ModelontInstanceEndpoint(RestEndpoint):
+class ModelontclassInstancesEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + f"/{self._id}"
+        return self._parent_endpoint + "/instances"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
-        id: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
-        self._id = id
 
     def get(
         self,
-    ) -> Instance:
+    ) -> List[Instance]:
         """
-        Get an instance by id
+        Get all instances of a specific class
         Args:
             """
         q_params = {}
     
         return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
 
     
     
     def delete(
         self,
     ) -> None:
         """
-        Delete an instance by id
+        Delete all instances of a specific class
         """
         self._session.delete(
             url=self._endpoint,
         ).execute()
 
-    def put(
-        self,
-        body: Instance
-    ) -> Instance:
-        """
-        Update an instance by id
-        """
-        return self._session.put(
-            url=self._endpoint,
-            json=InstanceSchema().dump(body)
-        ).execute().to(InstanceSchema)
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelont_instances.py` & `semantha_sdk-6.9.0/semantha_sdk/api/modelont_instances.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/modelontclass_instances.py` & `semantha_sdk-6.9.0/semantha_sdk/api/tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from semantha_sdk.model.instance import Instance
-from semantha_sdk.model.instance import InstanceSchema
+from semantha_sdk.api.tag import TagEndpoint
 from semantha_sdk.rest.rest_client import MediaType
 from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
 from typing import List
 
-class ModelontclassInstancesEndpoint(RestEndpoint):
+class TagsEndpoint(RestEndpoint):
     """ author semantha, this is a generated class do not change manually! 
     
     """
 
     @property
     def _endpoint(self) -> str:
-        return self._parent_endpoint + "/instances"
+        return self._parent_endpoint + "/tags"
 
     def __init__(
         self,
         session: RestClient,
         parent_endpoint: str,
     ) -> None:
         super().__init__(session, parent_endpoint)
+    def __call__(
+            self,
+            tagname: str,
+    ) -> TagEndpoint:
+        return TagEndpoint(self._session, self._endpoint, tagname)
 
     def get(
         self,
-    ) -> List[Instance]:
+    ) -> List[str]:
         """
-        Get all instances of a specific class
+        Get tags
         Args:
             """
         q_params = {}
     
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
 
     
     
-    def delete(
-        self,
-    ) -> None:
-        """
-        Delete all instances of a specific class
-        """
-        self._session.delete(
-            url=self._endpoint,
-        ).execute()
-
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/namedentities.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_instances.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,56 @@
-from semantha_sdk.model.document_named_entity import DocumentNamedEntity
-from semantha_sdk.model.document_named_entity import DocumentNamedEntitySchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class NamedentitiesEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/namedentities"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    def get(
-        self,
-        tags: str = None,
-        documentclassids: str = None,
-    ) -> List[DocumentNamedEntity]:
-        """
-        Get all named entities (a.k.a custom entities) from reference documents.
-            Can be filtered by tags or documentclassids.
-        Args:
-        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs.
-            The IDs are passed as a JSON array.
-            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
-        """
-        q_params = {}
-        if tags is not None:
-            q_params["tags"] = tags
-        if documentclassids is not None:
-            q_params["documentclassids"] = documentclassids
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(DocumentNamedEntitySchema)
-
-    
-    
-    
+from semantha_sdk.model.instance import Instance
+from semantha_sdk.model.instance import InstanceSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkmodelInstancesEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/instances"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def get(
+        self,
+    ) -> List[Instance]:
+        """
+        Get all instances
+            This is the quiet version of  'get /api/domains/{domainname}/instances'
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
+
+    def post(
+        self,
+        body: List[Instance] = None,
+    ) -> None:
+        """
+        Create an instance
+            This is the quiet version of 'post /api/model/domains/{domainname}/instances'
+        Args:
+        body (List[Instance]): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=InstanceSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/paragraph.py` & `semantha_sdk-6.9.0/semantha_sdk/api/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/paragraphs.py` & `semantha_sdk-6.9.0/semantha_sdk/api/paragraphs.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/referencedocuments.py` & `semantha_sdk-6.9.0/semantha_sdk/api/referencedocuments.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,293 +1,315 @@
-from io import IOBase
-from semantha_sdk.api.clusters import ClustersEndpoint
-from semantha_sdk.api.namedentities import NamedentitiesEndpoint
-from semantha_sdk.api.referencedocument import ReferencedocumentEndpoint
-from semantha_sdk.api.statistic import StatisticEndpoint
-from semantha_sdk.model.document_information import DocumentInformation
-from semantha_sdk.model.document_information import DocumentInformationSchema
-from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainer
-from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainerSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class ReferencedocumentsEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/referencedocuments"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-        self.__clusters = ClustersEndpoint(session, self._endpoint)
-        self.__namedentities = NamedentitiesEndpoint(session, self._endpoint)
-        self.__statistic = StatisticEndpoint(session, self._endpoint)
-    
-    @property
-    def clusters(self) -> ClustersEndpoint:
-        return self.__clusters
-    
-    @property
-    def namedentities(self) -> NamedentitiesEndpoint:
-        return self.__namedentities
-    
-    @property
-    def statistic(self) -> StatisticEndpoint:
-        return self.__statistic
-    def __call__(
-            self,
-            documentid: str,
-    ) -> ReferencedocumentEndpoint:
-        return ReferencedocumentEndpoint(self._session, self._endpoint, documentid)
-
-    def get(
-        self,
-        tags: str = None,
-        documentids: str = None,
-        name: str = None,
-        createdafter: int = None,
-        createdbefore: int = None,
-        updatedafter: int = None,
-        updatedbefore: int = None,
-        documentclassids: str = None,
-        withoutdocumentclass: bool = None,
-        mincharacters: int = None,
-        metadata: str = None,
-        comment: str = None,
-        sourcedoc: bool = None,
-        sourcedocumentid: str = None,
-        offset: int = None,
-        limit: int = None,
-        sort: str = None,
-        fields: str = None,
-    ) -> ReferenceDocumentsResponseContainer:
-        """
+from io import IOBase
+from semantha_sdk.api.clusters import ClustersEndpoint
+from semantha_sdk.api.namedentities import NamedentitiesEndpoint
+from semantha_sdk.api.referencedocument import ReferencedocumentEndpoint
+from semantha_sdk.api.statistic import StatisticEndpoint
+from semantha_sdk.model.document import Document
+from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.document_information import DocumentInformationSchema
+from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainer
+from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainerSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class ReferencedocumentsEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/referencedocuments"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self.__clusters = ClustersEndpoint(session, self._endpoint)
+        self.__namedentities = NamedentitiesEndpoint(session, self._endpoint)
+        self.__statistic = StatisticEndpoint(session, self._endpoint)
+    
+    @property
+    def clusters(self) -> ClustersEndpoint:
+        return self.__clusters
+    
+    @property
+    def namedentities(self) -> NamedentitiesEndpoint:
+        return self.__namedentities
+    
+    @property
+    def statistic(self) -> StatisticEndpoint:
+        return self.__statistic
+    def __call__(
+            self,
+            documentid: str,
+    ) -> ReferencedocumentEndpoint:
+        return ReferencedocumentEndpoint(self._session, self._endpoint, documentid)
+
+    def get(
+        self,
+        tags: str = None,
+        documentids: str = None,
+        name: str = None,
+        createdafter: int = None,
+        createdbefore: int = None,
+        updatedafter: int = None,
+        updatedbefore: int = None,
+        documentclassids: str = None,
+        withoutdocumentclass: bool = None,
+        mincharacters: int = None,
+        metadata: str = None,
+        comment: str = None,
+        sourcedoc: bool = None,
+        sourcedocumentid: str = None,
+        offset: int = None,
+        limit: int = None,
+        sort: str = None,
+        fields: str = None,
+    ) -> ReferenceDocumentsResponseContainer:
+        """
         Get all reference documents a.k.a. library items.
             Supports server side pagination and filtering for "application/json" media type only by using "offset" and "limit" query parameter.
             "Filter parameters:" name, createdbefore, createdafter, tags, documentclassids, metadata.
-            Without "offset" and "limit" parameter, data can be filtered only by "tags" and "documentclassids".
-        Args:
-        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    documentids str: List of document Ids for target. The limit here is 65000 IDs. The IDs can be passed as a comma separated string.
-    name str: Filter documents for a given name
-    createdafter int: Filter for documents which are created after a given UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
-    createdbefore int: Filter for documents which are created before a given UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
-    updatedafter int: Filter for documents which are updated after a given UNIX timestamp. The updatedafter filter only works when also using the parameters offset and limit.
-    updatedbefore int: Filter for documents which are updated before a given UNIX timestamp. The updatedbefore filter only works when also using the parameters offset and limit.
-    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs. The IDs are passed as a comma separated list.
-    withoutdocumentclass bool: Filters the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
-    mincharacters int: Filters the returned reference documents to include only documents that have a minimum of characters
-    metadata str: Filter documents for part of metadata, casing is ignored.
-    comment str: Filter documents for part of comment, casing is ignored.
-    sourcedoc bool: If true, then only source documents are returned.
-    sourcedocumentid str: Filter documents a specific source document.
-    offset int: Specify from which number on reference documents should be returned.
-    limit int: Specify the number of reference documents to be returned.
-    sort str: Define by which fields the returned reference documents are sorted. The following values can be sent as a comma-separated list: 'name', 'filename', 'metadata', 'created', 'updated', 'color', 'comment', 'derivedcolor', 'derivedcomment', 'documentclass'. Add a - before the field name to sort in descending order. Example: "documentclass,-created".
-    fields str: Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: 'id', 'name', 'tags', 'derivedtags', 'metadata', 'filename', 'created', 'processed', 'lang', 'updated, color, derivedcolor, comment, derivedcomment, documentclass, contentpreview'. If empty or null all fields will be returned. Example: "id,name,contentpreview,tags"
-        """
-        q_params = {}
-        if tags is not None:
-            q_params["tags"] = tags
-        if documentids is not None:
-            q_params["documentids"] = documentids
-        if name is not None:
-            q_params["name"] = name
-        if createdafter is not None:
-            q_params["createdafter"] = createdafter
-        if createdbefore is not None:
-            q_params["createdbefore"] = createdbefore
-        if updatedafter is not None:
-            q_params["updatedafter"] = updatedafter
-        if updatedbefore is not None:
-            q_params["updatedbefore"] = updatedbefore
-        if documentclassids is not None:
-            q_params["documentclassids"] = documentclassids
-        if withoutdocumentclass is not None:
-            q_params["withoutdocumentclass"] = withoutdocumentclass
-        if mincharacters is not None:
-            q_params["mincharacters"] = mincharacters
-        if metadata is not None:
-            q_params["metadata"] = metadata
-        if comment is not None:
-            q_params["comment"] = comment
-        if sourcedoc is not None:
-            q_params["sourcedoc"] = sourcedoc
-        if sourcedocumentid is not None:
-            q_params["sourcedocumentid"] = sourcedocumentid
-        if offset is not None:
-            q_params["offset"] = offset
-        if limit is not None:
-            q_params["limit"] = limit
-        if sort is not None:
-            q_params["sort"] = sort
-        if fields is not None:
-            q_params["fields"] = fields
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ReferenceDocumentsResponseContainerSchema)
-    def get_as_xlsx(
-        self,
-        tags: str = None,
-        documentids: str = None,
-        name: str = None,
-        createdafter: int = None,
-        createdbefore: int = None,
-        updatedafter: int = None,
-        updatedbefore: int = None,
-        documentclassids: str = None,
-        withoutdocumentclass: bool = None,
-        mincharacters: int = None,
-        metadata: str = None,
-        comment: str = None,
-        sourcedoc: bool = None,
-        sourcedocumentid: str = None,
-        offset: int = None,
-        limit: int = None,
-        sort: str = None,
-        fields: str = None,
-    ) -> IOBase:
-        """
+            Without "offset" and "limit" parameter, data can be filtered only by "tags" and "documentclassids".
+        Args:
+        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentids str: List of document Ids for target. The limit here is 65000 IDs. The IDs can be passed as a comma separated string.
+    name str: Filter documents for a given name
+    createdafter int: Filter for documents which are created after a given UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
+    createdbefore int: Filter for documents which are created before a given UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
+    updatedafter int: Filter for documents which are updated after a given UNIX timestamp. The updatedafter filter only works when also using the parameters offset and limit.
+    updatedbefore int: Filter for documents which are updated before a given UNIX timestamp. The updatedbefore filter only works when also using the parameters offset and limit.
+    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs. The IDs are passed as a comma separated list.
+    withoutdocumentclass bool: Filters the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
+    mincharacters int: Filters the returned reference documents to include only documents that have a minimum of characters
+    metadata str: Filter documents for part of metadata, casing is ignored.
+    comment str: Filter documents for part of comment, casing is ignored.
+    sourcedoc bool: If true, then only source documents are returned.
+    sourcedocumentid str: Filter documents a specific source document.
+    offset int: Specify from which number on reference documents should be returned.
+    limit int: Specify the number of reference documents to be returned.
+    sort str: Define by which fields the returned reference documents are sorted. The following values can be sent as a comma-separated list: 'name', 'filename', 'metadata', 'created', 'updated', 'color', 'comment', 'derivedcolor', 'derivedcomment', 'documentclass'. Add a - before the field name to sort in descending order. Example: "documentclass,-created".
+    fields str: Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: 'id', 'name', 'tags', 'derivedtags', 'metadata', 'filename', 'created', 'processed', 'lang', 'updated, color, derivedcolor, comment, derivedcomment, documentclass, contentpreview'. If empty or null all fields will be returned. Example: "id,name,contentpreview,tags"
+        """
+        q_params = {}
+        if tags is not None:
+            q_params["tags"] = tags
+        if documentids is not None:
+            q_params["documentids"] = documentids
+        if name is not None:
+            q_params["name"] = name
+        if createdafter is not None:
+            q_params["createdafter"] = createdafter
+        if createdbefore is not None:
+            q_params["createdbefore"] = createdbefore
+        if updatedafter is not None:
+            q_params["updatedafter"] = updatedafter
+        if updatedbefore is not None:
+            q_params["updatedbefore"] = updatedbefore
+        if documentclassids is not None:
+            q_params["documentclassids"] = documentclassids
+        if withoutdocumentclass is not None:
+            q_params["withoutdocumentclass"] = withoutdocumentclass
+        if mincharacters is not None:
+            q_params["mincharacters"] = mincharacters
+        if metadata is not None:
+            q_params["metadata"] = metadata
+        if comment is not None:
+            q_params["comment"] = comment
+        if sourcedoc is not None:
+            q_params["sourcedoc"] = sourcedoc
+        if sourcedocumentid is not None:
+            q_params["sourcedocumentid"] = sourcedocumentid
+        if offset is not None:
+            q_params["offset"] = offset
+        if limit is not None:
+            q_params["limit"] = limit
+        if sort is not None:
+            q_params["sort"] = sort
+        if fields is not None:
+            q_params["fields"] = fields
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(ReferenceDocumentsResponseContainerSchema)
+    def get_as_xlsx(
+        self,
+        tags: str = None,
+        documentids: str = None,
+        name: str = None,
+        createdafter: int = None,
+        createdbefore: int = None,
+        updatedafter: int = None,
+        updatedbefore: int = None,
+        documentclassids: str = None,
+        withoutdocumentclass: bool = None,
+        mincharacters: int = None,
+        metadata: str = None,
+        comment: str = None,
+        sourcedoc: bool = None,
+        sourcedocumentid: str = None,
+        offset: int = None,
+        limit: int = None,
+        sort: str = None,
+        fields: str = None,
+    ) -> IOBase:
+        """
         Get all reference documents a.k.a. library items.
             Supports server side pagination and filtering for "application/json" media type only by using "offset" and "limit" query parameter.
             "Filter parameters:" name, createdbefore, createdafter, tags, documentclassids, metadata.
-            Without "offset" and "limit" parameter, data can be filtered only by "tags" and "documentclassids".
-        Args:
-        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    documentids str: List of document Ids for target. The limit here is 65000 IDs. The IDs can be passed as a comma separated string.
-    name str: Filter documents for a given name
-    createdafter int: Filter for documents which are created after a given UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
-    createdbefore int: Filter for documents which are created before a given UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
-    updatedafter int: Filter for documents which are updated after a given UNIX timestamp. The updatedafter filter only works when also using the parameters offset and limit.
-    updatedbefore int: Filter for documents which are updated before a given UNIX timestamp. The updatedbefore filter only works when also using the parameters offset and limit.
-    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs. The IDs are passed as a comma separated list.
-    withoutdocumentclass bool: Filters the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
-    mincharacters int: Filters the returned reference documents to include only documents that have a minimum of characters
-    metadata str: Filter documents for part of metadata, casing is ignored.
-    comment str: Filter documents for part of comment, casing is ignored.
-    sourcedoc bool: If true, then only source documents are returned.
-    sourcedocumentid str: Filter documents a specific source document.
-    offset int: Specify from which number on reference documents should be returned.
-    limit int: Specify the number of reference documents to be returned.
-    sort str: Define by which fields the returned reference documents are sorted. The following values can be sent as a comma-separated list: 'name', 'filename', 'metadata', 'created', 'updated', 'color', 'comment', 'derivedcolor', 'derivedcomment', 'documentclass'. Add a - before the field name to sort in descending order. Example: "documentclass,-created".
-    fields str: Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: 'id', 'name', 'tags', 'derivedtags', 'metadata', 'filename', 'created', 'processed', 'lang', 'updated, color, derivedcolor, comment, derivedcomment, documentclass, contentpreview'. If empty or null all fields will be returned. Example: "id,name,contentpreview,tags"
-        """
-        q_params = {}
-        if tags is not None:
-            q_params["tags"] = tags
-        if documentids is not None:
-            q_params["documentids"] = documentids
-        if name is not None:
-            q_params["name"] = name
-        if createdafter is not None:
-            q_params["createdafter"] = createdafter
-        if createdbefore is not None:
-            q_params["createdbefore"] = createdbefore
-        if updatedafter is not None:
-            q_params["updatedafter"] = updatedafter
-        if updatedbefore is not None:
-            q_params["updatedbefore"] = updatedbefore
-        if documentclassids is not None:
-            q_params["documentclassids"] = documentclassids
-        if withoutdocumentclass is not None:
-            q_params["withoutdocumentclass"] = withoutdocumentclass
-        if mincharacters is not None:
-            q_params["mincharacters"] = mincharacters
-        if metadata is not None:
-            q_params["metadata"] = metadata
-        if comment is not None:
-            q_params["comment"] = comment
-        if sourcedoc is not None:
-            q_params["sourcedoc"] = sourcedoc
-        if sourcedocumentid is not None:
-            q_params["sourcedocumentid"] = sourcedocumentid
-        if offset is not None:
-            q_params["offset"] = offset
-        if limit is not None:
-            q_params["limit"] = limit
-        if sort is not None:
-            q_params["sort"] = sort
-        if fields is not None:
-            q_params["fields"] = fields
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.XLSX)).execute().as_bytesio()
-
-    def post(
-        self,
-        name: str = None,
-        tags: str = None,
-        metadata: str = None,
-        file: IOBase = None,
-        text: str = None,
-        documenttype: str = None,
-        color: str = None,
-        comment: str = None,
-        documentclassid: str = None,
-        addparagraphsasdocuments: bool = None,
-        detectlanguage: bool = None,
-    ) -> List[DocumentInformation]:
-        """
-        Add a reference document a.k.a. library item.
-        Args:
-        name (str): The document name in your library (in contrast to the file name being used during upload).
-    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    metadata (str): Filter by metadata
-    file (IOBase): Input document (left document).
-    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
-    comment (str): Use this parameter to add a comment to your reference document.
-    documentclassid (str): List of documentclass ID for the target. The limit here is 1 ID.
-    addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
-        """
-        q_params = {}
-        if detectlanguage is not None:
-            q_params["detectlanguage"] = detectlanguage
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "name": name,
-                "tags": tags,
-                "metadata": metadata,
-                "file": file,
-                "text": text,
-                "documenttype": documenttype,
-                "color": color,
-                "comment": comment,
-                "documentclassid": documentclassid,
-                "addparagraphsasdocuments": addparagraphsasdocuments,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(DocumentInformationSchema)
-
-    def patch(
-        self,
-        body: List[DocumentInformation]
-    ) -> None:
-        """
-        Update metadata of multiple reference documents. Needs roles: 'Domain Admin' or 'Expert User'
-        """
-        return self._session.patch(
-            url=self._endpoint,
-            json=DocumentInformationSchema().dump(body, many=True)
-        ).execute().as_none()
-
-    def delete(
-        self,
-    ) -> None:
-        """
-        Delete all reference documents. Needs roles: 'Domain Admin' or 'Expert User'
-        """
-        self._session.delete(
-            url=self._endpoint,
-        ).execute()
-
+            Without "offset" and "limit" parameter, data can be filtered only by "tags" and "documentclassids".
+        Args:
+        tags str: List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    documentids str: List of document Ids for target. The limit here is 65000 IDs. The IDs can be passed as a comma separated string.
+    name str: Filter documents for a given name
+    createdafter int: Filter for documents which are created after a given UNIX timestamp. The createdafter filter only works when also using the parameters offset and limit.
+    createdbefore int: Filter for documents which are created before a given UNIX timestamp. The createdbefore filter only works when also using the parameters offset and limit.
+    updatedafter int: Filter for documents which are updated after a given UNIX timestamp. The updatedafter filter only works when also using the parameters offset and limit.
+    updatedbefore int: Filter for documents which are updated before a given UNIX timestamp. The updatedbefore filter only works when also using the parameters offset and limit.
+    documentclassids str: List of documentclass IDs for the target. The limit here is 1000 IDs. The IDs are passed as a comma separated list.
+    withoutdocumentclass bool: Filters the returned reference documents to include only documents that are not linked to a documentclass. The parameter is of type boolean and is set to false by default.
+    mincharacters int: Filters the returned reference documents to include only documents that have a minimum of characters
+    metadata str: Filter documents for part of metadata, casing is ignored.
+    comment str: Filter documents for part of comment, casing is ignored.
+    sourcedoc bool: If true, then only source documents are returned.
+    sourcedocumentid str: Filter documents a specific source document.
+    offset int: Specify from which number on reference documents should be returned.
+    limit int: Specify the number of reference documents to be returned.
+    sort str: Define by which fields the returned reference documents are sorted. The following values can be sent as a comma-separated list: 'name', 'filename', 'metadata', 'created', 'updated', 'color', 'comment', 'derivedcolor', 'derivedcomment', 'documentclass'. Add a - before the field name to sort in descending order. Example: "documentclass,-created".
+    fields str: Define which fields should be returned by the /referencedocuments endpoints. The following values can be sent as a comma-separated list: 'id', 'name', 'tags', 'derivedtags', 'metadata', 'filename', 'created', 'processed', 'lang', 'updated, color, derivedcolor, comment, derivedcomment, documentclass, contentpreview'. If empty or null all fields will be returned. Example: "id,name,contentpreview,tags"
+        """
+        q_params = {}
+        if tags is not None:
+            q_params["tags"] = tags
+        if documentids is not None:
+            q_params["documentids"] = documentids
+        if name is not None:
+            q_params["name"] = name
+        if createdafter is not None:
+            q_params["createdafter"] = createdafter
+        if createdbefore is not None:
+            q_params["createdbefore"] = createdbefore
+        if updatedafter is not None:
+            q_params["updatedafter"] = updatedafter
+        if updatedbefore is not None:
+            q_params["updatedbefore"] = updatedbefore
+        if documentclassids is not None:
+            q_params["documentclassids"] = documentclassids
+        if withoutdocumentclass is not None:
+            q_params["withoutdocumentclass"] = withoutdocumentclass
+        if mincharacters is not None:
+            q_params["mincharacters"] = mincharacters
+        if metadata is not None:
+            q_params["metadata"] = metadata
+        if comment is not None:
+            q_params["comment"] = comment
+        if sourcedoc is not None:
+            q_params["sourcedoc"] = sourcedoc
+        if sourcedocumentid is not None:
+            q_params["sourcedocumentid"] = sourcedocumentid
+        if offset is not None:
+            q_params["offset"] = offset
+        if limit is not None:
+            q_params["limit"] = limit
+        if sort is not None:
+            q_params["sort"] = sort
+        if fields is not None:
+            q_params["fields"] = fields
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.XLSX)).execute().as_bytesio()
+
+    def post(
+        self,
+        name: str = None,
+        tags: str = None,
+        metadata: str = None,
+        file: IOBase = None,
+        text: str = None,
+        documenttype: str = None,
+        color: str = None,
+        comment: str = None,
+        documentclassid: str = None,
+        addparagraphsasdocuments: bool = None,
+        detectlanguage: bool = None,
+    ) -> List[DocumentInformation]:
+        """
+        Add a reference document a.k.a. library item.
+        Args:
+        name (str): The document name in your library (in contrast to the file name being used during upload).
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    metadata (str): Filter by metadata
+    file (IOBase): Input document (left document).
+    text (str): Plain text input (left document). If set, the parameter `file` will be ignored.
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    color (str): Use this parameter to specify the color for your reference document. Possible values are RED, MAGENTA, AQUA, ORANGE, GREY, or LAVENDER.
+    comment (str): Use this parameter to add a comment to your reference document.
+    documentclassid (str): List of documentclass ID for the target. The limit here is 1 ID.
+    addparagraphsasdocuments (bool): Use this parameter to create individual reference documents in the library for each paragraph in your document. The parameter is of type boolean and is set to false by default.
+        """
+        q_params = {}
+        if detectlanguage is not None:
+            q_params["detectlanguage"] = detectlanguage
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "name": name,
+                "tags": tags,
+                "metadata": metadata,
+                "file": file,
+                "text": text,
+                "documenttype": documenttype,
+                "color": color,
+                "comment": comment,
+                "documentclassid": documentclassid,
+                "addparagraphsasdocuments": addparagraphsasdocuments,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(DocumentInformationSchema)
+    def post_json(
+        self,
+        body: List[Document] = None,
+        detectlanguage: bool = None,
+    ) -> List[DocumentInformation]:
+        """
+        Add a reference document a.k.a. library item.
+        Args:
+        body (List[Document]): 
+        """
+        q_params = {}
+        if detectlanguage is not None:
+            q_params["detectlanguage"] = detectlanguage
+        response = self._session.post(
+            url=self._endpoint,
+            json=DocumentSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(DocumentInformationSchema)
+
+    def patch(
+        self,
+        body: List[DocumentInformation]
+    ) -> None:
+        """
+        Update metadata of multiple reference documents. Needs roles: 'Domain Admin' or 'Expert User'
+        """
+        return self._session.patch(
+            url=self._endpoint,
+            json=DocumentInformationSchema().dump(body, many=True)
+        ).execute().as_none()
+
+    def delete(
+        self,
+    ) -> None:
+        """
+        Delete all reference documents. Needs roles: 'Domain Admin' or 'Expert User'
+        """
+        self._session.delete(
+            url=self._endpoint,
+        ).execute()
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/roles.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodelclass_instances.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class RolesEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/roles"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    def get(
-        self,
-    ) -> List[str]:
-        """
-        Get the role/s of the current user.
-        Args:
-            """
-        q_params = {}
-    
-        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().as_list()
-
-    
-    
-    
+from semantha_sdk.model.instance import Instance
+from semantha_sdk.model.instance import InstanceSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkmodelclassInstancesEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/instances"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    def get(
+        self,
+    ) -> List[Instance]:
+        """
+        Get all instances of the classes by class id
+            This is the quiet version of 'get /api/model/domains/{domainname}/classes/{id}/instances'
+        Args:
+            """
+        q_params = {}
+    
+        return self._session.get(self._endpoint, q_params=q_params, headers=RestClient.to_header(MediaType.JSON)).execute().to(InstanceSchema)
+
+    
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/sentence.py` & `semantha_sdk-6.9.0/semantha_sdk/api/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/sentences.py` & `semantha_sdk-6.9.0/semantha_sdk/api/sentences.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/settings.py` & `semantha_sdk-6.9.0/semantha_sdk/api/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/similaritymatrix.py` & `semantha_sdk-6.9.0/semantha_sdk/api/similaritymatrix.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-from io import IOBase
-from semantha_sdk.api.similaritymatrix_cluster import SimilaritymatrixClusterEndpoint
-from semantha_sdk.model.matrix_row import MatrixRow
-from semantha_sdk.model.matrix_row import MatrixRowSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class SimilaritymatrixEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/similaritymatrix"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-        self.__cluster = SimilaritymatrixClusterEndpoint(session, self._endpoint)
-    
-    @property
-    def cluster(self) -> SimilaritymatrixClusterEndpoint:
-        return self.__cluster
-
-    
-    def post(
-        self,
-        file: IOBase = None,
-        tags: str = None,
-        sourcetags: str = None,
-        documentids: List[str] = None,
-        sourcedocumentids: List[str] = None,
-        documentclassids: List[str] = None,
-        sourcedocumentclassids: List[str] = None,
-        similaritythreshold: float = None,
-        mode: str = None,
-        documenttype: str = None,
-        considertexttype: bool = None,
-    ) -> List[MatrixRow]:
-        """
-        Get a similarity matrix
-        Args:
-        file (IOBase): Input document (left document).
-    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
-    sourcetags (str): Filters the input library by tags
+from io import IOBase
+from semantha_sdk.api.similaritymatrix_cluster import SimilaritymatrixClusterEndpoint
+from semantha_sdk.model.matrix_row import MatrixRow
+from semantha_sdk.model.matrix_row import MatrixRowSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class SimilaritymatrixEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/similaritymatrix"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+        self.__cluster = SimilaritymatrixClusterEndpoint(session, self._endpoint)
+    
+    @property
+    def cluster(self) -> SimilaritymatrixClusterEndpoint:
+        return self.__cluster
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+        tags: str = None,
+        sourcetags: str = None,
+        documentids: List[str] = None,
+        sourcedocumentids: List[str] = None,
+        documentclassids: List[str] = None,
+        sourcedocumentclassids: List[str] = None,
+        similaritythreshold: float = None,
+        mode: str = None,
+        documenttype: str = None,
+        considertexttype: bool = None,
+    ) -> List[MatrixRow]:
+        """
+        Get a similarity matrix
+        Args:
+        file (IOBase): Input document (left document).
+    tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+    sourcetags (str): Filters the input library by tags
     documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
-            The IDs are passed as a JSON array.
+            The IDs are passed as a JSON array.
     sourcedocumentids (List[str]): List of document IDs for source. The limit here is 65000 IDs.
-            The IDs are passed as a JSON array.
+            The IDs are passed as a JSON array.
     documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
             The IDs are passed as a JSON array.
-            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
     sourcedocumentclassids (List[str]): List of documentclass IDs for the source. The limit here is 1000 IDs.
-            The IDs are passed as a JSON array.
+            The IDs are passed as a JSON array.
     similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-            In general, the higher the threshold, the more precise the results.
+            In general, the higher the threshold, the more precise the results.
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
-    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-                "tags": tags,
-                "sourcetags": sourcetags,
-                "documentids": documentids,
-                "sourcedocumentids": sourcedocumentids,
-                "documentclassids": documentclassids,
-                "sourcedocumentclassids": sourcedocumentclassids,
-                "similaritythreshold": similaritythreshold,
-                "mode": mode,
-                "documenttype": documenttype,
-                "considertexttype": considertexttype,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(MatrixRowSchema)
-
-    
-    
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    documenttype (str): Specifies the document type that is to be used by semantha when reading the uploaded document.
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+                "tags": tags,
+                "sourcetags": sourcetags,
+                "documentids": documentids,
+                "sourcedocumentids": sourcedocumentids,
+                "documentclassids": documentclassids,
+                "sourcedocumentclassids": sourcedocumentclassids,
+                "similaritythreshold": similaritythreshold,
+                "mode": mode,
+                "documenttype": documenttype,
+                "considertexttype": considertexttype,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(MatrixRowSchema)
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/similaritymatrix_cluster.py` & `semantha_sdk-6.9.0/semantha_sdk/api/similaritymatrix_cluster.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,90 @@
-from semantha_sdk.model.matrix_row import MatrixRow
-from semantha_sdk.model.matrix_row import MatrixRowSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class SimilaritymatrixClusterEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/cluster"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post(
-        self,
-        tags: str = None,
-        documentids: List[str] = None,
-        documentclassids: List[str] = None,
-        similaritythreshold: float = None,
-        mode: str = None,
-        considertexttype: bool = None,
-    ) -> List[MatrixRow]:
-        """
+from semantha_sdk.model.matrix_row import MatrixRow
+from semantha_sdk.model.matrix_row import MatrixRowSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class SimilaritymatrixClusterEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/cluster"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        tags: str = None,
+        documentids: List[str] = None,
+        documentclassids: List[str] = None,
+        similaritythreshold: float = None,
+        mode: str = None,
+        considertexttype: bool = None,
+    ) -> List[MatrixRow]:
+        """
         Get document clusters
-            Consolidate the documents to clusters based on the results of `post post /api/domains/{domainname}/similaritymatrix`
-        Args:
-        tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+            Consolidate the documents to clusters based on the results of `post post /api/domains/{domainname}/similaritymatrix`
+        Args:
+        tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
     documentids (List[str]): List of document Ids for target. The limit here is 65000 IDs.
-            The IDs are passed as a JSON array.
+            The IDs are passed as a JSON array.
     documentclassids (List[str]): List of documentclass IDs for the target. The limit here is 1000 IDs.
             The IDs are passed as a JSON array.
-            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+            This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
     similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
-            In general, the higher the threshold, the more precise the results.
+            In general, the higher the threshold, the more precise the results.
     mode (str): When using the references endpoint: Use mode to determine the type of search semantha should perform. 
             fingerprint: semantic search based on sentences; 
             keyword: keyword: search based on sentences; 
             document: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. Higher scores indicate higher similarity. Please note that the similarity score has no upper limit and is not normalized; 
             document_fingerprint: a bag-of-words search that ranks a set of documents based on the query terms appearing in each document, regardless of their proximity within the document. The results are then reranked based on a semantic search. This reranking results in normalized scores and as such represents an enhancement of the mode document; 
             fingerprint_keyword (formerly auto): semantic search, if no results are found a keyword search is performed
-            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
-    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "tags": tags,
-                "documentids": documentids,
-                "documentclassids": documentclassids,
-                "similaritythreshold": similaritythreshold,
-                "mode": mode,
-                "considertexttype": considertexttype,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(MatrixRowSchema)
-
-    
-    
+            Creating document model: It also defines what structure should be considered for what operator (similarity or extraction).
+    considertexttype (bool): Use this parameter to ensure that only paragraphs of the same type are compared with each other. The parameter is of type boolean and is set to false by default.
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "tags": tags,
+                "documentids": documentids,
+                "documentclassids": documentclassids,
+                "similaritythreshold": similaritythreshold,
+                "mode": mode,
+                "considertexttype": considertexttype,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(MatrixRowSchema)
+    def post_json(
+        self,
+        body: List[MatrixRow] = None,
+    ) -> List[MatrixRow]:
+        """
+        Get document clusters
+            Consolidate the documents to clusters based on the results of `post post /api/domains/{domainname}/similaritymatrix`
+        Args:
+        body (List[MatrixRow]): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=MatrixRowSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(MatrixRowSchema)
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/summarizations.py` & `semantha_sdk-6.9.0/semantha_sdk/api/bulkmodel_boostwords.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,45 @@
-from semantha_sdk.model.summarization import Summarization
-from semantha_sdk.model.summarization import SummarizationSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-from typing import List
-
-class SummarizationsEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/summarizations"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post(
-        self,
-        texts: List[str] = None,
-        topic: str = None,
-        language: str = None,
-    ) -> Summarization:
-        """
-        Generates a summary for given number of texts. If topic is supplied summarization is generated for this topic
-        Args:
-        texts (List[str]): 
-    topic (str): 
-    language (str): 
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "texts": texts,
-                "topic": topic,
-                "language": language,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(SummarizationSchema)
-
-    
-    
+from semantha_sdk.model.boost_word import BoostWord
+from semantha_sdk.model.boost_word import BoostWordSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+from typing import List
+
+class BulkmodelBoostwordsEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/boostwords"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        body: List[BoostWord] = None,
+    ) -> None:
+        """
+        Create one or more boostwords
+            This is the quiet version of  'post /api/domains/{domainname}/boostwords'
+        Args:
+        body (List[BoostWord]): 
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=BoostWordSchema().dump(body, many=True),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.as_none()
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/tag.py` & `semantha_sdk-6.9.0/semantha_sdk/api/tag.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/transactions.py` & `semantha_sdk-6.9.0/semantha_sdk/api/transactions.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/api/validation.py` & `semantha_sdk-6.9.0/semantha_sdk/api/validation.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from io import IOBase
-from semantha_sdk.model.semantic_model import SemanticModel
-from semantha_sdk.model.semantic_model import SemanticModelSchema
-from semantha_sdk.rest.rest_client import MediaType
-from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
-
-class ValidationEndpoint(RestEndpoint):
-    """ author semantha, this is a generated class do not change manually! 
-    
-    """
-
-    @property
-    def _endpoint(self) -> str:
-        return self._parent_endpoint + "/validation"
-
-    def __init__(
-        self,
-        session: RestClient,
-        parent_endpoint: str,
-    ) -> None:
-        super().__init__(session, parent_endpoint)
-
-    
-    def post(
-        self,
-        file: IOBase = None,
-    ) -> SemanticModel:
-        """
+from io import IOBase
+from semantha_sdk.model.semantic_model import SemanticModel
+from semantha_sdk.model.semantic_model import SemanticModelSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient, RestEndpoint
+
+class ValidationEndpoint(RestEndpoint):
+    """ author semantha, this is a generated class do not change manually! 
+    
+    """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/validation"
+
+    def __init__(
+        self,
+        session: RestClient,
+        parent_endpoint: str,
+    ) -> None:
+        super().__init__(session, parent_endpoint)
+
+    
+    def post(
+        self,
+        file: IOBase = None,
+    ) -> SemanticModel:
+        """
         Validate existing data in a document
-            The coordinates come back, if data is found
-        Args:
-        file (IOBase): Input document (left document).
-        """
-        q_params = {}
-        response = self._session.post(
-            url=self._endpoint,
-            body={
-                "file": file,
-            },
-            headers=RestClient.to_header(MediaType.JSON),
-            q_params=q_params
-        ).execute()
-        return response.to(SemanticModelSchema)
-
-    
-    
+            The coordinates come back, if data is found
+        Args:
+        file (IOBase): Input document (left document).
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            body={
+                "file": file,
+            },
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(SemanticModelSchema)
+
+    
+
```

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/__init__.py` & `semantha_sdk-6.9.0/semantha_sdk/model/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/annotation_cell.py` & `semantha_sdk-6.9.0/semantha_sdk/model/annotation_cell.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/annotation_page.py` & `semantha_sdk-6.9.0/semantha_sdk/model/annotation_page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/answer.py` & `semantha_sdk-6.9.0/semantha_sdk/model/answer.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/argument.py` & `semantha_sdk-6.9.0/semantha_sdk/model/argument.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/attribute.py` & `semantha_sdk-6.9.0/semantha_sdk/model/attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/boost_word.py` & `semantha_sdk-6.9.0/semantha_sdk/model/boost_word.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/class_bulk.py` & `semantha_sdk-6.9.0/semantha_sdk/model/class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/classes_overview.py` & `semantha_sdk-6.9.0/semantha_sdk/model/classes_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/clazz.py` & `semantha_sdk-6.9.0/semantha_sdk/model/clazz.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/clustered_document.py` & `semantha_sdk-6.9.0/semantha_sdk/model/clustered_document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/clustering_response.py` & `semantha_sdk-6.9.0/semantha_sdk/model/clustering_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/complex_property.py` & `semantha_sdk-6.9.0/semantha_sdk/model/complex_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/condition.py` & `semantha_sdk-6.9.0/semantha_sdk/model/condition.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/condition_value.py` & `semantha_sdk-6.9.0/semantha_sdk/model/condition_value.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/data_property.py` & `semantha_sdk-6.9.0/semantha_sdk/model/data_property.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_class.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_class_bulk.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_class_bulk.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_class_node.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_class_node.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_cluster.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_cluster.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_information.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_type.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_type.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_type_change.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_type_change.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/document_type_config.py` & `semantha_sdk-6.9.0/semantha_sdk/model/document_type_config.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/expression.py` & `semantha_sdk-6.9.0/semantha_sdk/model/expression.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/extraction_area.py` & `semantha_sdk-6.9.0/semantha_sdk/model/extraction_area.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/extraction_file.py` & `semantha_sdk-6.9.0/semantha_sdk/model/extraction_file.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/extractor.py` & `semantha_sdk-6.9.0/semantha_sdk/model/extractor.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/extractor_attribute.py` & `semantha_sdk-6.9.0/semantha_sdk/model/extractor_attribute.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/extractor_class.py` & `semantha_sdk-6.9.0/semantha_sdk/model/extractor_class.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/extractor_class_overview.py` & `semantha_sdk-6.9.0/semantha_sdk/model/extractor_class_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/features.py` & `semantha_sdk-6.9.0/semantha_sdk/model/features.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/instance.py` & `semantha_sdk-6.9.0/semantha_sdk/model/instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/instance_overview.py` & `semantha_sdk-6.9.0/semantha_sdk/model/instance_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/linked_instance.py` & `semantha_sdk-6.9.0/semantha_sdk/model/linked_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/matrix_row.py` & `semantha_sdk-6.9.0/semantha_sdk/model/matrix_row.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/model_instance.py` & `semantha_sdk-6.9.0/semantha_sdk/model/model_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/page.py` & `semantha_sdk-6.9.0/semantha_sdk/model/page.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/paragraph.py` & `semantha_sdk-6.9.0/semantha_sdk/model/paragraph.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/process_information.py` & `semantha_sdk-6.9.0/semantha_sdk/model/process_information.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/reference.py` & `semantha_sdk-6.9.0/semantha_sdk/model/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/reference_documents_response_container.py` & `semantha_sdk-6.9.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/relation.py` & `semantha_sdk-6.9.0/semantha_sdk/model/relation.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/response_meta_info.py` & `semantha_sdk-6.9.0/semantha_sdk/model/response_meta_info.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/rule.py` & `semantha_sdk-6.9.0/semantha_sdk/model/rule.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/rule_function.py` & `semantha_sdk-6.9.0/semantha_sdk/model/rule_function.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/rule_overview.py` & `semantha_sdk-6.9.0/semantha_sdk/model/rule_overview.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/semantic_model.py` & `semantha_sdk-6.9.0/semantha_sdk/model/semantic_model.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/sentence.py` & `semantha_sdk-6.9.0/semantha_sdk/model/sentence.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/settings.py` & `semantha_sdk-6.9.0/semantha_sdk/model/settings.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/smart_cluster_response_container.py` & `semantha_sdk-6.9.0/semantha_sdk/model/smart_cluster_response_container.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py` & `semantha_sdk-6.9.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/statistic.py` & `semantha_sdk-6.9.0/semantha_sdk/model/statistic.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/synonym.py` & `semantha_sdk-6.9.0/semantha_sdk/model/synonym.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/model/table_instance.py` & `semantha_sdk-6.9.0/semantha_sdk/model/table_instance.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/rest/rest_client.py` & `semantha_sdk-6.9.0/semantha_sdk/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/__init__.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/compare/__init__.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/compare/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/customization.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/customization.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/domain/__init__.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/__init__.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/document.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/document.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/documentiter.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/documentiter.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/documenttags.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/documenttags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/metadata.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/metadata.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/reference.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/reference.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/library/tags.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/library/tags.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/ranking/hybrid.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/ranking/hybrid.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/semantha_sdk/semantha/ranking/sparse.py` & `semantha_sdk-6.9.0/semantha_sdk/semantha/ranking/sparse.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-6.8.0/PKG-INFO` & `semantha_sdk-6.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 6.8.0
+Version: 6.9.0
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
@@ -135,14 +135,23 @@
 annotated_pdf = api.domains(domain).documentannotations.post_as_pdf(file=pdf, similaritythreshold=0.85)
 with open('annotated.pdf', 'wb') as annotated_file:
     annotated_file.write(annotated_pdf.getbuffer())
 ```
 
 # Changelog for the Python SDK for the semantha platform
 
+## [6.9.0] 2024-02-23
+### Added
+Added implementation method "post_json" for "overloaded" services where we have content type multipart/form-data as well as application/json: 
+ - **/bulk/domains/{domainname}/referencedocuments** **POST**
+ - **/domains/{domainname}/modelinstances** **POST**
+ - **/domains/{domainname}/referencedocuments** **POST**
+ - **/domains/{domainname}/similaritymatrix/cluster** **POST**
+
+
 ## [6.8.0] 2024-02-09
 ### Removed
 - Removed two setting values: similarity_matcher and similarity_threshold for endpoint: **/domains/{domainname}/settings** **GET**
 
 ### Improved
 - More method and parameter comments
 - Endpoint **/domains** **GET** returns DomainInfo object now instead of Domain
@@ -288,14 +297,15 @@
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/documenttypes** -> BulkdomainsDocumenttypesEndpoint
     - [x] **GET** -> List[DocumentType]
     - [x] **POST** -> None
 - [x] **/bulk/domains/{domainname}/referencedocuments** -> BulkdomainsReferencedocumentsEndpoint
     - [x] **GET** -> List[Document]
     - [x] **POST** -> None
+    - [x] **POST** -> None
     - [x] **DELETE** -> None
 - [x] **/bulk/domains/{domainname}/references** -> BulkdomainsReferencesEndpoint
     - [x] **POST** -> List[Document]
 - [x] **/bulk/model** -> BulkModelEndpoint
 - [x] **/bulk/model/domains** -> BulkmodelDomainsEndpoint
 - [x] **/bulk/model/domains/{domainname}** -> BulkmodelDomainEndpoint
 - [x] **/bulk/model/domains/{domainname}/boostwords** -> BulkmodelBoostwordsEndpoint
@@ -375,19 +385,21 @@
     - [x] **PATCH** -> DocumentType
 - [x] **/domains/{domainname}/documenttypes/{id}/clone** -> CloneEndpoint
     - [x] **POST** -> DocumentType
 - [x] **/domains/{domainname}/modelclasses** -> ModelclassesEndpoint
     - [x] **GET** -> List[ModelClass]
 - [x] **/domains/{domainname}/modelinstances** -> ModelinstancesEndpoint
     - [x] **POST** -> SemanticModel
+    - [x] **POST** -> SemanticModel
     - [x] **POST** (Accept: xlsx) -> IOBase
 - [x] **/domains/{domainname}/referencedocuments** -> ReferencedocumentsEndpoint
     - [x] **GET** -> ReferenceDocumentsResponseContainer
     - [x] **GET** (Accept: xlsx) -> IOBase
     - [x] **POST** -> List[DocumentInformation]
+    - [x] **POST** -> List[DocumentInformation]
     - [x] **DELETE** -> None
     - [x] **PATCH** -> None
 - [x] **/domains/{domainname}/referencedocuments/clusters** -> ClustersEndpoint
     - [x] **GET** -> SmartClusterResponseContainer
     - [x] **PUT** -> SmartClusterResponseContainer
 - [x] **/domains/{domainname}/referencedocuments/namedentities** -> NamedentitiesEndpoint
     - [x] **GET** -> List[DocumentNamedEntity]
@@ -413,14 +425,15 @@
 - [x] **/domains/{domainname}/settings** -> SettingsEndpoint
     - [x] **GET** -> Settings
     - [x] **PATCH** -> Settings
 - [x] **/domains/{domainname}/similaritymatrix** -> SimilaritymatrixEndpoint
     - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/similaritymatrix/cluster** -> SimilaritymatrixClusterEndpoint
     - [x] **POST** -> List[MatrixRow]
+    - [x] **POST** -> List[MatrixRow]
 - [x] **/domains/{domainname}/summarizations** -> SummarizationsEndpoint
     - [x] **POST** -> Summarization
 - [x] **/domains/{domainname}/tags** -> TagsEndpoint
     - [x] **GET** -> List[str]
 - [x] **/domains/{domainname}/tags/{tagname}** -> TagEndpoint
 - [x] **/domains/{domainname}/tags/{tagname}/referencedocuments** -> TagReferencedocumentsEndpoint
     - [x] **GET** -> List[DocumentInformation]
```

