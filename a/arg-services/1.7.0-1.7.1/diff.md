# Comparing `tmp/arg_services-1.7.0.tar.gz` & `tmp/arg_services-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arg_services-1.7.0.tar", max compression
+gzip compressed data, was "arg_services-1.7.1.tar", max compression
```

## Comparing `arg_services-1.7.0.tar` & `arg_services-1.7.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1067 2024-04-04 09:41:41.288773 arg_services-1.7.0/LICENSE
--rw-r--r--   0        0        0      657 2024-04-04 09:41:41.288773 arg_services-1.7.0/README.md
--rw-r--r--   0        0        0      666 2024-04-04 09:42:41.552676 arg_services-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     7916 2024-04-04 09:42:41.184677 arg_services-1.7.0/src/arg_services/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.160677 arg_services-1.7.0/src/arg_services/cbr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.160677 arg_services-1.7.0/src/arg_services/cbr/v1beta/__init__.py
--rw-r--r--   0        0        0     7194 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.py
--rw-r--r--   0        0        0    12424 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
--rw-r--r--   0        0        0     2783 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
--rw-r--r--   0        0        0     1470 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
--rw-r--r--   0        0        0     3487 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.py
--rw-r--r--   0        0        0     3094 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi
--rw-r--r--   0        0        0     2792 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
--rw-r--r--   0        0        0     1474 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
--rw-r--r--   0        0        0     2566 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.py
--rw-r--r--   0        0        0     2515 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2_grpc.py
--rw-r--r--   0        0        0      400 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
--rw-r--r--   0        0        0     8381 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.py
--rw-r--r--   0        0        0    15179 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
--rw-r--r--   0        0        0     4628 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
--rw-r--r--   0        0        0     2214 2024-04-04 09:42:41.132677 arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.172677 arg_services-1.7.0/src/arg_services/graph/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.172677 arg_services-1.7.0/src/arg_services/graph/v1/__init__.py
--rw-r--r--   0        0        0    12004 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.py
--rw-r--r--   0        0        0    33449 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2_grpc.py
--rw-r--r--   0        0        0      475 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.152677 arg_services-1.7.0/src/arg_services/mining/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.152677 arg_services-1.7.0/src/arg_services/mining/v1beta/__init__.py
--rw-r--r--   0        0        0     5123 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     6692 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     4625 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     2199 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     5853 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     9022 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     2894 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1554 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     4221 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.py
--rw-r--r--   0        0        0     3932 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
--rw-r--r--   0        0        0     3092 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
--rw-r--r--   0        0        0     1713 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
--rw-r--r--   0        0        0     3883 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     4057 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     2896 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0     1552 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0     2977 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.py
--rw-r--r--   0        0        0     2419 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.pyi
--rw-r--r--   0        0        0     2834 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py
--rw-r--r--   0        0        0     1502 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.164677 arg_services-1.7.0/src/arg_services/mining_explanation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.164677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/__init__.py
--rw-r--r--   0        0        0     3418 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py
--rw-r--r--   0        0        0     3359 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
--rw-r--r--   0        0        0     3044 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
--rw-r--r--   0        0        0     1644 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
--rw-r--r--   0        0        0     4573 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
--rw-r--r--   0        0        0     5167 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
--rw-r--r--   0        0        0     3110 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
--rw-r--r--   0        0        0     1705 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
--rw-r--r--   0        0        0     3928 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
--rw-r--r--   0        0        0     3980 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
--rw-r--r--   0        0        0     3112 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
--rw-r--r--   0        0        0     1703 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.168677 arg_services-1.7.0/src/arg_services/nlp/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.168677 arg_services-1.7.0/src/arg_services/nlp/v1/__init__.py
--rw-r--r--   0        0        0     9100 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.py
--rw-r--r--   0        0        0    27846 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.pyi
--rw-r--r--   0        0        0     6344 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py
--rw-r--r--   0        0        0     4043 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.148677 arg_services-1.7.0/src/arg_services/quality/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.148677 arg_services-1.7.0/src/arg_services/quality/v1beta/__init__.py
--rw-r--r--   0        0        0     4342 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2.py
--rw-r--r--   0        0        0     5228 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2.pyi
--rw-r--r--   0        0        0     2961 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2_grpc.py
--rw-r--r--   0        0        0     1595 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2_grpc.pyi
--rw-r--r--   0        0        0     4494 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2.py
--rw-r--r--   0        0        0     5884 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2.pyi
--rw-r--r--   0        0        0     2917 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2_grpc.py
--rw-r--r--   0        0        0     1570 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2_grpc.pyi
--rw-r--r--   0        0        0     4102 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2.py
--rw-r--r--   0        0        0     5224 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2.pyi
--rw-r--r--   0        0        0     2923 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2_grpc.py
--rw-r--r--   0        0        0     1570 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.156677 arg_services-1.7.0/src/arg_services/ranking/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.156677 arg_services-1.7.0/src/arg_services/ranking/v1beta/__init__.py
--rw-r--r--   0        0        0     3509 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2.py
--rw-r--r--   0        0        0     3421 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2.pyi
--rw-r--r--   0        0        0     3063 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2_grpc.py
--rw-r--r--   0        0        0     1685 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2_grpc.pyi
--rw-r--r--   0        0        0     6899 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2.py
--rw-r--r--   0        0        0     9900 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2.pyi
--rw-r--r--   0        0        0     4814 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2_grpc.py
--rw-r--r--   0        0        0     2354 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.176677 arg_services-1.7.0/src/google/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 09:42:41.176677 arg_services-1.7.0/src/google/api/__init__.py
--rw-r--r--   0        0        0     1756 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2.py
--rw-r--r--   0        0        0     1047 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0      951 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/annotations_pb2_grpc.pyi
--rw-r--r--   0        0        0     2654 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2.py
--rw-r--r--   0        0        0    18295 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0      951 2024-04-04 09:42:41.136677 arg_services-1.7.0/src/google/api/http_pb2_grpc.pyi
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 arg_services-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-09 09:37:15.774916 arg_services-1.7.1/LICENSE
+-rw-r--r--   0        0        0      657 2024-04-09 09:37:15.774916 arg_services-1.7.1/README.md
+-rw-r--r--   0        0        0      666 2024-04-09 09:38:18.027533 arg_services-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7916 2024-04-09 09:38:17.603528 arg_services-1.7.1/src/arg_services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.591528 arg_services-1.7.1/src/arg_services/cbr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.591528 arg_services-1.7.1/src/arg_services/cbr/v1beta/__init__.py
+-rw-r--r--   0        0        0     7194 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2.py
+-rw-r--r--   0        0        0    12424 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2.pyi
+-rw-r--r--   0        0        0     2783 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py
+-rw-r--r--   0        0        0     1470 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3487 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2.py
+-rw-r--r--   0        0        0     3094 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2.pyi
+-rw-r--r--   0        0        0     2792 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py
+-rw-r--r--   0        0        0     1474 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2566 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/model_pb2.py
+-rw-r--r--   0        0        0     2515 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/model_pb2_grpc.py
+-rw-r--r--   0        0        0      400 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/model_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8381 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2.py
+-rw-r--r--   0        0        0    15179 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2.pyi
+-rw-r--r--   0        0        0     4628 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py
+-rw-r--r--   0        0        0     2214 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.579528 arg_services-1.7.1/src/arg_services/graph/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.583528 arg_services-1.7.1/src/arg_services/graph/v1/__init__.py
+-rw-r--r--   0        0        0    12004 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/graph/v1/graph_pb2.py
+-rw-r--r--   0        0        0    33449 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/graph/v1/graph_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/graph/v1/graph_pb2_grpc.py
+-rw-r--r--   0        0        0      475 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/graph/v1/graph_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.567528 arg_services-1.7.1/src/arg_services/mining/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.567528 arg_services-1.7.1/src/arg_services/mining/v1beta/__init__.py
+-rw-r--r--   0        0        0     5123 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     6692 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     4625 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     2199 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5853 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     9022 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     2894 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1554 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4221 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2.py
+-rw-r--r--   0        0        0     3932 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2.pyi
+-rw-r--r--   0        0        0     3092 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py
+-rw-r--r--   0        0        0     1713 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3883 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     4057 2024-04-09 09:38:17.539528 arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     2896 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0     1552 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2977 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2.py
+-rw-r--r--   0        0        0     2419 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2.pyi
+-rw-r--r--   0        0        0     2834 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2_grpc.py
+-rw-r--r--   0        0        0     1502 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.571528 arg_services-1.7.1/src/arg_services/mining_explanation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.571528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/__init__.py
+-rw-r--r--   0        0        0     3418 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2.py
+-rw-r--r--   0        0        0     3359 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi
+-rw-r--r--   0        0        0     3044 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py
+-rw-r--r--   0        0        0     1644 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4573 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.py
+-rw-r--r--   0        0        0     5167 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi
+-rw-r--r--   0        0        0     3110 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py
+-rw-r--r--   0        0        0     1705 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3928 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py
+-rw-r--r--   0        0        0     3980 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi
+-rw-r--r--   0        0        0     3112 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py
+-rw-r--r--   0        0        0     1703 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.583528 arg_services-1.7.1/src/arg_services/nlp/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.587528 arg_services-1.7.1/src/arg_services/nlp/v1/__init__.py
+-rw-r--r--   0        0        0     9100 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2.py
+-rw-r--r--   0        0        0    27846 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2.pyi
+-rw-r--r--   0        0        0     6344 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2_grpc.py
+-rw-r--r--   0        0        0     4043 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.575528 arg_services-1.7.1/src/arg_services/quality/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.579528 arg_services-1.7.1/src/arg_services/quality/v1beta/__init__.py
+-rw-r--r--   0        0        0     4342 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2.py
+-rw-r--r--   0        0        0     5228 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2.pyi
+-rw-r--r--   0        0        0     2961 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2_grpc.py
+-rw-r--r--   0        0        0     1595 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4494 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2.py
+-rw-r--r--   0        0        0     5884 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2.pyi
+-rw-r--r--   0        0        0     2917 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2_grpc.py
+-rw-r--r--   0        0        0     1570 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4340 2024-04-09 09:38:17.547528 arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2.py
+-rw-r--r--   0        0        0     5969 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2.pyi
+-rw-r--r--   0        0        0     2923 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2_grpc.py
+-rw-r--r--   0        0        0     1570 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.559528 arg_services-1.7.1/src/arg_services/ranking/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.563528 arg_services-1.7.1/src/arg_services/ranking/v1beta/__init__.py
+-rw-r--r--   0        0        0     3509 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2.py
+-rw-r--r--   0        0        0     3421 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2.pyi
+-rw-r--r--   0        0        0     3063 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2_grpc.py
+-rw-r--r--   0        0        0     1685 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6899 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2.py
+-rw-r--r--   0        0        0     9900 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2.pyi
+-rw-r--r--   0        0        0     4814 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2_grpc.py
+-rw-r--r--   0        0        0     2354 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.595528 arg_services-1.7.1/src/google/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 09:38:17.595528 arg_services-1.7.1/src/google/api/__init__.py
+-rw-r--r--   0        0        0     1756 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0     1047 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/annotations_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/annotations_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2654 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/http_pb2.py
+-rw-r--r--   0        0        0    18295 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/http_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0      951 2024-04-09 09:38:17.543528 arg_services-1.7.1/src/google/api/http_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 arg_services-1.7.1/PKG-INFO
```

### Comparing `arg_services-1.7.0/LICENSE` & `arg_services-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/README.md` & `arg_services-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/pyproject.toml` & `arg_services-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arg-services"
-version = "1.7.0"
+version = "1.7.1"
 description = "gRPC definitions for microservice-based argumentation machines"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/arg-services-python"
 include = ["src/**/*"]
```

### Comparing `arg_services-1.7.0/src/arg_services/__init__.py` & `arg_services-1.7.1/src/arg_services/__init__.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/adaptation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/casebase_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/model_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/model_pb2.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/cbr/v1beta/retrieval_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.py` & `arg_services-1.7.1/src/arg_services/graph/v1/graph_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/graph/v1/graph_pb2.pyi` & `arg_services-1.7.1/src/arg_services/graph/v1/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/graph_construction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining/v1beta/mining_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.py` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/adu_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.py` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/entailment_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/mining_explanation/v1beta/major_claim_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.py` & `arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2.pyi` & `arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/nlp/v1/nlp_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2.py` & `arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2.pyi` & `arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/expert_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/quality/v1beta/expert_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2.py` & `arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2.pyi` & `arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/explanation_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/quality/v1beta/explanation_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2.py` & `arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/quality/v1beta/qualia.proto\x12\x1b\x61rg_services.quality.v1beta\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xac\x01\n\x18QualiaAnnotationsRequest\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12K\n\x08patterns\x18\x02 \x03(\x0b\x32/.arg_services.quality.v1beta.QualiaInputPatternR\x08patterns\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xc7\x01\n\x19QualiaAnnotationsResponse\x12+\n\x11\x63onstituency_tree\x18\x01 \x01(\tR\x10\x63onstituencyTree\x12L\n\x08patterns\x18\x02 \x03(\x0b\x32\x30.arg_services.quality.v1beta.QualiaOutputPatternR\x08patterns\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x95\x01\n\x12QualiaInputPattern\x12\x18\n\x07pattern\x18\x01 \x01(\tR\x07pattern\x12;\n\x04role\x18\x02 \x01(\x0e\x32\'.arg_services.quality.v1beta.QualiaRoleR\x04role\x12(\n\x10\x61llowed_pos_tags\x18\x03 \x03(\tR\x0e\x61llowedPosTags\"f\n\x13QualiaOutputPattern\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12;\n\x04role\x18\x02 \x01(\x0e\x32\'.arg_services.quality.v1beta.QualiaRoleR\x04role*\x90\x01\n\nQualiaRole\x12\x1b\n\x17QUALIA_ROLE_UNSPECIFIED\x10\x00\x12\x16\n\x12QUALIA_ROLE_FORMAL\x10\x01\x12\x1c\n\x18QUALIA_ROLE_CONSITIUTIVE\x10\x02\x12\x15\n\x11QUALIA_ROLE_TELIC\x10\x03\x12\x18\n\x14QUALIA_ROLE_AGENTIVE\x10\x04\x32\xc3\x01\n\rQualiaService\x12\xb1\x01\n\x11QualiaAnnotations\x12\x35.arg_services.quality.v1beta.QualiaAnnotationsRequest\x1a\x36.arg_services.quality.v1beta.QualiaAnnotationsResponse\"-\x82\xd3\xe4\x93\x02\'\"\"/quality/v1beta/qualia_annotations:\x01*B\xb8\x01\n\x1f\x63om.arg_services.quality.v1betaB\x0bQualiaProtoP\x01\xa2\x02\x03\x41QX\xaa\x02\x1a\x41rgServices.Quality.V1beta\xca\x02\x1a\x41rgServices\\Quality\\V1beta\xe2\x02&ArgServices\\Quality\\V1beta\\GPBMetadata\xea\x02\x1c\x41rgServices::Quality::V1betab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(arg_services/quality/v1beta/qualia.proto\x12\x1b\x61rg_services.quality.v1beta\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\xe2\x01\n\x18QualiaAnnotationsRequest\x12\x12\n\x04text\x18\x01 \x01(\tR\x04text\x12K\n\x08patterns\x18\x02 \x03(\x0b\x32/.arg_services.quality.v1beta.QualiaInputPatternR\x08patterns\x12\x1a\n\x08language\x18\x03 \x01(\tR\x08language\x12\x18\n\x07queries\x18\x04 \x03(\tR\x07queries\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\xc7\x01\n\x19QualiaAnnotationsResponse\x12+\n\x11\x63onstituency_tree\x18\x01 \x01(\tR\x10\x63onstituencyTree\x12L\n\x08patterns\x18\x02 \x03(\x0b\x32\x30.arg_services.quality.v1beta.QualiaOutputPatternR\x08patterns\x12/\n\x06\x65xtras\x18\x0f \x01(\x0b\x32\x17.google.protobuf.StructR\x06\x65xtras\"\x95\x01\n\x12QualiaInputPattern\x12\x18\n\x07pattern\x18\x01 \x01(\tR\x07pattern\x12;\n\x04role\x18\x02 \x01(\x0e\x32\'.arg_services.quality.v1beta.QualiaRoleR\x04role\x12(\n\x10\x61llowed_pos_tags\x18\x03 \x03(\tR\x0e\x61llowedPosTags\"\xc2\x01\n\x13QualiaOutputPattern\x12.\n\x13input_pattern_match\x18\x01 \x01(\tR\x11inputPatternMatch\x12\x1d\n\nquery_text\x18\x02 \x01(\tR\tqueryText\x12\x1f\n\x0bqualia_text\x18\x03 \x01(\tR\nqualiaText\x12;\n\x04role\x18\x04 \x01(\x0e\x32\'.arg_services.quality.v1beta.QualiaRoleR\x04role*\x90\x01\n\nQualiaRole\x12\x1b\n\x17QUALIA_ROLE_UNSPECIFIED\x10\x00\x12\x16\n\x12QUALIA_ROLE_FORMAL\x10\x01\x12\x1c\n\x18QUALIA_ROLE_CONSITIUTIVE\x10\x02\x12\x15\n\x11QUALIA_ROLE_TELIC\x10\x03\x12\x18\n\x14QUALIA_ROLE_AGENTIVE\x10\x04\x32\xc3\x01\n\rQualiaService\x12\xb1\x01\n\x11QualiaAnnotations\x12\x35.arg_services.quality.v1beta.QualiaAnnotationsRequest\x1a\x36.arg_services.quality.v1beta.QualiaAnnotationsResponse\"-\x82\xd3\xe4\x93\x02\'\"\"/quality/v1beta/qualia_annotations:\x01*B\xb8\x01\n\x1f\x63om.arg_services.quality.v1betaB\x0bQualiaProtoP\x01\xa2\x02\x03\x41QX\xaa\x02\x1a\x41rgServices.Quality.V1beta\xca\x02\x1a\x41rgServices\\Quality\\V1beta\xe2\x02&ArgServices\\Quality\\V1beta\\GPBMetadata\xea\x02\x1c\x41rgServices::Quality::V1betab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'arg_services.quality.v1beta.qualia_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\037com.arg_services.quality.v1betaB\013QualiaProtoP\001\242\002\003AQX\252\002\032ArgServices.Quality.V1beta\312\002\032ArgServices\\Quality\\V1beta\342\002&ArgServices\\Quality\\V1beta\\GPBMetadata\352\002\034ArgServices::Quality::V1beta'
   _globals['_QUALIASERVICE'].methods_by_name['QualiaAnnotations']._options = None
   _globals['_QUALIASERVICE'].methods_by_name['QualiaAnnotations']._serialized_options = b'\202\323\344\223\002\'\"\"/quality/v1beta/qualia_annotations:\001*'
-  _globals['_QUALIAROLE']._serialized_start=767
-  _globals['_QUALIAROLE']._serialized_end=911
+  _globals['_QUALIAROLE']._serialized_start=914
+  _globals['_QUALIAROLE']._serialized_end=1058
   _globals['_QUALIAANNOTATIONSREQUEST']._serialized_start=134
-  _globals['_QUALIAANNOTATIONSREQUEST']._serialized_end=306
-  _globals['_QUALIAANNOTATIONSRESPONSE']._serialized_start=309
-  _globals['_QUALIAANNOTATIONSRESPONSE']._serialized_end=508
-  _globals['_QUALIAINPUTPATTERN']._serialized_start=511
-  _globals['_QUALIAINPUTPATTERN']._serialized_end=660
-  _globals['_QUALIAOUTPUTPATTERN']._serialized_start=662
-  _globals['_QUALIAOUTPUTPATTERN']._serialized_end=764
-  _globals['_QUALIASERVICE']._serialized_start=914
-  _globals['_QUALIASERVICE']._serialized_end=1109
+  _globals['_QUALIAANNOTATIONSREQUEST']._serialized_end=360
+  _globals['_QUALIAANNOTATIONSRESPONSE']._serialized_start=363
+  _globals['_QUALIAANNOTATIONSRESPONSE']._serialized_end=562
+  _globals['_QUALIAINPUTPATTERN']._serialized_start=565
+  _globals['_QUALIAINPUTPATTERN']._serialized_end=714
+  _globals['_QUALIAOUTPUTPATTERN']._serialized_start=717
+  _globals['_QUALIAOUTPUTPATTERN']._serialized_end=911
+  _globals['_QUALIASERVICE']._serialized_start=1061
+  _globals['_QUALIASERVICE']._serialized_end=1256
 # @@protoc_insertion_point(module_scope)
```

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2.pyi` & `arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -42,30 +42,37 @@
 
 @typing_extensions.final
 class QualiaAnnotationsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TEXT_FIELD_NUMBER: builtins.int
     PATTERNS_FIELD_NUMBER: builtins.int
+    LANGUAGE_FIELD_NUMBER: builtins.int
+    QUERIES_FIELD_NUMBER: builtins.int
     EXTRAS_FIELD_NUMBER: builtins.int
     text: builtins.str
     @property
     def patterns(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___QualiaInputPattern]: ...
+    language: builtins.str
+    @property
+    def queries(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def extras(self) -> google.protobuf.struct_pb2.Struct:
         """Implementation-specific information can be encoded here"""
     def __init__(
         self,
         *,
         text: builtins.str = ...,
         patterns: collections.abc.Iterable[global___QualiaInputPattern] | None = ...,
+        language: builtins.str = ...,
+        queries: collections.abc.Iterable[builtins.str] | None = ...,
         extras: google.protobuf.struct_pb2.Struct | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["extras", b"extras"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "patterns", b"patterns", "text", b"text"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extras", b"extras", "language", b"language", "patterns", b"patterns", "queries", b"queries", "text", b"text"]) -> None: ...
 
 global___QualiaAnnotationsRequest = QualiaAnnotationsRequest
 
 @typing_extensions.final
 class QualiaAnnotationsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -112,20 +119,26 @@
 
 global___QualiaInputPattern = QualiaInputPattern
 
 @typing_extensions.final
 class QualiaOutputPattern(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TEXT_FIELD_NUMBER: builtins.int
+    INPUT_PATTERN_MATCH_FIELD_NUMBER: builtins.int
+    QUERY_TEXT_FIELD_NUMBER: builtins.int
+    QUALIA_TEXT_FIELD_NUMBER: builtins.int
     ROLE_FIELD_NUMBER: builtins.int
-    text: builtins.str
+    input_pattern_match: builtins.str
+    query_text: builtins.str
+    qualia_text: builtins.str
     role: global___QualiaRole.ValueType
     def __init__(
         self,
         *,
-        text: builtins.str = ...,
+        input_pattern_match: builtins.str = ...,
+        query_text: builtins.str = ...,
+        qualia_text: builtins.str = ...,
         role: global___QualiaRole.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["role", b"role", "text", b"text"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["input_pattern_match", b"input_pattern_match", "qualia_text", b"qualia_text", "query_text", b"query_text", "role", b"role"]) -> None: ...
 
 global___QualiaOutputPattern = QualiaOutputPattern
```

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/quality/v1beta/qualia_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/quality/v1beta/qualia_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2.py` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2.pyi` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/granularity_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/granularity_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2.py` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2.pyi` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2_grpc.py` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/arg_services/ranking/v1beta/ranking_pb2_grpc.pyi` & `arg_services-1.7.1/src/arg_services/ranking/v1beta/ranking_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/google/api/annotations_pb2.py` & `arg_services-1.7.1/src/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/google/api/annotations_pb2.pyi` & `arg_services-1.7.1/src/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/google/api/annotations_pb2_grpc.pyi` & `arg_services-1.7.1/src/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/google/api/http_pb2.py` & `arg_services-1.7.1/src/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/google/api/http_pb2.pyi` & `arg_services-1.7.1/src/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/src/google/api/http_pb2_grpc.pyi` & `arg_services-1.7.1/src/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `arg_services-1.7.0/PKG-INFO` & `arg_services-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arg-services
-Version: 1.7.0
+Version: 1.7.1
 Summary: gRPC definitions for microservice-based argumentation machines
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

