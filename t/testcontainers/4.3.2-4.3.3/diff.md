# Comparing `tmp/testcontainers-4.3.2.tar.gz` & `tmp/testcontainers-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.3.2.tar", max compression
+gzip compressed data, was "testcontainers-4.3.3.tar", max compression
```

## Comparing `testcontainers-4.3.2.tar` & `testcontainers-4.3.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11328 2024-04-08 09:28:03.309967 testcontainers-4.3.2/LICENSE.txt
--rw-r--r--   0        0        0     2042 2024-04-08 09:28:03.309967 testcontainers-4.3.2/README.md
--rw-r--r--   0        0        0      172 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0     2433 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     7590 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     6839 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2418 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      516 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     2088 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4091 2024-04-08 09:28:03.309967 testcontainers-4.3.2/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3781 2024-04-08 09:28:03.309967 testcontainers-4.3.2/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-04-08 09:28:03.309967 testcontainers-4.3.2/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     2492 2024-04-08 09:28:03.309967 testcontainers-4.3.2/modules/cassandra/testcontainers/cassandra/__init__.py
--rw-r--r--   0        0        0     2736 2024-04-08 09:28:03.309967 testcontainers-4.3.2/modules/chroma/testcontainers/chroma/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-08 09:28:03.309967 testcontainers-4.3.2/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-04-08 09:28:03.309967 testcontainers-4.3.2/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0      106 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2709 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/google/testcontainers/google/datastore.py
--rw-r--r--   0        0        0     2952 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3760 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2694 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3592 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2727 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/kafka/testcontainers/kafka/_redpanda.py
--rw-r--r--   0        0        0     3313 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     4116 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     1809 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2811 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/nats/testcontainers/nats/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4109 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     2810 2024-04-08 09:28:03.313967 testcontainers-4.3.2/modules/oracle-free/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     3984 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     5209 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/qdrant/testcontainers/qdrant/__init__.py
--rw-r--r--   0        0        0     2967 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2761 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/registry/testcontainers/registry/__init__.py
--rw-r--r--   0        0        0     2722 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     2519 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/vault/testcontainers/vault/__init__.py
--rw-r--r--   0        0        0     5588 2024-04-08 09:28:03.317967 testcontainers-4.3.2/modules/weaviate/testcontainers/weaviate/__init__.py
--rw-r--r--   0        0        0     8731 2024-04-08 09:28:03.317967 testcontainers-4.3.2/pyproject.toml
--rw-r--r--   0        0        0     5495 1970-01-01 00:00:00.000000 testcontainers-4.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-04-09 13:54:24.560508 testcontainers-4.3.3/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-04-09 13:54:24.560508 testcontainers-4.3.3/README.md
+-rw-r--r--   0        0        0      172 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0     2433 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     7590 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     6839 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2418 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      516 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     2088 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4091 2024-04-09 13:54:24.560508 testcontainers-4.3.3/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3781 2024-04-09 13:54:24.560508 testcontainers-4.3.3/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3760 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2694 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     3313 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     4116 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     1809 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-09 13:54:24.564508 testcontainers-4.3.3/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2782 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4109 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2810 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3984 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5209 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2967 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     2722 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     2519 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/vault/testcontainers/vault/__init__.py
+-rw-r--r--   0        0        0     5588 2024-04-09 13:54:24.568508 testcontainers-4.3.3/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8755 2024-04-09 13:54:24.572508 testcontainers-4.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5528 1970-01-01 00:00:00.000000 testcontainers-4.3.3/PKG-INFO
```

### Comparing `testcontainers-4.3.2/LICENSE.txt` & `testcontainers-4.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/README.md` & `testcontainers-4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/compose/compose.py` & `testcontainers-4.3.3/core/testcontainers/compose/compose.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/config.py` & `testcontainers-4.3.3/core/testcontainers/core/config.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/container.py` & `testcontainers-4.3.3/core/testcontainers/core/container.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/docker_client.py` & `testcontainers-4.3.3/core/testcontainers/core/docker_client.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/exceptions.py` & `testcontainers-4.3.3/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/generic.py` & `testcontainers-4.3.3/core/testcontainers/core/generic.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/labels.py` & `testcontainers-4.3.3/core/testcontainers/core/labels.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/utils.py` & `testcontainers-4.3.3/core/testcontainers/core/utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.3.3/core/testcontainers/core/waiting_utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.3.3/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.3.3/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/cassandra/testcontainers/cassandra/__init__.py` & `testcontainers-4.3.3/modules/cassandra/testcontainers/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/chroma/testcontainers/chroma/__init__.py` & `testcontainers-4.3.3/modules/chroma/testcontainers/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.3.3/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.3.3/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/google/testcontainers/google/datastore.py` & `testcontainers-4.3.3/modules/google/testcontainers/google/datastore.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.3.3/modules/google/testcontainers/google/pubsub.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.3.3/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.3.3/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.3.3/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/kafka/testcontainers/kafka/_redpanda.py` & `testcontainers-4.3.3/modules/kafka/testcontainers/kafka/_redpanda.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.3.3/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.3.3/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.3.3/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.3.3/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/mssql/testcontainers/mssql/__init__.py` & `testcontainers-4.3.3/modules/mssql/testcontainers/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/mysql/testcontainers/mysql/__init__.py` & `testcontainers-4.3.3/modules/mysql/testcontainers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/nats/testcontainers/nats/__init__.py` & `testcontainers-4.3.3/modules/nats/testcontainers/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.3.3/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.3.3/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.3.3/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/oracle-free/testcontainers/oracle/__init__.py` & `testcontainers-4.3.3/modules/oracle-free/testcontainers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.3.3/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/qdrant/testcontainers/qdrant/__init__.py` & `testcontainers-4.3.3/modules/qdrant/testcontainers/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.3.3/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.3.3/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/registry/testcontainers/registry/__init__.py` & `testcontainers-4.3.3/modules/registry/testcontainers/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.3.3/modules/selenium/testcontainers/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/vault/testcontainers/vault/__init__.py` & `testcontainers-4.3.3/modules/vault/testcontainers/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/modules/weaviate/testcontainers/weaviate/__init__.py` & `testcontainers-4.3.3/modules/weaviate/testcontainers/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.3.2/pyproject.toml` & `testcontainers-4.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.3.2"  # auto-incremented by release-please
+version = "4.3.3"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
     "David Ankin <daveankin@gmail.com>",
     "Vemund Santi <vemund@santi.no>"
 ]
@@ -64,14 +64,15 @@
 "Issue Tracker" = "https://github.com/testcontainers/testcontainers-python/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 docker = "*" # ">=4.0"
 urllib3 = "*" # "<2.0"
 wrapt = "*" # "^1.16.0"
+typing-extensions = "*"
 
 # community modules
 python-arango = { version = "^7.8", optional = true }
 azure-storage-blob = { version = "^12.19", optional = true }
 clickhouse-driver = { version = "*", optional = true }
 google-cloud-pubsub = { version = ">=2", optional = true }
 google-cloud-datastore = { version = ">=2", optional = true }
```

### Comparing `testcontainers-4.3.2/PKG-INFO` & `testcontainers-4.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.3.2
+Version: 4.3.3
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -74,14 +74,15 @@
 Requires-Dist: python-arango (>=7.8,<8.0) ; extra == "arangodb"
 Requires-Dist: python-keycloak ; extra == "keycloak"
 Requires-Dist: pyyaml ; extra == "k3s"
 Requires-Dist: qdrant-client ; extra == "qdrant"
 Requires-Dist: redis ; extra == "redis"
 Requires-Dist: selenium ; extra == "selenium"
 Requires-Dist: sqlalchemy ; extra == "mssql" or extra == "mysql" or extra == "oracle" or extra == "oracle-free"
+Requires-Dist: typing-extensions
 Requires-Dist: urllib3
 Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate"
 Requires-Dist: wrapt
 Project-URL: GitHub, https://github.com/testcontainers/testcontainers-python
 Project-URL: Issue Tracker, https://github.com/testcontainers/testcontainers-python/issues
 Description-Content-Type: text/markdown
```

