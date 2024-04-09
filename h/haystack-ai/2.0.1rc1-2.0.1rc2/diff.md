# Comparing `tmp/haystack_ai-2.0.1rc1.tar.gz` & `tmp/haystack_ai-2.0.1rc2.tar.gz`

## Comparing `haystack_ai-2.0.1rc1.tar` & `haystack_ai-2.0.1rc2.tar`

### file list

```diff
@@ -1,169 +1,169 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/VERSION.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/errors.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/logging.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13706 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16195 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/azure.py
--rw-r--r--   0        0        0    12132 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    12720 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    17612 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    17574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/errors.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/serialization.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/type_utils.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/component.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/component/types.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    53414 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/document.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/sparse_embedding.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/marshal/yaml.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/__init__.py
--rw-r--r--   0        0        0    57626 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/factory.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/tracing/utils.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/auth.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/device.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/expit.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/filters.py
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/LICENSE
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/README.md
--rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/VERSION.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/errors.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/logging.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13706 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16195 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0    12132 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    12720 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    17612 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    17574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/errors.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/types.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    53414 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    57626 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/device.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/filters.py
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/LICENSE
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/README.md
+-rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/PKG-INFO
```

### Comparing `haystack_ai-2.0.1rc1/haystack/__init__.py` & `haystack_ai-2.0.1rc2/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/lazy_imports.py` & `haystack_ai-2.0.1rc2/haystack/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/logging.py` & `haystack_ai-2.0.1rc2/haystack/logging.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/audio/whisper_local.py` & `haystack_ai-2.0.1rc2/haystack/components/audio/whisper_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.0.1rc2/haystack/components/audio/whisper_remote.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/builders/answer_builder.py` & `haystack_ai-2.0.1rc2/haystack/components/builders/answer_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/builders/prompt_builder.py` & `haystack_ai-2.0.1rc2/haystack/components/builders/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/caching/cache_checker.py` & `haystack_ai-2.0.1rc2/haystack/components/caching/cache_checker.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.0.1rc2/haystack/components/classifiers/document_language_classifier.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.0.1rc2/haystack/components/connectors/openapi_service.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/__init__.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/azure.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/html.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/html.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/markdown.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/markdown.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/openapi_functions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/output_adapter.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/output_adapter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/pypdf.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/pypdf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/tika.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/tika.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/txt.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/txt.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/converters/utils.py` & `haystack_ai-2.0.1rc2/haystack/components/converters/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/__init__.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/azure_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/azure_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/openai_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/openai_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.0.1rc2/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.0.1rc2/haystack/components/extractors/named_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/fetchers/link_content.py` & `haystack_ai-2.0.1rc2/haystack/components/fetchers/link_content.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/azure.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from haystack.utils import (
     ComponentDevice,
     Secret,
     deserialize_callable,
     deserialize_secrets_inplace,
     serialize_callable,
 )
-from haystack.utils.hf import HFTokenStreamingHandler, deserialize_hf_model_kwargs, serialize_hf_model_kwargs
+from haystack.utils.hf import deserialize_hf_model_kwargs, serialize_hf_model_kwargs
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_TASKS = ["text-generation", "text2text-generation"]
 
 with LazyImport(message="Run 'pip install transformers[torch]'") as transformers_import:
     from huggingface_hub import model_info
     from transformers import StoppingCriteriaList, pipeline
 
-    from haystack.utils.hf import StopWordsCriteria  # pylint: disable=ungrouped-imports
+    from haystack.utils.hf import HFTokenStreamingHandler, StopWordsCriteria  # pylint: disable=ungrouped-imports
 
 
 @component
 class HuggingFaceLocalGenerator:
     """
     Generator based on a Hugging Face model.
```

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/openai.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/utils.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/chat/__init__.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/chat/azure.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/chat/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/generators/chat/openai.py` & `haystack_ai-2.0.1rc2/haystack/components/generators/chat/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.0.1rc2/haystack/components/joiners/document_joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/others/multiplexer.py` & `haystack_ai-2.0.1rc2/haystack/components/others/multiplexer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_splitter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.0.1rc2/haystack/components/preprocessors/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.0.1rc2/haystack/components/rankers/lost_in_the_middle.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/rankers/meta_field.py` & `haystack_ai-2.0.1rc2/haystack/components/rankers/meta_field.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.0.1rc2/haystack/components/rankers/transformers_similarity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/readers/extractive.py` & `haystack_ai-2.0.1rc2/haystack/components/readers/extractive.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.0.1rc2/haystack/components/retrievers/filter_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py` & `haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/routers/conditional_router.py` & `haystack_ai-2.0.1rc2/haystack/components/routers/conditional_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/routers/file_type_router.py` & `haystack_ai-2.0.1rc2/haystack/components/routers/file_type_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/routers/metadata_router.py` & `haystack_ai-2.0.1rc2/haystack/components/routers/metadata_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/routers/text_language_router.py` & `haystack_ai-2.0.1rc2/haystack/components/routers/text_language_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/samplers/top_p.py` & `haystack_ai-2.0.1rc2/haystack/components/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/validators/json_schema.py` & `haystack_ai-2.0.1rc2/haystack/components/validators/json_schema.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/websearch/searchapi.py` & `haystack_ai-2.0.1rc2/haystack/components/websearch/searchapi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.0.1rc2/haystack/components/websearch/serper_dev.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/components/writers/document_writer.py` & `haystack_ai-2.0.1rc2/haystack/components/writers/document_writer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/errors.py` & `haystack_ai-2.0.1rc2/haystack/core/errors.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/serialization.py` & `haystack_ai-2.0.1rc2/haystack/core/serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/type_utils.py` & `haystack_ai-2.0.1rc2/haystack/core/type_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/component/component.py` & `haystack_ai-2.0.1rc2/haystack/core/component/component.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/component/sockets.py` & `haystack_ai-2.0.1rc2/haystack/core/component/sockets.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/component/types.py` & `haystack_ai-2.0.1rc2/haystack/core/component/types.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/descriptions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/draw.py` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/draw.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/pipeline.py` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/template.py` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/template.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/__init__.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/answer.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/answer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/byte_stream.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/chat_message.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/chat_message.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/document.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/document.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/sparse_embedding.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/sparse_embedding.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/dataclasses/streaming_chunk.py` & `haystack_ai-2.0.1rc2/haystack/dataclasses/streaming_chunk.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.0.1rc2/haystack/document_stores/in_memory/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/document_stores/types/protocol.py` & `haystack_ai-2.0.1rc2/haystack/document_stores/types/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/telemetry/_environment.py` & `haystack_ai-2.0.1rc2/haystack/telemetry/_environment.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/telemetry/_telemetry.py` & `haystack_ai-2.0.1rc2/haystack/telemetry/_telemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/document_store.py` & `haystack_ai-2.0.1rc2/haystack/testing/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/factory.py` & `haystack_ai-2.0.1rc2/haystack/testing/factory.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/test_utils.py` & `haystack_ai-2.0.1rc2/haystack/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/accumulate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/add_value.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/concatenate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/fstring.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/greet.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/greet.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/parity.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/parity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/remainder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/self_loop.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/self_loop.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/subtract.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.0.1rc2/haystack/testing/sample_components/threshold.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/tracing/datadog.py` & `haystack_ai-2.0.1rc2/haystack/tracing/datadog.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/tracing/opentelemetry.py` & `haystack_ai-2.0.1rc2/haystack/tracing/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/tracing/tracer.py` & `haystack_ai-2.0.1rc2/haystack/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/tracing/utils.py` & `haystack_ai-2.0.1rc2/haystack/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/__init__.py` & `haystack_ai-2.0.1rc2/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/auth.py` & `haystack_ai-2.0.1rc2/haystack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/callable_serialization.py` & `haystack_ai-2.0.1rc2/haystack/utils/callable_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/device.py` & `haystack_ai-2.0.1rc2/haystack/utils/device.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/filters.py` & `haystack_ai-2.0.1rc2/haystack/utils/filters.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/hf.py` & `haystack_ai-2.0.1rc2/haystack/utils/hf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/jupyter.py` & `haystack_ai-2.0.1rc2/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/requests_utils.py` & `haystack_ai-2.0.1rc2/haystack/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/haystack/utils/type_serialization.py` & `haystack_ai-2.0.1rc2/haystack/utils/type_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/.gitignore` & `haystack_ai-2.0.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/LICENSE` & `haystack_ai-2.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/README.md` & `haystack_ai-2.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/pyproject.toml` & `haystack_ai-2.0.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc1/PKG-INFO` & `haystack_ai-2.0.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.0.1rc1
+Version: 2.0.1rc2
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: haystack-ai Version: 2.0.1rc1 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.0.1rc2 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
```

