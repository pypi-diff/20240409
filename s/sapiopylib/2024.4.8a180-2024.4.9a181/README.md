# Comparing `tmp/sapiopylib-2024.4.8a180.tar.gz` & `tmp/sapiopylib-2024.4.9a181.tar.gz`

## Comparing `sapiopylib-2024.4.8a180.tar` & `sapiopylib-2024.4.9a181.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0    13219 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/ClientCallbackService.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataService.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/MessengerService.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/ReportManager.py
--rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Message.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/field_set.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/protocol_template.py
--rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/autopaging.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recorddatasinks.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    28790 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/ancestry.py
--rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/properties.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/src/sapiopylib/utils/string.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/EmailAttachmentDataTest.py
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51536_test.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51549_test.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51551_test.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51635_test.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51821_test.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51846_test.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51847_test.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-51849_test.py
--rw-r--r--   0        0        0     8279 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/FR-52100_test.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51537_test.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51547.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51842_test.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51853_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51856_test.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/PR-51964_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/__init__.py
--rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/data_type_models.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/resources/NAC28735.fa
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/tests/resources/fr-51846.ssg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/LICENSE
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/README.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/pyproject.toml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.8a180/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0    13374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/ClientCallbackService.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataService.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/ReportManager.py
+-rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/field_set.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/protocol_template.py
+-rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/autopaging.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recorddatasinks.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    28845 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/ancestry.py
+-rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/properties.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/utils/string.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/EmailAttachmentDataTest.py
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51536_test.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51549_test.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51551_test.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51635_test.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51821_test.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51846_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51847_test.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51849_test.py
+-rw-r--r--   0        0        0     8917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-52100_test.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51537_test.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51547.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51842_test.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51853_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51856_test.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51964_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/__init__.py
+-rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/data_type_models.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/resources/NAC28735.fa
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/resources/fr-51846.ssg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/LICENSE
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/pyproject.toml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/PKG-INFO
```

### Comparing `sapiopylib-2024.4.8a180/INSTALL.md` & `sapiopylib-2024.4.9a181/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/ClientCallbackService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/ClientCallbackService.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import re
 from enum import Enum
 from typing import Any, Callable, IO, cast
 from weakref import WeakValueDictionary
 
+from sapiopylib.rest.pojo.DataRecord import DataRecord
+
 from sapiopylib.rest.pojo.webhook.ClientCallbackResult import InputSelectionResult, ClientCallbackResultParser
 
 from sapiopylib.rest.pojo.webhook.ClientCallbackRequest import FilePromptRequest, DisplayPopupRequest, \
     MultiFilePromptRequest, DataRecordSelectionRequest, TableEntryDialogRequest, DataRecordDialogRequest, \
     FormEntryDialogRequest, ListDialogRequest, OptionDialogRequest, InputSelectionRequest
 
 from sapiopylib.rest.User import SapioUser
@@ -213,21 +215,24 @@
         :return: the index of the button that the user choose or {@code null} if the user cancelled the dialog.
         """
         url = '/clientcallback/custombuttondialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
         return self.user.get_json_data_or_none(response)
 
-    def show_input_selection_dialog(self, request: InputSelectionRequest) -> InputSelectionResult | None:
+    def show_input_selection_dialog(self, request: InputSelectionRequest) -> list[DataRecord] | None:
         """
         Shows an input-selection dialog with configurations for enabling tabs for tree navigation, reports, and quick search.
         Allows the user to select records using the dialog and returns their selection to the user.
         :param request: The request defining the options for the dialog
         :return: A list of the selected data records.  If no records are selected, an empty list is returned.  If the user cancels the dialog, then None will be returned.
         """
         url = '/clientcallback/inputselectiondialog'
         response = self.user.post(url, payload=request.to_json())
         self.user.raise_for_status(response)
         json = self.user.get_json_data_or_none(response)
         if not json:
             return None
-        return cast(InputSelectionResult, ClientCallbackResultParser.parse_client_callback_result(json))
+        result = cast(InputSelectionResult, ClientCallbackResultParser.parse_client_callback_result(json))
+        if result.user_cancelled:
+            return None
+        return result.selected_record_list
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/MessengerService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/MessengerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/ReportManager.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/ReportManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/User.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,17 @@
         return self.__original_fields.get(field_name)
 
     def __str__(self):
         if self.__fields is not None and 'DataRecordName' in self.__fields:
             return self.__fields.get("DataRecordName")
         return self.__data_type_name + " " + str(self.__record_id)
 
+    def __repr__(self):
+        return self.__str__()
+
     @staticmethod
     def from_json(json_dct: Dict[str, Any]) -> Optional[DataRecord]:
         if json_dct is None:
             return None
         data_type_name = json_dct.get('dataTypeName')
         record_id = json_dct.get('recordId')
         fields = json_dct.get('fields')
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Message.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Message.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/field_set.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/field_set.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/eln/protocol_template.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/protocol_template.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,16 +239,18 @@
             user_response_data_list: Optional[List[Dict[str, Any]]] = \
                 json_dct.get('userResponseDataList')
             return TableEntryDialogResult(user_cancelled, callback_context_data,
                                           user_response_data_list=user_response_data_list)
         elif callback_type == CallbackType.WRITE_FILE:
             return WriteFileResult(user_cancelled, callback_context_data)
         elif callback_type == CallbackType.INPUT_SELECTION:
-            selected_record_list: list[DataRecord] = \
-                [DataRecord.from_json(x) for x in json_dct.get('selectedDataRecordList')]
+            selected_record_list: list[DataRecord] = []
+            selected_records_json = json_dct.get('selectedDataRecordList')
+            if selected_records_json:
+                selected_record_list = [DataRecord.from_json(x) for x in selected_records_json]
             return InputSelectionResult(user_cancelled, callback_context_data,
                                         selected_record_list)
         elif callback_type == CallbackType.DATA_RECORD_DIALOG:
             dialog_result: bool = json_dct.get('dialogResult')
             return DataRecordDialogResponse(user_cancelled, callback_context_data,
                                             dialog_result)
         else:
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,21 +24,51 @@
 
 
 class SapioWebhookContext:
     """
     The webhook context structure after receiving a request from Sapio Informatics Platform.
 
     Obtain your context variables here.
+
+    Attributes:
+        user: The user object contains your session and credentials. Typically, this is an interactive session with client callback enabled.
+        data_record_manager: The convenient way to retrieve DataRecordManager class object directly without using DataMgmtServer.
+        eln_manager: The convenient way to retrieve ElnManager class object directly without using DataMgmtServer.
+        active_protocol: The current protocol in protocol/step interface. It can be None if there is none in the context.
+        active_step: The current step in protocol/step interface. It can be None if there is none in the context.
+        end_point_type: The invocation point of the current endpoint.
+        data_record: The current data record of the context. It can be None if not applicable.
+        base_data_record: The current base data record of the context. This usually is only relevant in IDV and temporary record views. It can be None if not applicable.
+        data_record_list: The list of data records of the context. It can be None if not applicable.
+        data_type_name: The data type name of the context. It can be None if not applicable.
+        data_field_name: The data field name of the context. It can be None if not applicable.
+        velox_on_save_result_map: on save rule result context. It can be None if not applicable.
+        velox_on_save_field_map_result_map: on save rule result context for any triggered records that is no longer accessible. That is, objects that are deleted or is rendered otherwise inaccessible to the user. It can be None if not applicable.
+        velox_eln_rule_result_map: eln rule result context. It can be None if not applicable.
+        velox_eln_rule_field_map_result_map: eln rule context for any triggered records that is no longer accessible. That is, objects that are deleted or is rendered otherwise inaccessible to the user. It can be None if not applicable.
+        experiment_entry_list: ELN experiment entry list context. It can be None if not applicable.
+        experiment_entry: ELN experiment entry context. It can be None if not applicable.
+        eln_experiment: ELN experiment context. It can be None if not applicable.
+        client_callback_result: DEPRECATED. USE CLIENT CALLBACK SERVICE INSTEAD.
+        is_client_callback_available: DEPRECATED. USE CLIENT CALLBACK SERVICE INSTEAD.
+        report_builder_template_populator_data: Report builder context. It can be None if not applicable.
+        field_map_list: list of field map data. It can be None if not applicable. Generally, this is only non-blank in searches and temporary contexts.
+        field_map: field map data. It can be None if not applicable. Generally, this is only non-blank in selection list plugins of temporary data types.
+        selected_field_map_index_list: A list of 0-based indexes to the field_map_list of user selections. It can be None if not applicable.
+        data_field_name_list: A list of data field names. It can be None if not applicable.
+        context_data: any additional carrying data, usually from client-side plugins or another plugin installed in BLS that triggers the webhook.
+        entry_position: ELN entry position data. It can be None if not applicable. This is only filled if there is position data but no ELN entry, such as the case for grabber context when ELN entry has not been created.
+        custom_report: The custom report object of the current context. It can be None if not applicable. This object can be decorated already by the client, and may not contain result data.
     """
     user: SapioUser
 
     data_record_manager: DataRecordManager
     eln_manager: ElnManager
     active_protocol: Optional[AbstractProtocol]
-    active_step: AbstractStep
+    active_step: Optional[AbstractStep]
 
     end_point_type: WebhookEndpointType
 
     data_record: Optional[DataRecord]
     base_data_record: Optional[DataRecord]
     data_record_list: Optional[List[DataRecord]]
     data_type_name: Optional[str]
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,27 @@
 from sapiopylib.rest.pojo.webhook.WebhookDirective import AbstractWebhookDirective
 
 
 class SapioWebhookResult:
     """
     Returned webhook result from webhook handler to sapio platform.
 
-    passed: Whether the handler had successfully handled request. "False" value may cause transaction to be rolled back.
-
-    display_text: If this is selection list populator handler, the possible values for user to select in selection list.
-
-    directive: Any place we will navigate player to after receiving this request.
-
-    client_callback_request: A popup request asking client for more information in UI.
-
-    refresh_data: Whether forces the client to refresh existing data in the page.
-
-    auto_invoke_next_row: Used only for action text plugin, whether to automatically shift to next row and trigger.
-
-    commit_message: If the webhook is transactional, the commit message to write when the entire webhook is committing.
-
-    refresh_notebook_experiment: If set to true, the client browser will refresh the entire notebook experiment.
-    This typically is not good user experience. Avoid if possible.
-
-    eln_entry_refresh_list: Provide a list of ELN entry to be refreshed in client browser after returning.
-
-    create_eln_snapshot: If set to true, a PDF snapshot will be generated at after returning the result.
-
-    include_entry_description_in_eln_snapshot: Whether to include ELN entry descriptions (usually help texts) in PDF.
+    Attributes:
+        passed: Whether the handler had successfully handled request. "False" value may cause transaction to be rolled back.
+        display_text: DEPRECATED. USE CLIENT CALLBACK SERVICE INSTEAD.
+        directive: Any place we will navigate player to after receiving this request.
+        client_callback_request: DEPRECATED. USE CLIENT CALLBACK SERVICE INSTEAD.
+        refresh_data: Whether forces the client to refresh existing data in the page.
+        auto_invoke_next_row: Used only for action text plugin, whether to automatically shift to next row and trigger.
+        commit_message: If the webhook is transactional, the commit message to write when the entire webhook is committing.
+        refresh_notebook_experiment: If set to true, the client browser will refresh the entire notebook experiment.
+        This typically is not good user experience. Avoid if possible.
+        eln_entry_refresh_list: Provide a list of ELN entry to be refreshed in client browser after returning.
+        create_eln_snapshot: If set to true, a PDF snapshot will be generated at after returning the result.
+        include_entry_description_in_eln_snapshot: Whether to include ELN entry descriptions (usually help texts) in PDF.
     """
     passed: bool
     display_text: Optional[str]
     list_values: Optional[List[str]]
     directive: Optional[AbstractWebhookDirective]
     client_callback_request: Optional[AbstractClientCallbackRequest]
     refresh_data: bool
@@ -57,34 +48,16 @@
                  report_builder_template_populator_data: Optional[RbTemplatePopulatorData] = None,
                  auto_invoke_next_row: bool = False, commit_message: Optional[str] = None,
                  refresh_notebook_experiment:bool = False,
                  eln_entry_refresh_list: Optional[List[ExperimentEntry]] = None,
                  create_eln_snapshot: bool = False,
                  include_entry_description_in_eln_snapshot: bool = False):
         """
-        Returned webhook result from webhook handler to sapio platform.
-
-        :param passed: Whether the handler had successfully handled request.
-        "False" value may cause transaction to be rolled back.
-
-        :param display_text: If this is selection list populator handler, the possible values for user to select in
-        selection list.
-
-        :param directive: Any place we will navigate player to after receiving this request.
-
-        :param client_callback_request: A popup request asking client for more information in UI.
-
-        :param refresh_data: Whether forces the client to refresh existing data in the page.
-
-        :param auto_invoke_next_row Whether the client should automatically invoke the plugin for this field on the next
-        row when viewing this field in a table of data.
-        This boolean is only relevant for the ActionTextField plugin point.
-
-        :param commit_message The commit message to be used when committing the transaction after the webhook completes.
-        Only relevant when webhook is configured as transactional.
+        The objects of this class should not be created by end users.
+        The library will create this object on initialization of webhook context.
         """
         self.passed = passed
         self.display_text = display_text
         self.list_values = list_values
         self.directive = directive
         self.client_callback_request = client_callback_request
         self.refresh_data = refresh_data
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/autopaging.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/autopaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recorddatasinks.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recorddatasinks.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,14 +180,17 @@
     _non_loaded_removed_children: Set[PyRecordModel]
     _non_loaded_removed_forward_links: Set[str]
     _non_loaded_removed_reverse_links: SetMultimap[RecordModelReverseSideLinkCacheKey, PyRecordModel]
 
     def __str__(self):
         return self.data_type_name + " " + str(self.record_id) + ": " + str(self.fields)
 
+    def __repr__(self):
+        return self.__str__()
+
     def __init__(self, backing_record: DataRecord, record_model_manager):
         self._backing_record = backing_record
         self._model_fields = RecordModelFieldMap(self, backing_record.get_fields())
         self._record_model_manager = record_model_manager
         self.__is_deleted = False
         self._children_types_loaded = set()
         self._parent_types_loaded = set()
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,17 @@
         if not isinstance(other, WrappedRecordModel):
             return False
         return self._backing_model == other._backing_model
 
     def __str__(self):
         return str(self._backing_model)
 
+    def __repr__(self):
+        return self.__str__()
+
     @property
     def backing_model(self):
         """
         The base model is the root model backing the decorated type.
         """
         return self._backing_model
```

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/ancestry.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/ancestry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/rest/utils/recordmodel/properties.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/properties.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/src/sapiopylib/utils/string.py` & `sapiopylib-2024.4.9a181/src/sapiopylib/utils/string.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/EmailAttachmentDataTest.py` & `sapiopylib-2024.4.9a181/tests/EmailAttachmentDataTest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51536_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51536_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51549_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51549_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51551_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51551_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51635_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51635_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51821_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51821_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51846_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51846_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51847_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51847_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-51849_test.py` & `sapiopylib-2024.4.9a181/tests/FR-51849_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/FR-52100_test.py` & `sapiopylib-2024.4.9a181/tests/FR-52100_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def run(self, context: SapioWebhookContext) -> SapioWebhookResult:
         user = context.user
         client_callback = DataMgmtServer.get_client_callback(user)
         selected_option: int | None = client_callback.show_option_dialog(OptionDialogRequest("Select Input Dialog Option",
                                                                "Please make a selection in one of these options to test ^_^.",
                                                                ['Abort', 'Field Entry', 'Table Entry', 'List', 'Record IDV', 'Record Selection',
-                                                                "Download", "Upload", "Upload Multiple"]))
+                                                                "Download", "Upload", "Upload Multiple", "Input Selection Search"]))
         if selected_option == 1:
             self.test_field_entry(context)
         elif selected_option == 2:
             self.test_table_entry(context)
         elif selected_option == 3:
             self.test_list(context)
         elif selected_option == 4:
@@ -47,14 +47,16 @@
             self.test_record_selection(context)
         elif selected_option == 6:
             self.test_download_file_to_user(context)
         elif selected_option == 7:
             self.test_upload_file_from_user(context)
         elif selected_option == 8:
             self.test_multi_upload_file_from_user(context)
+        elif selected_option == 9:
+            self.test_input_selection_search_from_user(context)
         return SapioWebhookResult(True)
 
     def test_field_entry(self, context):
         user = context.user
         client_callback = DataMgmtServer.get_client_callback(user)
         fb: FormBuilder = FormBuilder()
         fb.add_field(VeloxStringFieldDefinition(fb.get_data_type_name(), "Test1", "Test 1"))
@@ -142,14 +144,24 @@
         if not fake_file_path_list:
             return
         for fake_file_path in fake_file_path_list:
             sink = InMemoryStringDataSink(user)
             sink.consume_client_callback_file_path_data(fake_file_path)
             client_callback.display_info("Received file content for '" + fake_file_path + "':\n" + sink.text)
 
+    def test_input_selection_search_from_user(self, context):
+        user = context.user
+        client_callback = DataMgmtServer.get_client_callback(user)
+        result = client_callback.show_input_selection_dialog(InputSelectionRequest(data_type_name="Directory", dialog_message="Select One", multi_select=False))
+        if result is None:
+            client_callback.display_info("User did not select anything.")
+        else:
+            client_callback.display_info("User has selected: " + str(result))
+
+
 
 config: WebhookConfiguration = WebhookConfiguration(verify_sapio_cert=False, debug=True)
 config.register('/display_info_test', TestDisplayInfo)
 config.register('/dialog_test', TestUserInputDialogs)
 
 app = WebhookServerFactory.configure_flask_app(app=None, config=config)
 app.run(host="0.0.0.0", port=8099)
```

### Comparing `sapiopylib-2024.4.8a180/tests/PR-51537_test.py` & `sapiopylib-2024.4.9a181/tests/PR-51537_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/PR-51547.py` & `sapiopylib-2024.4.9a181/tests/PR-51547.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/PR-51842_test.py` & `sapiopylib-2024.4.9a181/tests/PR-51842_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/PR-51853_test.py` & `sapiopylib-2024.4.9a181/tests/PR-51853_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/PR-51856_test.py` & `sapiopylib-2024.4.9a181/tests/PR-51856_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/PR-51964_test.py` & `sapiopylib-2024.4.9a181/tests/PR-51964_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/data_type_models.py` & `sapiopylib-2024.4.9a181/tests/data_type_models.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/resources/NAC28735.fa` & `sapiopylib-2024.4.9a181/tests/resources/NAC28735.fa`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/tests/resources/fr-51846.ssg` & `sapiopylib-2024.4.9a181/tests/resources/fr-51846.ssg`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/LICENSE` & `sapiopylib-2024.4.9a181/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/README.md` & `sapiopylib-2024.4.9a181/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.8a180/pyproject.toml` & `sapiopylib-2024.4.9a181/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2024.04.08a180'
+version='2024.04.09a181'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sapiopylib-2024.4.8a180/PKG-INFO` & `sapiopylib-2024.4.9a181/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopylib
-Version: 2024.4.8a180
+Version: 2024.4.9a181
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.8a180 Summary: Official
+Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.9a181 Summary: Official
 Sapio Informatics Platform Python API Project-URL: Homepage, https://
 github.com/sapiosciences Project-URL: Bug Tracker, https://github.com/
 sapiosciences/sapio-py-tutorials/issues Author-email: Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

