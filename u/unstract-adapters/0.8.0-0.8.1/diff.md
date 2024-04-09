# Comparing `tmp/unstract_adapters-0.8.0.tar.gz` & `tmp/unstract_adapters-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstract_adapters-0.8.0.tar", last modified: Tue Apr  2 04:46:27 2024, max compression
+gzip compressed data, was "unstract_adapters-0.8.1.tar", last modified: Tue Apr  9 06:23:41 2024, max compression
```

## Comparing `unstract_adapters-0.8.0.tar` & `unstract_adapters-0.8.1.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0    34523 2024-04-02 04:46:08.105988 unstract_adapters-0.8.0/LICENSE
--rw-r--r--   0        0        0     1598 2024-04-02 04:46:08.105988 unstract_adapters-0.8.0/README.md
--rw-r--r--   0        0        0     2271 2024-04-02 04:46:27.253869 unstract_adapters-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      297 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/__init__.py
--rw-r--r--   0        0        0     2665 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/adapterkit.py
--rw-r--r--   0        0        0     1745 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/base.py
--rw-r--r--   0        0        0      282 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/constants.py
--rw-r--r--   0        0        0      183 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/__init__.py
--rw-r--r--   0        0        0      154 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/README.md
--rw-r--r--   0        0        0      514 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      216 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1548 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      899 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/embedding_adapter.py
--rw-r--r--   0        0        0     1324 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/helper.py
--rw-r--r--   0        0        0       42 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/README.md
--rw-r--r--   0        0        0      517 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/pyproject.toml
--rw-r--r--   0        0        0      215 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
--rw-r--r--   0        0        0      940 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
--rw-r--r--   0        0        0       30 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/README.md
--rw-r--r--   0        0        0      503 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py
--rw-r--r--   0        0        0      719 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       35 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/README.md
--rw-r--r--   0        0        0      510 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/pyproject.toml
--rw-r--r--   0        0        0      179 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/__init__.py
--rw-r--r--   0        0        0     2041 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/palm.py
--rw-r--r--   0        0        0      804 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json
--rw-r--r--   0        0        0       46 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
--rw-r--r--   0        0        0      524 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
--rw-r--r--   0        0        0      239 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
--rw-r--r--   0        0        0     1827 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
--rw-r--r--   0        0        0      553 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
--rw-r--r--   0        0        0     2086 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/embedding/register.py
--rw-r--r--   0        0        0      184 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/enums.py
--rw-r--r--   0        0        0      502 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/exceptions.py
--rw-r--r--   0        0        0      165 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/__init__.py
--rw-r--r--   0        0        0       33 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/README.md
--rw-r--r--   0        0        0      498 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/__init__.py
--rw-r--r--   0        0        0     2324 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/anthropic.py
--rw-r--r--   0        0        0     1017 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
--rw-r--r--   0        0        0       33 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/README.md
--rw-r--r--   0        0        0      498 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/pyproject.toml
--rw-r--r--   0        0        0      202 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/__init__.py
--rw-r--r--   0        0        0     2520 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/anyscale.py
--rw-r--r--   0        0        0     1327 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
--rw-r--r--   0        0        0       37 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/README.md
--rw-r--r--   0        0        0      503 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
--rw-r--r--   0        0        0     2312 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
--rw-r--r--   0        0        0     1681 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       41 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/constants.py
--rw-r--r--   0        0        0      844 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/helper.py
--rw-r--r--   0        0        0     1544 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/llm_adapter.py
--rw-r--r--   0        0        0       34 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/README.md
--rw-r--r--   0        0        0      500 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/pyproject.toml
--rw-r--r--   0        0        0      197 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/mistral.py
--rw-r--r--   0        0        0      852 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json
--rw-r--r--   0        0        0       31 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/README.md
--rw-r--r--   0        0        0      491 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/pyproject.toml
--rw-r--r--   0        0        0      193 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/__init__.py
--rw-r--r--   0        0        0     2763 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/open_ai.py
--rw-r--r--   0        0        0     1489 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
--rw-r--r--   0        0        0       26 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/README.md
--rw-r--r--   0        0        0      496 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/pyproject.toml
--rw-r--r--   0        0        0      182 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/__init__.py
--rw-r--r--   0        0        0     2136 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/palm.py
--rw-r--r--   0        0        0      989 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/static/json_schema.json
--rw-r--r--   0        0        0     1963 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/register.py
--rw-r--r--   0        0        0       33 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/README.md
--rw-r--r--   0        0        0      499 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/pyproject.toml
--rw-r--r--   0        0        0      207 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/replicate.py
--rw-r--r--   0        0        0      840 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json
--rw-r--r--   0        0        0      273 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/README.md
--rw-r--r--   0        0        0      480 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/pyproject.toml
--rw-r--r--   0        0        0      203 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/__init__.py
--rw-r--r--   0        0        0      964 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
--rw-r--r--   0        0        0     2137 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
--rw-r--r--   0        0        0      165 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/__init__.py
--rw-r--r--   0        0        0      430 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/constants.py
--rw-r--r--   0        0        0       42 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/README.md
--rw-r--r--   0        0        0      491 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/README.md
--rw-r--r--   0        0        0      237 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
--rw-r--r--   0        0        0     5994 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
--rw-r--r--   0        0        0      817 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
--rw-r--r--   0        0        0      978 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/ocr_adapter.py
--rw-r--r--   0        0        0     1964 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/ocr/register.py
--rw-r--r--   0        0        0      277 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/registry.py
--rw-r--r--   0        0        0     1745 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/utils.py
--rw-r--r--   0        0        0      181 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/__init__.py
--rw-r--r--   0        0        0      225 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/constants.py
--rw-r--r--   0        0        0     4187 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/helper.py
--rw-r--r--   0        0        0       27 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/README.md
--rw-r--r--   0        0        0      508 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/__init__.py
--rw-r--r--   0        0        0     2775 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/milvus.py
--rw-r--r--   0        0        0      805 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/README.md
--rw-r--r--   0        0        0      519 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/__init__.py
--rw-r--r--   0        0        0     3541 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
--rw-r--r--   0        0        0      771 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
--rw-r--r--   0        0        0       29 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/README.md
--rw-r--r--   0        0        0      512 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/__init__.py
--rw-r--r--   0        0        0     3930 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/postgres.py
--rw-r--r--   0        0        0      912 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
--rw-r--r--   0        0        0       27 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/README.md
--rw-r--r--   0        0        0      513 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/pyproject.toml
--rw-r--r--   0        0        0      188 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/__init__.py
--rw-r--r--   0        0        0     3019 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
--rw-r--r--   0        0        0      571 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
--rw-r--r--   0        0        0     2039 2024-04-02 04:46:08.109988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/register.py
--rw-r--r--   0        0        0    75042 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/samples/sample1.txt
--rw-r--r--   0        0        0       29 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/README.md
--rw-r--r--   0        0        0      512 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/__init__.py
--rw-r--r--   0        0        0      937 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
--rw-r--r--   0        0        0     3349 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/supabase.py
--rw-r--r--   0        0        0      947 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/vectordb_adapter.py
--rw-r--r--   0        0        0       29 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/README.md
--rw-r--r--   0        0        0      520 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/pyproject.toml
--rw-r--r--   0        0        0      198 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/__init__.py
--rw-r--r--   0        0        0      678 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
--rw-r--r--   0        0        0     3722 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
--rw-r--r--   0        0        0      174 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/__init__.py
--rw-r--r--   0        0        0      145 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/constants.py
--rw-r--r--   0        0        0     5407 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/helper.py
--rw-r--r--   0        0        0       40 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/README.md
--rw-r--r--   0        0        0      495 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
--rw-r--r--   0        0        0      217 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
--rw-r--r--   0        0        0      981 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
--rw-r--r--   0        0        0     6562 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
--rw-r--r--   0        0        0     3115 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
--rw-r--r--   0        0        0     1991 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/register.py
--rw-r--r--   0        0        0       51 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/README.md
--rw-r--r--   0        0        0      499 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
--rw-r--r--   0        0        0      255 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
--rw-r--r--   0        0        0      583 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
--rw-r--r--   0        0        0     1463 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
--rw-r--r--   0        0        0       52 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/README.md
--rw-r--r--   0        0        0      499 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
--rw-r--r--   0        0        0      259 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
--rw-r--r--   0        0        0      805 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
--rw-r--r--   0        0        0     1468 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
--rw-r--r--   0        0        0     1006 2024-04-02 04:46:08.113988 unstract_adapters-0.8.0/src/unstract/adapters/x2text/x2text_adapter.py
--rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 unstract_adapters-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-09 06:23:17.493884 unstract_adapters-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1598 2024-04-09 06:23:17.493884 unstract_adapters-0.8.1/README.md
+-rw-r--r--   0        0        0     2271 2024-04-09 06:23:41.681894 unstract_adapters-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      297 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/__init__.py
+-rw-r--r--   0        0        0     2665 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/adapterkit.py
+-rw-r--r--   0        0        0     1745 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/base.py
+-rw-r--r--   0        0        0      282 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/constants.py
+-rw-r--r--   0        0        0      183 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/README.md
+-rw-r--r--   0        0        0      514 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      216 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2511 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1548 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0      899 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/embedding_adapter.py
+-rw-r--r--   0        0        0     1324 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/helper.py
+-rw-r--r--   0        0        0       42 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/README.md
+-rw-r--r--   0        0        0      517 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/pyproject.toml
+-rw-r--r--   0        0        0      215 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py
+-rw-r--r--   0        0        0      940 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json
+-rw-r--r--   0        0        0       30 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/README.md
+-rw-r--r--   0        0        0      503 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0      719 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       35 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/README.md
+-rw-r--r--   0        0        0      510 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/pyproject.toml
+-rw-r--r--   0        0        0      179 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/__init__.py
+-rw-r--r--   0        0        0     2041 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/palm.py
+-rw-r--r--   0        0        0      804 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0       46 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/README.md
+-rw-r--r--   0        0        0      524 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml
+-rw-r--r--   0        0        0      239 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/__init__.py
+-rw-r--r--   0        0        0     1827 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py
+-rw-r--r--   0        0        0      553 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json
+-rw-r--r--   0        0        0     2086 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/embedding/register.py
+-rw-r--r--   0        0        0      184 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/enums.py
+-rw-r--r--   0        0        0      502 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/exceptions.py
+-rw-r--r--   0        0        0      165 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/README.md
+-rw-r--r--   0        0        0      498 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/__init__.py
+-rw-r--r--   0        0        0     2324 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/anthropic.py
+-rw-r--r--   0        0        0     1017 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json
+-rw-r--r--   0        0        0       33 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/README.md
+-rw-r--r--   0        0        0      498 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/pyproject.toml
+-rw-r--r--   0        0        0      202 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/__init__.py
+-rw-r--r--   0        0        0     2520 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/anyscale.py
+-rw-r--r--   0        0        0     1327 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json
+-rw-r--r--   0        0        0       37 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/README.md
+-rw-r--r--   0        0        0      503 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2312 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py
+-rw-r--r--   0        0        0     1681 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       41 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/constants.py
+-rw-r--r--   0        0        0      844 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/helper.py
+-rw-r--r--   0        0        0     1544 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/llm_adapter.py
+-rw-r--r--   0        0        0       34 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/README.md
+-rw-r--r--   0        0        0      500 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/pyproject.toml
+-rw-r--r--   0        0        0      197 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/__init__.py
+-rw-r--r--   0        0        0     1824 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/mistral.py
+-rw-r--r--   0        0        0      852 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json
+-rw-r--r--   0        0        0       31 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/README.md
+-rw-r--r--   0        0        0      491 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/pyproject.toml
+-rw-r--r--   0        0        0      193 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/__init__.py
+-rw-r--r--   0        0        0     2763 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/open_ai.py
+-rw-r--r--   0        0        0     1489 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0       26 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/README.md
+-rw-r--r--   0        0        0      496 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/__init__.py
+-rw-r--r--   0        0        0     2136 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/palm.py
+-rw-r--r--   0        0        0      989 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/static/json_schema.json
+-rw-r--r--   0        0        0     1963 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/register.py
+-rw-r--r--   0        0        0       33 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/README.md
+-rw-r--r--   0        0        0      499 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/replicate.py
+-rw-r--r--   0        0        0      840 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json
+-rw-r--r--   0        0        0      273 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/README.md
+-rw-r--r--   0        0        0      480 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0     2137 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py
+-rw-r--r--   0        0        0      165 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/constants.py
+-rw-r--r--   0        0        0       42 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/README.md
+-rw-r--r--   0        0        0      491 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/README.md
+-rw-r--r--   0        0        0      237 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/__init__.py
+-rw-r--r--   0        0        0     5994 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py
+-rw-r--r--   0        0        0      817 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json
+-rw-r--r--   0        0        0      978 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/ocr_adapter.py
+-rw-r--r--   0        0        0     1964 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/ocr/register.py
+-rw-r--r--   0        0        0      277 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/registry.py
+-rw-r--r--   0        0        0     1745 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/utils.py
+-rw-r--r--   0        0        0      181 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/constants.py
+-rw-r--r--   0        0        0     4187 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/helper.py
+-rw-r--r--   0        0        0       27 2024-04-09 06:23:17.497884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/README.md
+-rw-r--r--   0        0        0      508 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/__init__.py
+-rw-r--r--   0        0        0     2775 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/milvus.py
+-rw-r--r--   0        0        0      805 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/README.md
+-rw-r--r--   0        0        0      519 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/__init__.py
+-rw-r--r--   0        0        0     3572 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py
+-rw-r--r--   0        0        0      771 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json
+-rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/README.md
+-rw-r--r--   0        0        0      512 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/postgres.py
+-rw-r--r--   0        0        0      912 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json
+-rw-r--r--   0        0        0       27 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/README.md
+-rw-r--r--   0        0        0      513 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/pyproject.toml
+-rw-r--r--   0        0        0      188 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/__init__.py
+-rw-r--r--   0        0        0     3019 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py
+-rw-r--r--   0        0        0      571 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json
+-rw-r--r--   0        0        0     2039 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/register.py
+-rw-r--r--   0        0        0    75042 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/samples/sample1.txt
+-rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/README.md
+-rw-r--r--   0        0        0      512 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json
+-rw-r--r--   0        0        0     3349 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/supabase.py
+-rw-r--r--   0        0        0      947 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/vectordb_adapter.py
+-rw-r--r--   0        0        0       29 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/README.md
+-rw-r--r--   0        0        0      520 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/pyproject.toml
+-rw-r--r--   0        0        0      198 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json
+-rw-r--r--   0        0        0     3722 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py
+-rw-r--r--   0        0        0      174 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/constants.py
+-rw-r--r--   0        0        0     5407 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/helper.py
+-rw-r--r--   0        0        0       40 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/README.md
+-rw-r--r--   0        0        0      495 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/__init__.py
+-rw-r--r--   0        0        0      981 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py
+-rw-r--r--   0        0        0     6562 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py
+-rw-r--r--   0        0        0     3115 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json
+-rw-r--r--   0        0        0     1991 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/register.py
+-rw-r--r--   0        0        0       51 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/README.md
+-rw-r--r--   0        0        0      499 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json
+-rw-r--r--   0        0        0     1463 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py
+-rw-r--r--   0        0        0       52 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/README.md
+-rw-r--r--   0        0        0      499 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/__init__.py
+-rw-r--r--   0        0        0      805 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json
+-rw-r--r--   0        0        0     1468 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py
+-rw-r--r--   0        0        0     1006 2024-04-09 06:23:17.501884 unstract_adapters-0.8.1/src/unstract/adapters/x2text/x2text_adapter.py
+-rw-r--r--   0        0        0     3243 1970-01-01 00:00:00.000000 unstract_adapters-0.8.1/PKG-INFO
```

### Comparing `unstract_adapters-0.8.0/LICENSE` & `unstract_adapters-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/README.md` & `unstract_adapters-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/pyproject.toml` & `unstract_adapters-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.8.0"
+version = "0.8.1"
 
 [project.urls]
 Homepage = "https://unstract.com"
 "Release notes" = "https://github.com/Zipstack/unstract-adapters/releases"
 Source = "https://github.com/Zipstack/unstract-adapters"
 
 [project.license]
```

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/adapterkit.py` & `unstract_adapters-0.8.1/src/unstract/adapters/adapterkit.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/base.py` & `unstract_adapters-0.8.1/src/unstract/adapters/base.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/azure_open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/embedding_adapter.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/embedding_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/helper.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/hugging_face.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/hugging_face/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/open_ai.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/palm.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/palm.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/palm/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/qdrant_fast_embed.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/qdrant_fast_embed/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/embedding/register.py` & `unstract_adapters-0.8.1/src/unstract/adapters/embedding/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/anthropic.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/anthropic.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/anthropic/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/anthropic/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/anyscale.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/anyscale.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/any_scale/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/any_scale/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/azure_open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/azure_open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/helper.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/llm_adapter.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/llm_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/mistral.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/mistral.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/mistral/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/mistral/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/open_ai.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/open_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/open_ai/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/open_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/palm.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/palm.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/palm/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/palm/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/register.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/replicate.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/replicate.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/replicate/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/replicate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py` & `unstract_adapters-0.8.1/src/unstract/adapters/llm/vertex_ai/src/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py` & `unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/google_document_ai.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/ocr/google_document_ai/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/ocr/ocr_adapter.py` & `unstract_adapters-0.8.1/src/unstract/adapters/ocr/ocr_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/ocr/register.py` & `unstract_adapters-0.8.1/src/unstract/adapters/ocr/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/utils.py` & `unstract_adapters-0.8.1/src/unstract/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/helper.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/milvus.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/milvus.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/milvus/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/pinecone.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,17 @@
                 api_key=str(self.config.get(Constants.API_KEY)),
                 environment=str(self.config.get(Constants.ENVIRONMENT)),
             )
             collection_name = VectorDBHelper.get_collection_name(
                 self.config.get(VectorDbConstants.VECTOR_DB_NAME),
                 self.config.get(VectorDbConstants.EMBEDDING_DIMENSION),
             )
-            # Piecone allows only alphanumeric & hyphens for collection naming
-            self.collection_name = collection_name.replace("_", "-")
+            # Pinecone allows only lowercase alphanumeric & hyphens for
+            # collection name
+            self.collection_name = collection_name.replace("_", "-").lower()
             dimension = self.config.get(
                 VectorDbConstants.EMBEDDING_DIMENSION,
                 VectorDbConstants.DEFAULT_EMBEDDING_SIZE,
             )
             try:
                 pinecone.describe_index(name=self.collection_name)
             except NotFoundException as e:
```

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/pinecone/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/postgres.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/postgres.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/postgres/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/qdrant.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/qdrant.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/qdrant/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/register.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/samples/sample1.txt` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/samples/sample1.txt`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/supabase/src/supabase.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/supabase/src/supabase.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/vectordb_adapter.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/vectordb_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/pyproject.toml` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/vectordb/weaviate/src/weaviate.py` & `unstract_adapters-0.8.1/src/unstract/adapters/vectordb/weaviate/src/weaviate.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/helper.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/constants.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/constants.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/llm_whisperer.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/llm_whisperer/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/register.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/register.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_community/src/unstructured_community.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/static/json_schema.json`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/unstructured_enterprise/src/unstructured_enterprise.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/src/unstract/adapters/x2text/x2text_adapter.py` & `unstract_adapters-0.8.1/src/unstract/adapters/x2text/x2text_adapter.py`

 * *Files identical despite different names*

### Comparing `unstract_adapters-0.8.0/PKG-INFO` & `unstract_adapters-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstract-adapters
-Version: 0.8.0
+Version: 0.8.1
 Summary: Unstract interface for LLMs, Embeddings and VectorDBs
 Author-Email: Zipstack Inc. <devsupport@zipstack.com>
 License: AGPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
```

