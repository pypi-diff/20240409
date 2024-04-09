# Comparing `tmp/pulumi_ovh-0.40.1.tar.gz` & `tmp/pulumi_ovh-0.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ovh-0.40.1.tar", last modified: Tue Mar 26 10:30:34 2024, max compression
+gzip compressed data, was "pulumi_ovh-0.42.0.tar", last modified: Tue Apr  9 11:35:05 2024, max compression
```

## Comparing `pulumi_ovh-0.40.1.tar` & `pulumi_ovh-0.42.0.tar`

### file list

```diff
@@ -1,259 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.711817 pulumi_ovh-0.40.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-26 10:30:34.711817 pulumi_ovh-0.40.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.679817 pulumi_ovh-0.40.1/pulumi_ovh/
--rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.687817 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75053 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/alerting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    39886 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    57293 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/failover_ip_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_capabilities_container_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_capabilities_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registries.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_failover_ip_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_m3db_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_m3db_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_m3db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_mongo_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_open_search_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_open_search_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_open_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user_s3_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user_s3_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user_s3_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_v_rack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46082 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    56647 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    31338 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/network_private.py
--rw-r--r--   0 runner    (1001) docker     (127)    28355 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/network_private_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    90734 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/region_storage_presign.py
--rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/s3_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/s3_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/workflow_backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.691817 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/database_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17077 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/ip_restriction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23063 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    35161 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    17453 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/m3_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    22403 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/opensearch_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21207 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    23948 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/redis_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.691817 pulumi_ovh-0.40.1/pulumi_ovh/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.695817 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_input_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    16806 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/logs_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/logs_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    46041 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/logs_output_graylog_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dbaas/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.695817 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/ceph_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_ceph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_nas_ha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_server_boots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_server_specifications_hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    16472 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/nas_ha_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12792 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/nas_ha_partition_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17175 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_install_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_reboot_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.699817 pulumi_ovh-0.40.1/pulumi_ovh/domain/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25381 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/zone_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/domain/zone_redirection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/get_installation_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/get_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/get_vrack_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.699817 pulumi_ovh-0.40.1/pulumi_ovh/hosting/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_user_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42087 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_user_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.699817 pulumi_ovh-0.40.1/pulumi_ovh/iam/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_permissions_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_permissions_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_reference_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_reference_resource_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_resource_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/get_resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/permissions_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iam/resource_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.703817 pulumi_ovh-0.40.1/pulumi_ovh/ip/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    27412 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/ip_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/move.py
--rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/ip/reverse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.703817 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/get_vrack_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_farm_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_route_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    39241 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    21453 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_farm_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_route_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/vrack_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.707817 pulumi_ovh-0.40.1/pulumi_ovh/me/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/apio_auth2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_apio_auth2_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_apio_auth2_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_installation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_installation_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_paymentmean_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_paymentmean_credit_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/identity_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35246 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template_partition_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
--rw-r--r--   0 runner    (1001) docker     (127)    26052 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template_partition_scheme_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/me/ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.707817 pulumi_ovh-0.40.1/pulumi_ovh/order/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product_options_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    38797 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/order/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.711817 pulumi_ovh-0.40.1/pulumi_ovh/vps/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vps/get_vps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vps/get_vpss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.711817 pulumi_ovh-0.40.1/pulumi_ovh/vrack/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/cloud_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/dedicated_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/dedicated_server_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/get_vracks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/ip_loadbalancing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23900 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh/vrack/vrack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:30:34.679817 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/pulumi_ovh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 10:30:34.711817 pulumi_ovh-0.40.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-26 10:30:34.000000 pulumi_ovh-0.40.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.586086 pulumi_ovh-0.42.0/pulumi_ovh/
+-rw-r--r--   0 runner    (1001) docker     (127)    20078 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.586086 pulumi_ovh-0.42.0/pulumi_ovh/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloud/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.598086 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76758 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39886 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60837 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/failover_ip_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_mongo_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_v_rack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46082 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56647 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31338 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22208 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28355 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91949 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23676 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18373 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/region_storage_presign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12087 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/workflow_backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.606086 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/database_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14208 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23623 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23063 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22898 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/log_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35161 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17453 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22403 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18564 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21197 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23948 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/redis_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.606086 pulumi_ovh-0.42.0/pulumi_ovh/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.606086 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_input_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31288 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45978 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dbaas/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.610086 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/ceph_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_ceph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_nas_ha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_boots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_install_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10502 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15716 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_reboot_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.610086 pulumi_ovh-0.42.0/pulumi_ovh/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13079 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11746 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25381 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16657 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_redirection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_installation_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15051 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/get_vrack_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.614086 pulumi_ovh-0.42.0/pulumi_ovh/hosting/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14071 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42087 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13743 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.614086 pulumi_ovh-0.42.0/pulumi_ovh/iam/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18506 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/permissions_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28002 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iam/resource_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.618086 pulumi_ovh-0.42.0/pulumi_ovh/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29412 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27412 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/ip_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20383 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/ip/reverse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.622086 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35579 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13567 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_vrack_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31891 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39241 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21453 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30831 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27680 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17644 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21386 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/udp_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/vrack_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.626086 pulumi_ovh-0.42.0/pulumi_ovh/me/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18551 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/apio_auth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7141 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_credit_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/identity_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32374 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26052 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/me/ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.626086 pulumi_ovh-0.42.0/pulumi_ovh/order/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8586 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/order/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.626086 pulumi_ovh-0.42.0/pulumi_ovh/vps/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21804 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vpss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18960 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37896 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vps/vps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/pulumi_ovh/vrack/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/cloud_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/get_vracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_loadbalancing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23900 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh/vrack/vrack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:35:05.586086 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/pulumi_ovh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:35:05.630086 pulumi_ovh-0.42.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 11:35:05.000000 pulumi_ovh-0.42.0/setup.py
```

### Comparing `pulumi_ovh-0.40.1/PKG-INFO` & `pulumi_ovh-0.42.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ovh
-Version: 0.40.1
+Version: 0.42.0
 Summary: A Pulumi package for creating and managing OVH resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ovh/pulumi-ovh
 Keywords: pulumi ovh category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_ovh Version: 0.40.1 Summary: A Pulumi
+Metadata-Version: 2.1 Name: pulumi_ovh Version: 0.42.0 Summary: A Pulumi
 package for creating and managing OVH resources. Home-page: https://
 www.pulumi.com License: Apache-2.0 Project-URL: Repository, https://github.com/
 ovh/pulumi-ovh Keywords: pulumi ovh category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown # OVH Resource Provider
 The OVH Resource Provider lets you manage [OVHcloud](https://www.ovhcloud.com/
 en/) resources. _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_][![GoDoc](https://godoc.org/github.com/ovh/
 pulumi-ovh?status.svg)](https://pkg.go.dev/github.com/ovh/pulumi-ovh/sdk) [!
```

### Comparing `pulumi_ovh-0.40.1/README.md` & `pulumi_ovh-0.42.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .get_servers import *
 from .get_vrack_networks import *
 from .provider import *
 from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
+    import pulumi_ovh.cloud as __cloud
+    cloud = __cloud
     import pulumi_ovh.cloudproject as __cloudproject
     cloudproject = __cloudproject
     import pulumi_ovh.cloudprojectdatabase as __cloudprojectdatabase
     cloudprojectdatabase = __cloudprojectdatabase
     import pulumi_ovh.config as __config
     config = __config
     import pulumi_ovh.dbaas as __dbaas
@@ -39,14 +41,15 @@
     import pulumi_ovh.order as __order
     order = __order
     import pulumi_ovh.vps as __vps
     vps = __vps
     import pulumi_ovh.vrack as __vrack
     vrack = __vrack
 else:
+    cloud = _utilities.lazy_import('pulumi_ovh.cloud')
     cloudproject = _utilities.lazy_import('pulumi_ovh.cloudproject')
     cloudprojectdatabase = _utilities.lazy_import('pulumi_ovh.cloudprojectdatabase')
     config = _utilities.lazy_import('pulumi_ovh.config')
     dbaas = _utilities.lazy_import('pulumi_ovh.dbaas')
     dedicated = _utilities.lazy_import('pulumi_ovh.dedicated')
     domain = _utilities.lazy_import('pulumi_ovh.domain')
     hosting = _utilities.lazy_import('pulumi_ovh.hosting')
@@ -275,14 +278,22 @@
   "fqn": "pulumi_ovh.cloudprojectdatabase",
   "classes": {
    "ovh:CloudProjectDatabase/kafkaTopic:KafkaTopic": "KafkaTopic"
   }
  },
  {
   "pkg": "ovh",
+  "mod": "CloudProjectDatabase/logSubscription",
+  "fqn": "pulumi_ovh.cloudprojectdatabase",
+  "classes": {
+   "ovh:CloudProjectDatabase/logSubscription:LogSubscription": "LogSubscription"
+  }
+ },
+ {
+  "pkg": "ovh",
   "mod": "CloudProjectDatabase/m3DbNamespace",
   "fqn": "pulumi_ovh.cloudprojectdatabase",
   "classes": {
    "ovh:CloudProjectDatabase/m3DbNamespace:M3DbNamespace": "M3DbNamespace"
   }
  },
  {
@@ -443,14 +454,22 @@
   "fqn": "pulumi_ovh.domain",
   "classes": {
    "ovh:Domain/zone:Zone": "Zone"
   }
  },
  {
   "pkg": "ovh",
+  "mod": "Domain/zoneDNSSec",
+  "fqn": "pulumi_ovh.domain",
+  "classes": {
+   "ovh:Domain/zoneDNSSec:ZoneDNSSec": "ZoneDNSSec"
+  }
+ },
+ {
+  "pkg": "ovh",
   "mod": "Domain/zoneRecord",
   "fqn": "pulumi_ovh.domain",
   "classes": {
    "ovh:Domain/zoneRecord:ZoneRecord": "ZoneRecord"
   }
  },
  {
@@ -523,22 +542,46 @@
   "fqn": "pulumi_ovh.iam",
   "classes": {
    "ovh:Iam/resourceGroup:ResourceGroup": "ResourceGroup"
   }
  },
  {
   "pkg": "ovh",
+  "mod": "Ip/firewall",
+  "fqn": "pulumi_ovh.ip",
+  "classes": {
+   "ovh:Ip/firewall:Firewall": "Firewall"
+  }
+ },
+ {
+  "pkg": "ovh",
+  "mod": "Ip/firewallRule",
+  "fqn": "pulumi_ovh.ip",
+  "classes": {
+   "ovh:Ip/firewallRule:FirewallRule": "FirewallRule"
+  }
+ },
+ {
+  "pkg": "ovh",
   "mod": "Ip/ipService",
   "fqn": "pulumi_ovh.ip",
   "classes": {
    "ovh:Ip/ipService:IpService": "IpService"
   }
  },
  {
   "pkg": "ovh",
+  "mod": "Ip/mitigation",
+  "fqn": "pulumi_ovh.ip",
+  "classes": {
+   "ovh:Ip/mitigation:Mitigation": "Mitigation"
+  }
+ },
+ {
+  "pkg": "ovh",
   "mod": "Ip/move",
   "fqn": "pulumi_ovh.ip",
   "classes": {
    "ovh:Ip/move:Move": "Move"
   }
  },
  {
@@ -643,14 +686,22 @@
   "fqn": "pulumi_ovh.iploadbalancing",
   "classes": {
    "ovh:IpLoadBalancing/tcpRouteRule:TcpRouteRule": "TcpRouteRule"
   }
  },
  {
   "pkg": "ovh",
+  "mod": "IpLoadBalancing/udpFrontend",
+  "fqn": "pulumi_ovh.iploadbalancing",
+  "classes": {
+   "ovh:IpLoadBalancing/udpFrontend:UdpFrontend": "UdpFrontend"
+  }
+ },
+ {
+  "pkg": "ovh",
   "mod": "IpLoadBalancing/vrackNetwork",
   "fqn": "pulumi_ovh.iploadbalancing",
   "classes": {
    "ovh:IpLoadBalancing/vrackNetwork:VrackNetwork": "VrackNetwork"
   }
  },
  {
@@ -715,14 +766,22 @@
   "fqn": "pulumi_ovh.me",
   "classes": {
    "ovh:Me/sshKey:SshKey": "SshKey"
   }
  },
  {
   "pkg": "ovh",
+  "mod": "Vps/vps",
+  "fqn": "pulumi_ovh.vps",
+  "classes": {
+   "ovh:Vps/vps:Vps": "Vps"
+  }
+ },
+ {
+  "pkg": "ovh",
   "mod": "Vrack/cloudProject",
   "fqn": "pulumi_ovh.vrack",
   "classes": {
    "ovh:Vrack/cloudProject:CloudProject": "CloudProject"
   }
  },
  {
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/_utilities.py` & `pulumi_ovh-0.42.0/pulumi_ovh/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 __all__ = [
     'AlertingFormattedMonthlyThresholdArgs',
     'ContainerRegistryPlanArgs',
     'ContainerRegistryPlanFeatureArgs',
     'ContainerRegistryPlanRegistryLimitArgs',
     'DatabaseEndpointArgs',
+    'DatabaseIpRestrictionArgs',
     'DatabaseNodeArgs',
     'KubeCustomizationArgs',
     'KubeCustomizationApiserverArgs',
     'KubeCustomizationApiserverAdmissionpluginArgs',
     'KubeCustomizationKubeProxyArgs',
     'KubeCustomizationKubeProxyIptablesArgs',
     'KubeCustomizationKubeProxyIpvsArgs',
@@ -416,14 +417,69 @@
 
     @uri.setter
     def uri(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "uri", value)
 
 
 @pulumi.input_type
+class DatabaseIpRestrictionArgs:
+    def __init__(__self__, *,
+                 description: Optional[pulumi.Input[str]] = None,
+                 ip: Optional[pulumi.Input[str]] = None,
+                 status: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] description: Description of the IP restriction
+        :param pulumi.Input[str] ip: Authorized IP
+        :param pulumi.Input[str] status: Current status of the cluster.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        """
+        Description of the IP restriction
+        """
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+    @property
+    @pulumi.getter
+    def ip(self) -> Optional[pulumi.Input[str]]:
+        """
+        Authorized IP
+        """
+        return pulumi.get(self, "ip")
+
+    @ip.setter
+    def ip(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ip", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
+        """
+        Current status of the cluster.
+        """
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
+
+@pulumi.input_type
 class DatabaseNodeArgs:
     def __init__(__self__, *,
                  region: pulumi.Input[str],
                  network_id: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] region: Public cloud region in which the node should be deployed.
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/alerting.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/alerting.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_oidc.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/container_registry_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/container_registry_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/database.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
                  service_name: pulumi.Input[str],
                  version: pulumi.Input[str],
                  advanced_configuration: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  backup_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  backup_time: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
+                 ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Database resource.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
@@ -45,16 +46,17 @@
                * Redis: "essential", "business"
         :param pulumi.Input[str] service_name: The id of the public cloud project. If omitted,
                the `OVH_CLOUD_PROJECT_SERVICE` environment variable is used.
         :param pulumi.Input[str] version: The version of the engine in which the service should be deployed
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
-        :param pulumi.Input[str] description: Small description of the database service.
+        :param pulumi.Input[str] description: Description of the IP restriction
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
+        :param pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         """
         pulumi.set(__self__, "engine", engine)
         pulumi.set(__self__, "flavor", flavor)
         pulumi.set(__self__, "nodes", nodes)
         pulumi.set(__self__, "plan", plan)
@@ -66,14 +68,16 @@
             pulumi.set(__self__, "backup_regions", backup_regions)
         if backup_time is not None:
             pulumi.set(__self__, "backup_time", backup_time)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
+        if ip_restrictions is not None:
+            pulumi.set(__self__, "ip_restrictions", ip_restrictions)
         if kafka_rest_api is not None:
             pulumi.set(__self__, "kafka_rest_api", kafka_rest_api)
         if opensearch_acls_enabled is not None:
             pulumi.set(__self__, "opensearch_acls_enabled", opensearch_acls_enabled)
 
     @property
     @pulumi.getter
@@ -192,15 +196,15 @@
     def backup_time(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "backup_time", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Small description of the database service.
+        Description of the IP restriction
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -213,14 +217,26 @@
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
+    @pulumi.getter(name="ipRestrictions")
+    def ip_restrictions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]]:
+        """
+        IP Blocks authorized to access to the cluster.
+        """
+        return pulumi.get(self, "ip_restrictions")
+
+    @ip_restrictions.setter
+    def ip_restrictions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]]):
+        pulumi.set(self, "ip_restrictions", value)
+
+    @property
     @pulumi.getter(name="kafkaRestApi")
     def kafka_rest_api(self) -> Optional[pulumi.Input[bool]]:
         """
         Defines whether the REST API is enabled on a kafka cluster
         """
         return pulumi.get(self, "kafka_rest_api")
 
@@ -250,14 +266,15 @@
                  created_at: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  disk_type: Optional[pulumi.Input[str]] = None,
                  endpoints: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseEndpointArgs']]]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  flavor: Optional[pulumi.Input[str]] = None,
+                 ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
                  maintenance_time: Optional[pulumi.Input[str]] = None,
                  network_type: Optional[pulumi.Input[str]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseNodeArgs']]]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
@@ -265,23 +282,24 @@
                  version: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Database resources.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
         :param pulumi.Input[str] created_at: Date of the creation of the cluster.
-        :param pulumi.Input[str] description: Small description of the database service.
+        :param pulumi.Input[str] description: Description of the IP restriction
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[str] disk_type: Defines the disk type of the database service.
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseEndpointArgs']]] endpoints: List of all endpoints objects of the service.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
+        :param pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
         :param pulumi.Input[str] maintenance_time: Time on which maintenances can start every day.
         :param pulumi.Input[str] network_type: Type of network of the cluster.
         :param pulumi.Input[Sequence[pulumi.Input['DatabaseNodeArgs']]] nodes: List of nodes object.
                Multi region cluster are not yet available, all node should be identical.
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         :param pulumi.Input[str] plan: Plan of the cluster.
@@ -310,14 +328,16 @@
             pulumi.set(__self__, "disk_type", disk_type)
         if endpoints is not None:
             pulumi.set(__self__, "endpoints", endpoints)
         if engine is not None:
             pulumi.set(__self__, "engine", engine)
         if flavor is not None:
             pulumi.set(__self__, "flavor", flavor)
+        if ip_restrictions is not None:
+            pulumi.set(__self__, "ip_restrictions", ip_restrictions)
         if kafka_rest_api is not None:
             pulumi.set(__self__, "kafka_rest_api", kafka_rest_api)
         if maintenance_time is not None:
             pulumi.set(__self__, "maintenance_time", maintenance_time)
         if network_type is not None:
             pulumi.set(__self__, "network_type", network_type)
         if nodes is not None:
@@ -381,15 +401,15 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Small description of the database service.
+        Description of the IP restriction
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -453,14 +473,26 @@
         return pulumi.get(self, "flavor")
 
     @flavor.setter
     def flavor(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "flavor", value)
 
     @property
+    @pulumi.getter(name="ipRestrictions")
+    def ip_restrictions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]]:
+        """
+        IP Blocks authorized to access to the cluster.
+        """
+        return pulumi.get(self, "ip_restrictions")
+
+    @ip_restrictions.setter
+    def ip_restrictions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['DatabaseIpRestrictionArgs']]]]):
+        pulumi.set(self, "ip_restrictions", value)
+
+    @property
     @pulumi.getter(name="kafkaRestApi")
     def kafka_rest_api(self) -> Optional[pulumi.Input[bool]]:
         """
         Defines whether the REST API is enabled on a kafka cluster
         """
         return pulumi.get(self, "kafka_rest_api")
 
@@ -579,14 +611,15 @@
                  advanced_configuration: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  backup_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  backup_time: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  flavor: Optional[pulumi.Input[str]] = None,
+                 ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -687,15 +720,25 @@
             description="my-first-postgresql",
             engine="postgresql",
             version="14",
             plan="essential",
             nodes=[ovh.cloud_project.DatabaseNodeArgs(
                 region="WAW",
             )],
-            flavor="db1-4")
+            flavor="db1-4",
+            ip_restrictions=[
+                ovh.cloud_project.DatabaseIpRestrictionArgs(
+                    description="ip 1",
+                    ip="178.97.6.0/24",
+                ),
+                ovh.cloud_project.DatabaseIpRestrictionArgs(
+                    description="ip 2",
+                    ip="178.97.7.0/24",
+                ),
+            ])
         redisdb = ovh.cloud_project.Database("redisdb",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             description="my-first-redis",
             engine="redis",
             version="6.2",
             plan="essential",
             nodes=[ovh.cloud_project.DatabaseNodeArgs(
@@ -785,21 +828,22 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
-        :param pulumi.Input[str] description: Small description of the database service.
+        :param pulumi.Input[str] description: Description of the IP restriction
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]] nodes: List of nodes object.
                Multi region cluster are not yet available, all node should be identical.
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         :param pulumi.Input[str] plan: Plan of the cluster.
                * MongoDB: Enum: "discovery", "production", "advanced".
                * Mysql, PosgreSQL, Cassandra, M3DB, : Enum: "essential", "business", "enterprise".
@@ -912,15 +956,25 @@
             description="my-first-postgresql",
             engine="postgresql",
             version="14",
             plan="essential",
             nodes=[ovh.cloud_project.DatabaseNodeArgs(
                 region="WAW",
             )],
-            flavor="db1-4")
+            flavor="db1-4",
+            ip_restrictions=[
+                ovh.cloud_project.DatabaseIpRestrictionArgs(
+                    description="ip 1",
+                    ip="178.97.6.0/24",
+                ),
+                ovh.cloud_project.DatabaseIpRestrictionArgs(
+                    description="ip 2",
+                    ip="178.97.7.0/24",
+                ),
+            ])
         redisdb = ovh.cloud_project.Database("redisdb",
             service_name="xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
             description="my-first-redis",
             engine="redis",
             version="6.2",
             plan="essential",
             nodes=[ovh.cloud_project.DatabaseNodeArgs(
@@ -1027,14 +1081,15 @@
                  advanced_configuration: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  backup_regions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  backup_time: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  flavor: Optional[pulumi.Input[str]] = None,
+                 ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]]] = None,
                  kafka_rest_api: Optional[pulumi.Input[bool]] = None,
                  nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]]] = None,
                  opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
                  plan: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
@@ -1053,14 +1108,15 @@
             __props__.__dict__["disk_size"] = disk_size
             if engine is None and not opts.urn:
                 raise TypeError("Missing required property 'engine'")
             __props__.__dict__["engine"] = engine
             if flavor is None and not opts.urn:
                 raise TypeError("Missing required property 'flavor'")
             __props__.__dict__["flavor"] = flavor
+            __props__.__dict__["ip_restrictions"] = ip_restrictions
             __props__.__dict__["kafka_rest_api"] = kafka_rest_api
             if nodes is None and not opts.urn:
                 raise TypeError("Missing required property 'nodes'")
             __props__.__dict__["nodes"] = nodes
             __props__.__dict__["opensearch_acls_enabled"] = opensearch_acls_enabled
             if plan is None and not opts.urn:
                 raise TypeError("Missing required property 'plan'")
@@ -1093,14 +1149,15 @@
             created_at: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             disk_size: Optional[pulumi.Input[int]] = None,
             disk_type: Optional[pulumi.Input[str]] = None,
             endpoints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseEndpointArgs']]]]] = None,
             engine: Optional[pulumi.Input[str]] = None,
             flavor: Optional[pulumi.Input[str]] = None,
+            ip_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]]] = None,
             kafka_rest_api: Optional[pulumi.Input[bool]] = None,
             maintenance_time: Optional[pulumi.Input[str]] = None,
             network_type: Optional[pulumi.Input[str]] = None,
             nodes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]]] = None,
             opensearch_acls_enabled: Optional[pulumi.Input[bool]] = None,
             plan: Optional[pulumi.Input[str]] = None,
             service_name: Optional[pulumi.Input[str]] = None,
@@ -1113,23 +1170,24 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] advanced_configuration: Advanced configuration key / value.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] backup_regions: List of region where backups are pushed. Not more than 1 regions for MongoDB. Not more than 2 regions for the other engines with one being the same as the nodes[].region field
         :param pulumi.Input[str] backup_time: Time on which backups start every day.
         :param pulumi.Input[str] created_at: Date of the creation of the cluster.
-        :param pulumi.Input[str] description: Small description of the database service.
+        :param pulumi.Input[str] description: Description of the IP restriction
         :param pulumi.Input[int] disk_size: The disk size (in GB) of the database service.
         :param pulumi.Input[str] disk_type: Defines the disk type of the database service.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseEndpointArgs']]]] endpoints: List of all endpoints objects of the service.
         :param pulumi.Input[str] engine: The database engine you want to deploy. To get a full list of available engine visit.
                [public documentation](https://docs.ovh.com/gb/en/publiccloud/databases).
         :param pulumi.Input[str] flavor: A valid OVHcloud public cloud database flavor name in which the nodes will be started.
                Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
                You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseIpRestrictionArgs']]]] ip_restrictions: IP Blocks authorized to access to the cluster.
         :param pulumi.Input[bool] kafka_rest_api: Defines whether the REST API is enabled on a kafka cluster
         :param pulumi.Input[str] maintenance_time: Time on which maintenances can start every day.
         :param pulumi.Input[str] network_type: Type of network of the cluster.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DatabaseNodeArgs']]]] nodes: List of nodes object.
                Multi region cluster are not yet available, all node should be identical.
         :param pulumi.Input[bool] opensearch_acls_enabled: Defines whether the ACLs are enabled on an OpenSearch cluster
         :param pulumi.Input[str] plan: Plan of the cluster.
@@ -1152,14 +1210,15 @@
         __props__.__dict__["created_at"] = created_at
         __props__.__dict__["description"] = description
         __props__.__dict__["disk_size"] = disk_size
         __props__.__dict__["disk_type"] = disk_type
         __props__.__dict__["endpoints"] = endpoints
         __props__.__dict__["engine"] = engine
         __props__.__dict__["flavor"] = flavor
+        __props__.__dict__["ip_restrictions"] = ip_restrictions
         __props__.__dict__["kafka_rest_api"] = kafka_rest_api
         __props__.__dict__["maintenance_time"] = maintenance_time
         __props__.__dict__["network_type"] = network_type
         __props__.__dict__["nodes"] = nodes
         __props__.__dict__["opensearch_acls_enabled"] = opensearch_acls_enabled
         __props__.__dict__["plan"] = plan
         __props__.__dict__["service_name"] = service_name
@@ -1199,15 +1258,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Small description of the database service.
+        Description of the IP restriction
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> pulumi.Output[int]:
         """
@@ -1247,14 +1306,22 @@
         A valid OVHcloud public cloud database flavor name in which the nodes will be started.
         Ex: "db1-7". Changing this value upgrade the nodes with the new flavor.
         You can find the list of flavor names: https://www.ovhcloud.com/fr/public-cloud/prices/
         """
         return pulumi.get(self, "flavor")
 
     @property
+    @pulumi.getter(name="ipRestrictions")
+    def ip_restrictions(self) -> pulumi.Output[Optional[Sequence['outputs.DatabaseIpRestriction']]]:
+        """
+        IP Blocks authorized to access to the cluster.
+        """
+        return pulumi.get(self, "ip_restrictions")
+
+    @property
     @pulumi.getter(name="kafkaRestApi")
     def kafka_rest_api(self) -> pulumi.Output[Optional[bool]]:
         """
         Defines whether the REST API is enabled on a kafka cluster
         """
         return pulumi.get(self, "kafka_rest_api")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/failover_ip_attach.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/failover_ip_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/gateway.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_capabilities_container_filter.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_filter.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_capabilities_container_registry.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_capabilities_container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registries.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registries.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_management.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_ip_restrictions_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_oidc.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_container_registry_users.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_container_registry_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_failover_ip_attach.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_failover_ip_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_ip_restrictions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_node_pool.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_node_pool_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_nodes.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_kube_oidc.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_kube_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_m3db_namespace.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_m3db_namespaces.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_namespaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_m3db_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_m3db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_mongo_db_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_mongo_db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_open_search_pattern.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_open_search_patterns.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_patterns.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_open_search_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_open_search_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_redis_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_region.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_regions.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user_s3_credential.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user_s3_credentials.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_user_s3_policy.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_user_s3_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_users.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/get_v_rack.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/get_v_rack.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube_ip_restrictions.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_ip_restrictions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube_node_pool.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/kube_oidc.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/kube_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/network_private.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/network_private_subnet.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/network_private_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 __all__ = [
     'AlertingFormattedMonthlyThreshold',
     'ContainerRegistryPlan',
     'ContainerRegistryPlanFeature',
     'ContainerRegistryPlanRegistryLimit',
     'DatabaseEndpoint',
+    'DatabaseIpRestriction',
     'DatabaseNode',
     'KubeCustomization',
     'KubeCustomizationApiserver',
     'KubeCustomizationApiserverAdmissionplugin',
     'KubeCustomizationKubeProxy',
     'KubeCustomizationKubeProxyIptables',
     'KubeCustomizationKubeProxyIpvs',
@@ -422,14 +423,57 @@
         """
         URI of the endpoint.
         """
         return pulumi.get(self, "uri")
 
 
 @pulumi.output_type
+class DatabaseIpRestriction(dict):
+    def __init__(__self__, *,
+                 description: Optional[str] = None,
+                 ip: Optional[str] = None,
+                 status: Optional[str] = None):
+        """
+        :param str description: Description of the IP restriction
+        :param str ip: Authorized IP
+        :param str status: Current status of the cluster.
+        """
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if ip is not None:
+            pulumi.set(__self__, "ip", ip)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[str]:
+        """
+        Description of the IP restriction
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def ip(self) -> Optional[str]:
+        """
+        Authorized IP
+        """
+        return pulumi.get(self, "ip")
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional[str]:
+        """
+        Current status of the cluster.
+        """
+        return pulumi.get(self, "status")
+
+
+@pulumi.output_type
 class DatabaseNode(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "networkId":
             suggest = "network_id"
         elif key == "subnetId":
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/project.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/region_storage_presign.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/region_storage_presign.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/s3_credential.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/s3_policy.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/s3_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudproject/workflow_backup.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudproject/workflow_backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from .get_capabilities import *
 from .get_certificates import *
 from .get_database import *
 from .get_database_instance import *
 from .get_database_instances import *
 from .get_database_integration import *
 from .get_database_integrations import *
+from .get_database_log_subscription import *
+from .get_database_log_subscriptions import *
+from .get_database_postgre_sql_connection_pools import *
 from .get_databases import *
 from .get_ip_restrictions import *
 from .get_kafka_acl import *
 from .get_kafka_acls import *
 from .get_kafka_schema_registry_acl import *
 from .get_kafka_schema_registry_acls import *
 from .get_kafka_topic import *
@@ -27,14 +30,15 @@
 from .get_user import *
 from .get_users import *
 from .integration import *
 from .ip_restriction import *
 from .kafka_acl import *
 from .kafka_schema_registry_acl import *
 from .kafka_topic import *
+from .log_subscription import *
 from .m3_db_namespace import *
 from .m3_db_user import *
 from .mongo_db_user import *
 from .opensearch_pattern import *
 from .opensearch_user import *
 from .postgres_sql_connection_pool import *
 from .postgres_sql_user import *
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/database_instance.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_capabilities.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_capabilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_certificates.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_certificates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetDatabaseResult:
     """
     A collection of values returned by getDatabase.
     """
-    def __init__(__self__, advanced_configuration=None, backup_regions=None, backup_time=None, created_at=None, description=None, disk_size=None, disk_type=None, endpoints=None, engine=None, flavor=None, id=None, kafka_rest_api=None, maintenance_time=None, network_type=None, nodes=None, opensearch_acls_enabled=None, plan=None, service_name=None, status=None, version=None):
+    def __init__(__self__, advanced_configuration=None, backup_regions=None, backup_time=None, created_at=None, description=None, disk_size=None, disk_type=None, endpoints=None, engine=None, flavor=None, id=None, ip_restrictions=None, kafka_rest_api=None, maintenance_time=None, network_type=None, nodes=None, opensearch_acls_enabled=None, plan=None, service_name=None, status=None, version=None):
         if advanced_configuration and not isinstance(advanced_configuration, dict):
             raise TypeError("Expected argument 'advanced_configuration' to be a dict")
         pulumi.set(__self__, "advanced_configuration", advanced_configuration)
         if backup_regions and not isinstance(backup_regions, list):
             raise TypeError("Expected argument 'backup_regions' to be a list")
         pulumi.set(__self__, "backup_regions", backup_regions)
         if backup_time and not isinstance(backup_time, str):
@@ -52,14 +52,17 @@
         pulumi.set(__self__, "engine", engine)
         if flavor and not isinstance(flavor, str):
             raise TypeError("Expected argument 'flavor' to be a str")
         pulumi.set(__self__, "flavor", flavor)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
+        if ip_restrictions and not isinstance(ip_restrictions, list):
+            raise TypeError("Expected argument 'ip_restrictions' to be a list")
+        pulumi.set(__self__, "ip_restrictions", ip_restrictions)
         if kafka_rest_api and not isinstance(kafka_rest_api, bool):
             raise TypeError("Expected argument 'kafka_rest_api' to be a bool")
         pulumi.set(__self__, "kafka_rest_api", kafka_rest_api)
         if maintenance_time and not isinstance(maintenance_time, str):
             raise TypeError("Expected argument 'maintenance_time' to be a str")
         pulumi.set(__self__, "maintenance_time", maintenance_time)
         if network_type and not isinstance(network_type, str):
@@ -116,15 +119,15 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def description(self) -> str:
         """
-        Small description of the database service.
+        Description of the IP restriction
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="diskSize")
     def disk_size(self) -> int:
         """
@@ -169,14 +172,22 @@
     def id(self) -> str:
         """
         See Argument Reference above.
         """
         return pulumi.get(self, "id")
 
     @property
+    @pulumi.getter(name="ipRestrictions")
+    def ip_restrictions(self) -> Sequence['outputs.GetDatabaseIpRestrictionResult']:
+        """
+        IP Blocks authorized to access to the cluster.
+        """
+        return pulumi.get(self, "ip_restrictions")
+
+    @property
     @pulumi.getter(name="kafkaRestApi")
     def kafka_rest_api(self) -> bool:
         """
         Defines whether the REST API is enabled on a kafka cluster.
         """
         return pulumi.get(self, "kafka_rest_api")
 
@@ -255,14 +266,15 @@
             description=self.description,
             disk_size=self.disk_size,
             disk_type=self.disk_type,
             endpoints=self.endpoints,
             engine=self.engine,
             flavor=self.flavor,
             id=self.id,
+            ip_restrictions=self.ip_restrictions,
             kafka_rest_api=self.kafka_rest_api,
             maintenance_time=self.maintenance_time,
             network_type=self.network_type,
             nodes=self.nodes,
             opensearch_acls_enabled=self.opensearch_acls_enabled,
             plan=self.plan,
             service_name=self.service_name,
@@ -315,14 +327,15 @@
         description=pulumi.get(__ret__, 'description'),
         disk_size=pulumi.get(__ret__, 'disk_size'),
         disk_type=pulumi.get(__ret__, 'disk_type'),
         endpoints=pulumi.get(__ret__, 'endpoints'),
         engine=pulumi.get(__ret__, 'engine'),
         flavor=pulumi.get(__ret__, 'flavor'),
         id=pulumi.get(__ret__, 'id'),
+        ip_restrictions=pulumi.get(__ret__, 'ip_restrictions'),
         kafka_rest_api=pulumi.get(__ret__, 'kafka_rest_api'),
         maintenance_time=pulumi.get(__ret__, 'maintenance_time'),
         network_type=pulumi.get(__ret__, 'network_type'),
         nodes=pulumi.get(__ret__, 'nodes'),
         opensearch_acls_enabled=pulumi.get(__ret__, 'opensearch_acls_enabled'),
         plan=pulumi.get(__ret__, 'plan'),
         service_name=pulumi.get(__ret__, 'service_name'),
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_instance.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_instances.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_integration.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_database_integrations.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_databases.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,17 @@
 
 
 def get_ip_restrictions(cluster_id: Optional[str] = None,
                         engine: Optional[str] = None,
                         service_name: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetIpRestrictionsResult:
     """
-    Use the list of IP restrictions associated with a public cloud project.
+    Deprecated: Use ip_restrictions field in cloud_project_database datasource instead.
+
+    Use this data source to get the list of IP restrictions associated with a public cloud project.
 
     ## Example Usage
 
     To get the list of IP restriction on a database cluster service:
 
     <!--Start PulumiCodeChooser -->
     ```python
@@ -139,15 +141,17 @@
 
 @_utilities.lift_output_func(get_ip_restrictions)
 def get_ip_restrictions_output(cluster_id: Optional[pulumi.Input[str]] = None,
                                engine: Optional[pulumi.Input[str]] = None,
                                service_name: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIpRestrictionsResult]:
     """
-    Use the list of IP restrictions associated with a public cloud project.
+    Deprecated: Use ip_restrictions field in cloud_project_database datasource instead.
+
+    Use this data source to get the list of IP restrictions associated with a public cloud project.
 
     ## Example Usage
 
     To get the list of IP restriction on a database cluster service:
 
     <!--Start PulumiCodeChooser -->
     ```python
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_topics.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_kafka_user_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_connection_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_postgres_sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/get_users.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/integration.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/ip_restriction.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/ip_restriction.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,17 @@
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
                  ip: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        Deprecated: Use ip_restriction field in cloud_project_database resource instead.
+        Continuing to use the CloudProjectDatabase.IpRestriction resource to add an IP restriction to a cloud_project_database resource will cause the cloud_project_database resource to be updated on every apply
+
         Apply IP restrictions to an OVHcloud Managed Database cluster.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
@@ -262,14 +265,17 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: IpRestrictionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        Deprecated: Use ip_restriction field in cloud_project_database resource instead.
+        Continuing to use the CloudProjectDatabase.IpRestriction resource to add an IP restriction to a cloud_project_database resource will cause the cloud_project_database resource to be updated on every apply
+
         Apply IP restrictions to an OVHcloud Managed Database cluster.
 
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/kafka_acl.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/kafka_topic.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/m3_db_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/m3_db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/mongo_db_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/opensearch_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/opensearch_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __all__ = [
     'OpensearchUserAcl',
     'GetCapabilitiesEngineResult',
     'GetCapabilitiesFlavorResult',
     'GetCapabilitiesOptionResult',
     'GetCapabilitiesPlanResult',
     'GetDatabaseEndpointResult',
+    'GetDatabaseIpRestrictionResult',
     'GetDatabaseNodeResult',
 ]
 
 @pulumi.output_type
 class OpensearchUserAcl(dict):
     def __init__(__self__, *,
                  pattern: str,
@@ -324,14 +325,54 @@
         """
         URI of the endpoint.
         """
         return pulumi.get(self, "uri")
 
 
 @pulumi.output_type
+class GetDatabaseIpRestrictionResult(dict):
+    def __init__(__self__, *,
+                 description: str,
+                 ip: str,
+                 status: str):
+        """
+        :param str description: Description of the IP restriction
+        :param str ip: Authorized IP
+        :param str status: Current status of the cluster.
+        """
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "ip", ip)
+        pulumi.set(__self__, "status", status)
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        Description of the IP restriction
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter
+    def ip(self) -> str:
+        """
+        Authorized IP
+        """
+        return pulumi.get(self, "ip")
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        """
+        Current status of the cluster.
+        """
+        return pulumi.get(self, "status")
+
+
+@pulumi.output_type
 class GetDatabaseNodeResult(dict):
     def __init__(__self__, *,
                  network_id: str,
                  region: str,
                  subnet_id: str):
         """
         :param str network_id: Private network id in which the node should be deployed. It's the regional openstackId of the private network
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,13 +534,13 @@
         """
         Connection URI to the pool.
         """
         return pulumi.get(self, "uri")
 
     @property
     @pulumi.getter(name="userId")
-    def user_id(self) -> pulumi.Output[Optional[str]]:
+    def user_id(self) -> pulumi.Output[str]:
         """
         Database user authorized to connect to the pool, if none all the users are allowed.
         """
         return pulumi.get(self, "user_id")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/postgres_sql_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/redis_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/redis_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/cloudprojectdatabase/user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/cloudprojectdatabase/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/config/vars.py` & `pulumi_ovh-0.42.0/pulumi_ovh/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_cluster.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_clusters.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_clusters.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_input_engine.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_input_engine.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/get_logs_output_graylog_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         """
         return pulumi.get(self, "indexing_max_size")
 
     @property
     @pulumi.getter(name="indexingNotifyEnabled")
     def indexing_notify_enabled(self) -> bool:
         """
-        If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         """
         return pulumi.get(self, "indexing_notify_enabled")
 
     @property
     @pulumi.getter(name="isEditable")
     def is_editable(self) -> bool:
         """
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/logs_cluster.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/logs_input.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_input.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/logs_output_graylog_stream.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/logs_output_graylog_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         :param pulumi.Input[str] cold_storage_content: ColdStorage content
         :param pulumi.Input[bool] cold_storage_enabled: Is Cold storage enabled?
         :param pulumi.Input[bool] cold_storage_notify_enabled: Notify on new Cold storage archive
         :param pulumi.Input[int] cold_storage_retention: Cold storage retention in year
         :param pulumi.Input[str] cold_storage_target: ColdStorage destination
         :param pulumi.Input[bool] indexing_enabled: Enable ES indexing
         :param pulumi.Input[int] indexing_max_size: Maximum indexing size (in GB)
-        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         :param pulumi.Input[str] parent_stream_id: Parent stream ID
         :param pulumi.Input[bool] pause_indexing_on_max_size: If set, pause indexing when maximum size is reach
         :param pulumi.Input[str] retention_id: Retention ID
         :param pulumi.Input[bool] web_socket_enabled: Enable Websocket
         """
         pulumi.set(__self__, "description", description)
         pulumi.set(__self__, "service_name", service_name)
@@ -211,15 +211,15 @@
     def indexing_max_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "indexing_max_size", value)
 
     @property
     @pulumi.getter(name="indexingNotifyEnabled")
     def indexing_notify_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         """
         return pulumi.get(self, "indexing_notify_enabled")
 
     @indexing_notify_enabled.setter
     def indexing_notify_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "indexing_notify_enabled", value)
 
@@ -308,15 +308,15 @@
         :param pulumi.Input[bool] cold_storage_notify_enabled: Notify on new Cold storage archive
         :param pulumi.Input[int] cold_storage_retention: Cold storage retention in year
         :param pulumi.Input[str] cold_storage_target: ColdStorage destination
         :param pulumi.Input[str] created_at: Stream creation
         :param pulumi.Input[str] description: Stream description
         :param pulumi.Input[bool] indexing_enabled: Enable ES indexing
         :param pulumi.Input[int] indexing_max_size: Maximum indexing size (in GB)
-        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         :param pulumi.Input[bool] is_editable: Indicates if you are allowed to edit entry
         :param pulumi.Input[bool] is_shareable: Indicates if you are allowed to share entry
         :param pulumi.Input[int] nb_alert_condition: Number of alert condition
         :param pulumi.Input[int] nb_archive: Number of coldstored archives
         :param pulumi.Input[str] parent_stream_id: Parent stream ID
         :param pulumi.Input[bool] pause_indexing_on_max_size: If set, pause indexing when maximum size is reach
         :param pulumi.Input[str] retention_id: Retention ID
@@ -507,15 +507,15 @@
     def indexing_max_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "indexing_max_size", value)
 
     @property
     @pulumi.getter(name="indexingNotifyEnabled")
     def indexing_notify_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
-        If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         """
         return pulumi.get(self, "indexing_notify_enabled")
 
     @indexing_notify_enabled.setter
     def indexing_notify_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "indexing_notify_enabled", value)
 
@@ -695,15 +695,15 @@
         :param pulumi.Input[bool] cold_storage_enabled: Is Cold storage enabled?
         :param pulumi.Input[bool] cold_storage_notify_enabled: Notify on new Cold storage archive
         :param pulumi.Input[int] cold_storage_retention: Cold storage retention in year
         :param pulumi.Input[str] cold_storage_target: ColdStorage destination
         :param pulumi.Input[str] description: Stream description
         :param pulumi.Input[bool] indexing_enabled: Enable ES indexing
         :param pulumi.Input[int] indexing_max_size: Maximum indexing size (in GB)
-        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         :param pulumi.Input[str] parent_stream_id: Parent stream ID
         :param pulumi.Input[bool] pause_indexing_on_max_size: If set, pause indexing when maximum size is reach
         :param pulumi.Input[str] retention_id: Retention ID
         :param pulumi.Input[str] service_name: The service name
         :param pulumi.Input[str] title: Stream description
         :param pulumi.Input[bool] web_socket_enabled: Enable Websocket
         """
@@ -833,15 +833,15 @@
         :param pulumi.Input[bool] cold_storage_notify_enabled: Notify on new Cold storage archive
         :param pulumi.Input[int] cold_storage_retention: Cold storage retention in year
         :param pulumi.Input[str] cold_storage_target: ColdStorage destination
         :param pulumi.Input[str] created_at: Stream creation
         :param pulumi.Input[str] description: Stream description
         :param pulumi.Input[bool] indexing_enabled: Enable ES indexing
         :param pulumi.Input[int] indexing_max_size: Maximum indexing size (in GB)
-        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        :param pulumi.Input[bool] indexing_notify_enabled: If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         :param pulumi.Input[bool] is_editable: Indicates if you are allowed to edit entry
         :param pulumi.Input[bool] is_shareable: Indicates if you are allowed to share entry
         :param pulumi.Input[int] nb_alert_condition: Number of alert condition
         :param pulumi.Input[int] nb_archive: Number of coldstored archives
         :param pulumi.Input[str] parent_stream_id: Parent stream ID
         :param pulumi.Input[bool] pause_indexing_on_max_size: If set, pause indexing when maximum size is reach
         :param pulumi.Input[str] retention_id: Retention ID
@@ -969,15 +969,15 @@
         """
         return pulumi.get(self, "indexing_max_size")
 
     @property
     @pulumi.getter(name="indexingNotifyEnabled")
     def indexing_notify_enabled(self) -> pulumi.Output[bool]:
         """
-        If set, notify when size is near 80, 90 or 100 %!o(MISSING)f the maximum configured setting
+        If set, notify when size is near 80, 90 or 100 % of the maximum configured setting
         """
         return pulumi.get(self, "indexing_notify_enabled")
 
     @property
     @pulumi.getter(name="isEditable")
     def is_editable(self) -> pulumi.Output[bool]:
         """
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dbaas/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dbaas/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,92 +13,58 @@
     'ServerInstallTaskDetailsArgs',
     'ServerNetworkingInterfaceArgs',
 ]
 
 @pulumi.input_type
 class ServerInstallTaskDetailsArgs:
     def __init__(__self__, *,
-                 change_log: Optional[pulumi.Input[str]] = None,
                  custom_hostname: Optional[pulumi.Input[str]] = None,
                  disk_group_id: Optional[pulumi.Input[int]] = None,
-                 install_rtm: Optional[pulumi.Input[bool]] = None,
                  install_sql_server: Optional[pulumi.Input[bool]] = None,
                  language: Optional[pulumi.Input[str]] = None,
                  no_raid: Optional[pulumi.Input[bool]] = None,
                  post_installation_script_link: Optional[pulumi.Input[str]] = None,
                  post_installation_script_return: Optional[pulumi.Input[str]] = None,
-                 reset_hw_raid: Optional[pulumi.Input[bool]] = None,
                  soft_raid_devices: Optional[pulumi.Input[int]] = None,
                  ssh_key_name: Optional[pulumi.Input[str]] = None,
-                 use_distrib_kernel: Optional[pulumi.Input[bool]] = None,
                  use_spla: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] change_log: Template change log details.
         :param pulumi.Input[str] custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param pulumi.Input[int] disk_group_id: Disk group id.
-        :param pulumi.Input[bool] install_rtm: set to true to install RTM.
         :param pulumi.Input[bool] install_sql_server: set to true to install sql server (Windows template only).
         :param pulumi.Input[str] language: language.
         :param pulumi.Input[bool] no_raid: set to true to disable RAID.
         :param pulumi.Input[str] post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param pulumi.Input[str] post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param pulumi.Input[bool] reset_hw_raid: set to true to make a hardware raid reset.
         :param pulumi.Input[int] soft_raid_devices: soft raid devices.
         :param pulumi.Input[str] ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param pulumi.Input[bool] use_distrib_kernel: Use the distribution's native kernel instead of the recommended OVHcloud Kernel.
         :param pulumi.Input[bool] use_spla: set to true to use SPLA.
         """
-        if change_log is not None:
-            warnings.warn("""field is not used anymore""", DeprecationWarning)
-            pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-        if change_log is not None:
-            pulumi.set(__self__, "change_log", change_log)
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if disk_group_id is not None:
             pulumi.set(__self__, "disk_group_id", disk_group_id)
-        if install_rtm is not None:
-            pulumi.set(__self__, "install_rtm", install_rtm)
         if install_sql_server is not None:
             pulumi.set(__self__, "install_sql_server", install_sql_server)
         if language is not None:
             pulumi.set(__self__, "language", language)
         if no_raid is not None:
             pulumi.set(__self__, "no_raid", no_raid)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if reset_hw_raid is not None:
-            pulumi.set(__self__, "reset_hw_raid", reset_hw_raid)
         if soft_raid_devices is not None:
             pulumi.set(__self__, "soft_raid_devices", soft_raid_devices)
         if ssh_key_name is not None:
             pulumi.set(__self__, "ssh_key_name", ssh_key_name)
-        if use_distrib_kernel is not None:
-            pulumi.set(__self__, "use_distrib_kernel", use_distrib_kernel)
         if use_spla is not None:
             pulumi.set(__self__, "use_spla", use_spla)
 
     @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> Optional[pulumi.Input[str]]:
-        """
-        Template change log details.
-        """
-        warnings.warn("""field is not used anymore""", DeprecationWarning)
-        pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-
-        return pulumi.get(self, "change_log")
-
-    @change_log.setter
-    def change_log(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "change_log", value)
-
-    @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[pulumi.Input[str]]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
         return pulumi.get(self, "custom_hostname")
 
@@ -115,26 +81,14 @@
         return pulumi.get(self, "disk_group_id")
 
     @disk_group_id.setter
     def disk_group_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_group_id", value)
 
     @property
-    @pulumi.getter(name="installRtm")
-    def install_rtm(self) -> Optional[pulumi.Input[bool]]:
-        """
-        set to true to install RTM.
-        """
-        return pulumi.get(self, "install_rtm")
-
-    @install_rtm.setter
-    def install_rtm(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "install_rtm", value)
-
-    @property
     @pulumi.getter(name="installSqlServer")
     def install_sql_server(self) -> Optional[pulumi.Input[bool]]:
         """
         set to true to install sql server (Windows template only).
         """
         return pulumi.get(self, "install_sql_server")
 
@@ -187,26 +141,14 @@
         return pulumi.get(self, "post_installation_script_return")
 
     @post_installation_script_return.setter
     def post_installation_script_return(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "post_installation_script_return", value)
 
     @property
-    @pulumi.getter(name="resetHwRaid")
-    def reset_hw_raid(self) -> Optional[pulumi.Input[bool]]:
-        """
-        set to true to make a hardware raid reset.
-        """
-        return pulumi.get(self, "reset_hw_raid")
-
-    @reset_hw_raid.setter
-    def reset_hw_raid(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "reset_hw_raid", value)
-
-    @property
     @pulumi.getter(name="softRaidDevices")
     def soft_raid_devices(self) -> Optional[pulumi.Input[int]]:
         """
         soft raid devices.
         """
         return pulumi.get(self, "soft_raid_devices")
 
@@ -223,26 +165,14 @@
         return pulumi.get(self, "ssh_key_name")
 
     @ssh_key_name.setter
     def ssh_key_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key_name", value)
 
     @property
-    @pulumi.getter(name="useDistribKernel")
-    def use_distrib_kernel(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Use the distribution's native kernel instead of the recommended OVHcloud Kernel.
-        """
-        return pulumi.get(self, "use_distrib_kernel")
-
-    @use_distrib_kernel.setter
-    def use_distrib_kernel(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "use_distrib_kernel", value)
-
-    @property
     @pulumi.getter(name="useSpla")
     def use_spla(self) -> Optional[pulumi.Input[bool]]:
         """
         set to true to use SPLA.
         """
         return pulumi.get(self, "use_spla")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/ceph_acl.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/ceph_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_ceph.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_ceph.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_nas_ha.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_nas_ha.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,16 +128,15 @@
         """
         return pulumi.get(self, "service_name")
 
     @property
     @pulumi.getter(name="zpoolCapacity")
     def zpool_capacity(self) -> float:
         """
-        percentage of HA-NAS space used in %!
-        (MISSING)
+        percentage of HA-NAS space used in %
         """
         return pulumi.get(self, "zpool_capacity")
 
     @property
     @pulumi.getter(name="zpoolSize")
     def zpool_size(self) -> float:
         """
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_server_boots.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_boots.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/get_server_specifications_hardware.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/get_server_specifications_hardware.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/nas_ha_partition.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,23 +104,21 @@
                  name: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  service_name: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  used_by_snapshots: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering NasHAPartition resources.
-        :param pulumi.Input[int] capacity: Percentage of partition space used in %!
-               (MISSING)
+        :param pulumi.Input[int] capacity: Percentage of partition space used in %
         :param pulumi.Input[str] description: A brief description of the partition
         :param pulumi.Input[str] name: name of the partition
         :param pulumi.Input[str] protocol: one of "NFS", "CIFS" or "NFS_CIFS"
         :param pulumi.Input[str] service_name: The internal name of your HA-NAS (it has to be ordered via OVHcloud interface)
         :param pulumi.Input[int] size: size of the partition in GB
-        :param pulumi.Input[int] used_by_snapshots: Percentage of partition space used by snapshots in %!
-               (MISSING)
+        :param pulumi.Input[int] used_by_snapshots: Percentage of partition space used by snapshots in %
         """
         if capacity is not None:
             pulumi.set(__self__, "capacity", capacity)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -133,16 +131,15 @@
         if used_by_snapshots is not None:
             pulumi.set(__self__, "used_by_snapshots", used_by_snapshots)
 
     @property
     @pulumi.getter
     def capacity(self) -> Optional[pulumi.Input[int]]:
         """
-        Percentage of partition space used in %!
-        (MISSING)
+        Percentage of partition space used in %
         """
         return pulumi.get(self, "capacity")
 
     @capacity.setter
     def capacity(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "capacity", value)
 
@@ -206,16 +203,15 @@
     def size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "size", value)
 
     @property
     @pulumi.getter(name="usedBySnapshots")
     def used_by_snapshots(self) -> Optional[pulumi.Input[int]]:
         """
-        Percentage of partition space used by snapshots in %!
-        (MISSING)
+        Percentage of partition space used by snapshots in %
         """
         return pulumi.get(self, "used_by_snapshots")
 
     @used_by_snapshots.setter
     def used_by_snapshots(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "used_by_snapshots", value)
 
@@ -357,23 +353,21 @@
         """
         Get an existing NasHAPartition resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[int] capacity: Percentage of partition space used in %!
-               (MISSING)
+        :param pulumi.Input[int] capacity: Percentage of partition space used in %
         :param pulumi.Input[str] description: A brief description of the partition
         :param pulumi.Input[str] name: name of the partition
         :param pulumi.Input[str] protocol: one of "NFS", "CIFS" or "NFS_CIFS"
         :param pulumi.Input[str] service_name: The internal name of your HA-NAS (it has to be ordered via OVHcloud interface)
         :param pulumi.Input[int] size: size of the partition in GB
-        :param pulumi.Input[int] used_by_snapshots: Percentage of partition space used by snapshots in %!
-               (MISSING)
+        :param pulumi.Input[int] used_by_snapshots: Percentage of partition space used by snapshots in %
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NasHAPartitionState.__new__(_NasHAPartitionState)
 
         __props__.__dict__["capacity"] = capacity
         __props__.__dict__["description"] = description
@@ -384,16 +378,15 @@
         __props__.__dict__["used_by_snapshots"] = used_by_snapshots
         return NasHAPartition(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def capacity(self) -> pulumi.Output[int]:
         """
-        Percentage of partition space used in %!
-        (MISSING)
+        Percentage of partition space used in %
         """
         return pulumi.get(self, "capacity")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
@@ -433,12 +426,11 @@
         """
         return pulumi.get(self, "size")
 
     @property
     @pulumi.getter(name="usedBySnapshots")
     def used_by_snapshots(self) -> pulumi.Output[int]:
         """
-        Percentage of partition space used by snapshots in %!
-        (MISSING)
+        Percentage of partition space used by snapshots in %
         """
         return pulumi.get(self, "used_by_snapshots")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/nas_ha_partition_access.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS partition access can be imported using the `{service_name}/{partition_name}/{ip}`, e.g.
 
         ```sh
-        $ pulumi import ovh:Dedicated/nasHAPartitionAccess:NasHAPartitionAccess my-partition zpool-12345/my-partition/123.123.123.123%!F(MISSING)32`
+        $ pulumi import ovh:Dedicated/nasHAPartitionAccess:NasHAPartitionAccess my-partition zpool-12345/my-partition/123.123.123.123%2F32`
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] ip: ip block in x.x.x.x/x format
         :param pulumi.Input[str] partition_name: name of the partition
         :param pulumi.Input[str] service_name: The internal name of your HA-NAS (it has to be ordered via OVHcloud interface)
@@ -220,15 +220,15 @@
         <!--End PulumiCodeChooser -->
 
         ## Import
 
         HA-NAS partition access can be imported using the `{service_name}/{partition_name}/{ip}`, e.g.
 
         ```sh
-        $ pulumi import ovh:Dedicated/nasHAPartitionAccess:NasHAPartitionAccess my-partition zpool-12345/my-partition/123.123.123.123%!F(MISSING)32`
+        $ pulumi import ovh:Dedicated/nasHAPartitionAccess:NasHAPartitionAccess my-partition zpool-12345/my-partition/123.123.123.123%2F32`
         ```
 
         :param str resource_name: The name of the resource.
         :param NasHAPartitionAccessArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/nas_ha_partition_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/outputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,38 +23,30 @@
 ]
 
 @pulumi.output_type
 class ServerInstallTaskDetails(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "changeLog":
-            suggest = "change_log"
-        elif key == "customHostname":
+        if key == "customHostname":
             suggest = "custom_hostname"
         elif key == "diskGroupId":
             suggest = "disk_group_id"
-        elif key == "installRtm":
-            suggest = "install_rtm"
         elif key == "installSqlServer":
             suggest = "install_sql_server"
         elif key == "noRaid":
             suggest = "no_raid"
         elif key == "postInstallationScriptLink":
             suggest = "post_installation_script_link"
         elif key == "postInstallationScriptReturn":
             suggest = "post_installation_script_return"
-        elif key == "resetHwRaid":
-            suggest = "reset_hw_raid"
         elif key == "softRaidDevices":
             suggest = "soft_raid_devices"
         elif key == "sshKeyName":
             suggest = "ssh_key_name"
-        elif key == "useDistribKernel":
-            suggest = "use_distrib_kernel"
         elif key == "useSpla":
             suggest = "use_spla"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ServerInstallTaskDetails. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -62,85 +54,58 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         ServerInstallTaskDetails.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 change_log: Optional[str] = None,
                  custom_hostname: Optional[str] = None,
                  disk_group_id: Optional[int] = None,
-                 install_rtm: Optional[bool] = None,
                  install_sql_server: Optional[bool] = None,
                  language: Optional[str] = None,
                  no_raid: Optional[bool] = None,
                  post_installation_script_link: Optional[str] = None,
                  post_installation_script_return: Optional[str] = None,
-                 reset_hw_raid: Optional[bool] = None,
                  soft_raid_devices: Optional[int] = None,
                  ssh_key_name: Optional[str] = None,
-                 use_distrib_kernel: Optional[bool] = None,
                  use_spla: Optional[bool] = None):
         """
-        :param str change_log: Template change log details.
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param int disk_group_id: Disk group id.
-        :param bool install_rtm: set to true to install RTM.
         :param bool install_sql_server: set to true to install sql server (Windows template only).
         :param str language: language.
         :param bool no_raid: set to true to disable RAID.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param str post_installation_script_return: Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
-        :param bool reset_hw_raid: set to true to make a hardware raid reset.
         :param int soft_raid_devices: soft raid devices.
         :param str ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param bool use_distrib_kernel: Use the distribution's native kernel instead of the recommended OVHcloud Kernel.
         :param bool use_spla: set to true to use SPLA.
         """
-        if change_log is not None:
-            pulumi.set(__self__, "change_log", change_log)
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if disk_group_id is not None:
             pulumi.set(__self__, "disk_group_id", disk_group_id)
-        if install_rtm is not None:
-            pulumi.set(__self__, "install_rtm", install_rtm)
         if install_sql_server is not None:
             pulumi.set(__self__, "install_sql_server", install_sql_server)
         if language is not None:
             pulumi.set(__self__, "language", language)
         if no_raid is not None:
             pulumi.set(__self__, "no_raid", no_raid)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
-        if reset_hw_raid is not None:
-            pulumi.set(__self__, "reset_hw_raid", reset_hw_raid)
         if soft_raid_devices is not None:
             pulumi.set(__self__, "soft_raid_devices", soft_raid_devices)
         if ssh_key_name is not None:
             pulumi.set(__self__, "ssh_key_name", ssh_key_name)
-        if use_distrib_kernel is not None:
-            pulumi.set(__self__, "use_distrib_kernel", use_distrib_kernel)
         if use_spla is not None:
             pulumi.set(__self__, "use_spla", use_spla)
 
     @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> Optional[str]:
-        """
-        Template change log details.
-        """
-        warnings.warn("""field is not used anymore""", DeprecationWarning)
-        pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-
-        return pulumi.get(self, "change_log")
-
-    @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[str]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
         return pulumi.get(self, "custom_hostname")
 
@@ -149,22 +114,14 @@
     def disk_group_id(self) -> Optional[int]:
         """
         Disk group id.
         """
         return pulumi.get(self, "disk_group_id")
 
     @property
-    @pulumi.getter(name="installRtm")
-    def install_rtm(self) -> Optional[bool]:
-        """
-        set to true to install RTM.
-        """
-        return pulumi.get(self, "install_rtm")
-
-    @property
     @pulumi.getter(name="installSqlServer")
     def install_sql_server(self) -> Optional[bool]:
         """
         set to true to install sql server (Windows template only).
         """
         return pulumi.get(self, "install_sql_server")
 
@@ -197,22 +154,14 @@
     def post_installation_script_return(self) -> Optional[str]:
         """
         Indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         """
         return pulumi.get(self, "post_installation_script_return")
 
     @property
-    @pulumi.getter(name="resetHwRaid")
-    def reset_hw_raid(self) -> Optional[bool]:
-        """
-        set to true to make a hardware raid reset.
-        """
-        return pulumi.get(self, "reset_hw_raid")
-
-    @property
     @pulumi.getter(name="softRaidDevices")
     def soft_raid_devices(self) -> Optional[int]:
         """
         soft raid devices.
         """
         return pulumi.get(self, "soft_raid_devices")
 
@@ -221,22 +170,14 @@
     def ssh_key_name(self) -> Optional[str]:
         """
         Name of the ssh key that should be installed. Password login will be disabled.
         """
         return pulumi.get(self, "ssh_key_name")
 
     @property
-    @pulumi.getter(name="useDistribKernel")
-    def use_distrib_kernel(self) -> Optional[bool]:
-        """
-        Use the distribution's native kernel instead of the recommended OVHcloud Kernel.
-        """
-        return pulumi.get(self, "use_distrib_kernel")
-
-    @property
     @pulumi.getter(name="useSpla")
     def use_spla(self) -> Optional[bool]:
         """
         set to true to use SPLA.
         """
         return pulumi.get(self, "use_spla")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_install_task.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_install_task.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_networking.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_networking.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_reboot_task.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_reboot_task.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/dedicated/server_update.py` & `pulumi_ovh-0.42.0/pulumi_ovh/dedicated/server_update.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/domain/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/domain/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/domain/get_zone.py` & `pulumi_ovh-0.42.0/pulumi_ovh/domain/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/domain/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/domain/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/domain/zone.py` & `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/domain/zone_record.py` & `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,15 @@
             ttl=3600,
             zone="testdemo.ovh")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        OVHcloud domain zone record can be imported using the `id`, which can be retrieved by using [OVH API portal](<https://api.ovh.com/console/#/domain/zone/%!B(MISSING)zoneName%!D(MISSING)/record~GET>), and the `zone`, separated by "." E.g.,
+        OVHcloud domain zone record can be imported using the `id`, which can be retrieved by using [OVH API portal](https://api.ovh.com/console/#/domain/zone/%7BzoneName%7D/record~GET), and the `zone`, separated by "." E.g.,
 
         bash
 
         ```sh
         $ pulumi import ovh:Domain/zoneRecord:ZoneRecord test id.zone
         ```
 
@@ -253,15 +253,15 @@
             ttl=3600,
             zone="testdemo.ovh")
         ```
         <!--End PulumiCodeChooser -->
 
         ## Import
 
-        OVHcloud domain zone record can be imported using the `id`, which can be retrieved by using [OVH API portal](<https://api.ovh.com/console/#/domain/zone/%!B(MISSING)zoneName%!D(MISSING)/record~GET>), and the `zone`, separated by "." E.g.,
+        OVHcloud domain zone record can be imported using the `id`, which can be retrieved by using [OVH API portal](https://api.ovh.com/console/#/domain/zone/%7BzoneName%7D/record~GET), and the `zone`, separated by "." E.g.,
 
         bash
 
         ```sh
         $ pulumi import ovh:Domain/zoneRecord:ZoneRecord test id.zone
         ```
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/domain/zone_redirection.py` & `pulumi_ovh-0.42.0/pulumi_ovh/domain/zone_redirection.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/get_installation_templates.py` & `pulumi_ovh-0.42.0/pulumi_ovh/get_installation_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/get_server.py` & `pulumi_ovh-0.42.0/pulumi_ovh/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/get_servers.py` & `pulumi_ovh-0.42.0/pulumi_ovh/get_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/get_vrack_networks.py` & `pulumi_ovh-0.42.0/pulumi_ovh/get_vrack_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_allowlist.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_db.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/get_private_database_user_grant.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/get_private_database_user_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_allowlist.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_allowlist.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_db.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_db.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/hosting/private_database_user_grant.py` & `pulumi_ovh-0.42.0/pulumi_ovh/hosting/private_database_user_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_permissions_group.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_permissions_groups.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_permissions_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_policies.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_policy.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_reference_actions.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_reference_resource_type.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_reference_resource_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_resource_group.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/get_resource_groups.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/get_resource_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/permissions_group.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/permissions_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/policy.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iam/resource_group.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iam/resource_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/ip/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/ip/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/ip/get_service.py` & `pulumi_ovh-0.42.0/pulumi_ovh/ip/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/ip/ip_service.py` & `pulumi_ovh-0.42.0/pulumi_ovh/ip/ip_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/ip/move.py` & `pulumi_ovh-0.42.0/pulumi_ovh/ip/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     def __init__(__self__, *,
                  ip: pulumi.Input[str],
                  routed_to: pulumi.Input['MoveRoutedToArgs'],
                  description: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Move resource.
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
-        :param pulumi.Input['MoveRoutedToArgs'] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-               instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        :param pulumi.Input['MoveRoutedToArgs'] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+               instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         :param pulumi.Input[str] description: Description attached to the IP
         """
         pulumi.set(__self__, "ip", ip)
         pulumi.set(__self__, "routed_to", routed_to)
         if description is not None:
             pulumi.set(__self__, "description", description)
 
@@ -43,16 +43,16 @@
     def ip(self, value: pulumi.Input[str]):
         pulumi.set(self, "ip", value)
 
     @property
     @pulumi.getter(name="routedTo")
     def routed_to(self) -> pulumi.Input['MoveRoutedToArgs']:
         """
-        Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-        instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+        instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         """
         return pulumi.get(self, "routed_to")
 
     @routed_to.setter
     def routed_to(self, value: pulumi.Input['MoveRoutedToArgs']):
         pulumi.set(self, "routed_to", value)
 
@@ -85,16 +85,16 @@
         """
         Input properties used for looking up and filtering Move resources.
         :param pulumi.Input[bool] can_be_terminated: Whether IP service can be terminated
         :param pulumi.Input[str] country: Country
         :param pulumi.Input[str] description: Description attached to the IP
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
         :param pulumi.Input[str] organisation_id: IP block organisation Id
-        :param pulumi.Input['MoveRoutedToArgs'] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-               instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        :param pulumi.Input['MoveRoutedToArgs'] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+               instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         :param pulumi.Input[str] service_name: Name of the service to route the IP to. IP will be parked if this value is an empty string
         :param pulumi.Input[str] task_start_date: Starting date and time field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] task_status: Status field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] type: Possible values for ip type
         """
         if can_be_terminated is not None:
             pulumi.set(__self__, "can_be_terminated", can_be_terminated)
@@ -177,16 +177,16 @@
     def organisation_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "organisation_id", value)
 
     @property
     @pulumi.getter(name="routedTo")
     def routed_to(self) -> Optional[pulumi.Input['MoveRoutedToArgs']]:
         """
-        Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-        instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+        instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         """
         return pulumi.get(self, "routed_to")
 
     @routed_to.setter
     def routed_to(self, value: Optional[pulumi.Input['MoveRoutedToArgs']]):
         pulumi.set(self, "routed_to", value)
 
@@ -281,16 +281,16 @@
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description attached to the IP
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
-        :param pulumi.Input[pulumi.InputType['MoveRoutedToArgs']] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-               instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        :param pulumi.Input[pulumi.InputType['MoveRoutedToArgs']] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+               instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: MoveArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -396,16 +396,16 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] can_be_terminated: Whether IP service can be terminated
         :param pulumi.Input[str] country: Country
         :param pulumi.Input[str] description: Description attached to the IP
         :param pulumi.Input[str] ip: IP block that we want to attach to a different service
         :param pulumi.Input[str] organisation_id: IP block organisation Id
-        :param pulumi.Input[pulumi.InputType['MoveRoutedToArgs']] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-               instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        :param pulumi.Input[pulumi.InputType['MoveRoutedToArgs']] routed_to: Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+               instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         :param pulumi.Input[str] service_name: Name of the service to route the IP to. IP will be parked if this value is an empty string
         :param pulumi.Input[str] task_start_date: Starting date and time field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] task_status: Status field of the current IP task that is in charge of changing the service the IP is attached to
         :param pulumi.Input[str] type: Possible values for ip type
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -463,16 +463,16 @@
         """
         return pulumi.get(self, "organisation_id")
 
     @property
     @pulumi.getter(name="routedTo")
     def routed_to(self) -> pulumi.Output['outputs.MoveRoutedTo']:
         """
-        Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/park~POST)
-        instead of [moved](https://api.ovh.com/console/#/ip/%!B(MISSING)ip%!D(MISSING)/move~POST)
+        Service to route the IP to. If null, the IP will be [parked](https://api.ovh.com/console/#/ip/%7Bip%7D/park~POST)
+        instead of [moved](https://api.ovh.com/console/#/ip/%7Bip%7D/move~POST)
         """
         return pulumi.get(self, "routed_to")
 
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/ip/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/ip/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/ip/reverse.py` & `pulumi_ovh-0.42.0/pulumi_ovh/ip/reverse.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 from .load_balancer import *
 from .refresh import *
 from .tcp_farm import *
 from .tcp_farm_server import *
 from .tcp_frontend import *
 from .tcp_route import *
 from .tcp_route_rule import *
+from .udp_frontend import *
 from .vrack_network import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_ip_load_balancing.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/get_vrack_network.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/get_vrack_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_farm.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_farm_server.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_farm_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_frontend.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_frontend.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_route.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/http_route_rule.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/http_route_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/load_balancer.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/refresh.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/refresh.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_farm.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_farm_server.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_farm_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_frontend.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_frontend.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_route.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/tcp_route_rule.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/tcp_route_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/iploadbalancing/vrack_network.py` & `pulumi_ovh-0.42.0/pulumi_ovh/iploadbalancing/vrack_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/_inputs.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,65 +12,39 @@
 __all__ = [
     'InstallationTemplateCustomizationArgs',
 ]
 
 @pulumi.input_type
 class InstallationTemplateCustomizationArgs:
     def __init__(__self__, *,
-                 change_log: Optional[pulumi.Input[str]] = None,
                  custom_hostname: Optional[pulumi.Input[str]] = None,
                  post_installation_script_link: Optional[pulumi.Input[str]] = None,
                  post_installation_script_return: Optional[pulumi.Input[str]] = None,
                  rating: Optional[pulumi.Input[int]] = None,
-                 ssh_key_name: Optional[pulumi.Input[str]] = None,
-                 use_distribution_kernel: Optional[pulumi.Input[bool]] = None):
+                 ssh_key_name: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] change_log: Template change log details.
         :param pulumi.Input[str] custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param pulumi.Input[str] post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param pulumi.Input[str] post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         :param pulumi.Input[int] rating: Rating.
         :param pulumi.Input[str] ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param pulumi.Input[bool] use_distribution_kernel: Use the distribution's native kernel instead of the recommended OV
         """
-        if change_log is not None:
-            warnings.warn("""field is not used anymore""", DeprecationWarning)
-            pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-        if change_log is not None:
-            pulumi.set(__self__, "change_log", change_log)
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
         if rating is not None:
             warnings.warn("""field is not used anymore""", DeprecationWarning)
             pulumi.log.warn("""rating is deprecated: field is not used anymore""")
         if rating is not None:
             pulumi.set(__self__, "rating", rating)
         if ssh_key_name is not None:
             pulumi.set(__self__, "ssh_key_name", ssh_key_name)
-        if use_distribution_kernel is not None:
-            pulumi.set(__self__, "use_distribution_kernel", use_distribution_kernel)
-
-    @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> Optional[pulumi.Input[str]]:
-        """
-        Template change log details.
-        """
-        warnings.warn("""field is not used anymore""", DeprecationWarning)
-        pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-
-        return pulumi.get(self, "change_log")
-
-    @change_log.setter
-    def change_log(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "change_log", value)
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[pulumi.Input[str]]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -127,20 +101,8 @@
         """
         return pulumi.get(self, "ssh_key_name")
 
     @ssh_key_name.setter
     def ssh_key_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key_name", value)
 
-    @property
-    @pulumi.getter(name="useDistributionKernel")
-    def use_distribution_kernel(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Use the distribution's native kernel instead of the recommended OV
-        """
-        return pulumi.get(self, "use_distribution_kernel")
-
-    @use_distribution_kernel.setter
-    def use_distribution_kernel(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "use_distribution_kernel", value)
-
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/apio_auth2_client.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/apio_auth2_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_apio_auth2_client.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_apio_auth2_clients.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_apio_auth2_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_group.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_groups.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_identity_users.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_identity_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_installation_template.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 
 @pulumi.output_type
 class GetInstallationTemplateResult:
     """
     A collection of values returned by getInstallationTemplate.
     """
-    def __init__(__self__, available_languages=None, beta=None, bit_format=None, category=None, customizations=None, default_language=None, deprecated=None, description=None, distribution=None, family=None, filesystems=None, hard_raid_configuration=None, id=None, last_modification=None, lvm_ready=None, partition_schemes=None, supports_distribution_kernel=None, supports_rtm=None, supports_sql_server=None, template_name=None):
+    def __init__(__self__, available_languages=None, beta=None, bit_format=None, category=None, customizations=None, default_language=None, deprecated=None, description=None, distribution=None, family=None, filesystems=None, hard_raid_configuration=None, id=None, last_modification=None, lvm_ready=None, partition_schemes=None, supports_sql_server=None, template_name=None):
         if available_languages and not isinstance(available_languages, list):
             raise TypeError("Expected argument 'available_languages' to be a list")
         pulumi.set(__self__, "available_languages", available_languages)
         if beta and not isinstance(beta, bool):
             raise TypeError("Expected argument 'beta' to be a bool")
         pulumi.set(__self__, "beta", beta)
         if bit_format and not isinstance(bit_format, int):
@@ -67,20 +67,14 @@
         pulumi.set(__self__, "last_modification", last_modification)
         if lvm_ready and not isinstance(lvm_ready, bool):
             raise TypeError("Expected argument 'lvm_ready' to be a bool")
         pulumi.set(__self__, "lvm_ready", lvm_ready)
         if partition_schemes and not isinstance(partition_schemes, list):
             raise TypeError("Expected argument 'partition_schemes' to be a list")
         pulumi.set(__self__, "partition_schemes", partition_schemes)
-        if supports_distribution_kernel and not isinstance(supports_distribution_kernel, bool):
-            raise TypeError("Expected argument 'supports_distribution_kernel' to be a bool")
-        pulumi.set(__self__, "supports_distribution_kernel", supports_distribution_kernel)
-        if supports_rtm and not isinstance(supports_rtm, bool):
-            raise TypeError("Expected argument 'supports_rtm' to be a bool")
-        pulumi.set(__self__, "supports_rtm", supports_rtm)
         if supports_sql_server and not isinstance(supports_sql_server, bool):
             raise TypeError("Expected argument 'supports_sql_server' to be a bool")
         pulumi.set(__self__, "supports_sql_server", supports_sql_server)
         if template_name and not isinstance(template_name, str):
             raise TypeError("Expected argument 'template_name' to be a str")
         pulumi.set(__self__, "template_name", template_name)
 
@@ -200,30 +194,14 @@
 
     @property
     @pulumi.getter(name="partitionSchemes")
     def partition_schemes(self) -> Sequence['outputs.GetInstallationTemplatePartitionSchemeResult']:
         return pulumi.get(self, "partition_schemes")
 
     @property
-    @pulumi.getter(name="supportsDistributionKernel")
-    def supports_distribution_kernel(self) -> bool:
-        """
-        This distribution supports installation using the distribution's native kernel instead of the recommended OVHcloud kernel.
-        """
-        return pulumi.get(self, "supports_distribution_kernel")
-
-    @property
-    @pulumi.getter(name="supportsRtm")
-    def supports_rtm(self) -> bool:
-        """
-        This distribution supports RTM software.
-        """
-        return pulumi.get(self, "supports_rtm")
-
-    @property
     @pulumi.getter(name="supportsSqlServer")
     def supports_sql_server(self) -> bool:
         """
         This distribution supports the microsoft SQL server.
         """
         return pulumi.get(self, "supports_sql_server")
 
@@ -251,16 +229,14 @@
             family=self.family,
             filesystems=self.filesystems,
             hard_raid_configuration=self.hard_raid_configuration,
             id=self.id,
             last_modification=self.last_modification,
             lvm_ready=self.lvm_ready,
             partition_schemes=self.partition_schemes,
-            supports_distribution_kernel=self.supports_distribution_kernel,
-            supports_rtm=self.supports_rtm,
             supports_sql_server=self.supports_sql_server,
             template_name=self.template_name)
 
 
 def get_installation_template(template_name: Optional[str] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInstallationTemplateResult:
     """
@@ -298,16 +274,14 @@
         family=pulumi.get(__ret__, 'family'),
         filesystems=pulumi.get(__ret__, 'filesystems'),
         hard_raid_configuration=pulumi.get(__ret__, 'hard_raid_configuration'),
         id=pulumi.get(__ret__, 'id'),
         last_modification=pulumi.get(__ret__, 'last_modification'),
         lvm_ready=pulumi.get(__ret__, 'lvm_ready'),
         partition_schemes=pulumi.get(__ret__, 'partition_schemes'),
-        supports_distribution_kernel=pulumi.get(__ret__, 'supports_distribution_kernel'),
-        supports_rtm=pulumi.get(__ret__, 'supports_rtm'),
         supports_sql_server=pulumi.get(__ret__, 'supports_sql_server'),
         template_name=pulumi.get(__ret__, 'template_name'))
 
 
 @_utilities.lift_output_func(get_installation_template)
 def get_installation_template_output(template_name: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstallationTemplateResult]:
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_installation_templates.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_installation_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_me.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_me.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_paymentmean_bank_account.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_bank_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_paymentmean_credit_card.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_paymentmean_credit_card.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_ssh_key.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/get_ssh_keys.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/identity_group.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/identity_user.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/identity_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -109,16 +109,14 @@
                  distribution: Optional[pulumi.Input[str]] = None,
                  family: Optional[pulumi.Input[str]] = None,
                  filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
                  last_modification: Optional[pulumi.Input[str]] = None,
                  lvm_ready: Optional[pulumi.Input[bool]] = None,
                  remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
-                 supports_distribution_kernel: Optional[pulumi.Input[bool]] = None,
-                 supports_rtm: Optional[pulumi.Input[bool]] = None,
                  supports_sql_server: Optional[pulumi.Input[bool]] = None,
                  template_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering InstallationTemplate resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] available_languages: List of all language available for this template.
         :param pulumi.Input[str] base_template_name: The name of an existing installation template, choose one among the list given by `get_installation_templates` datasource.
         :param pulumi.Input[bool] beta: This distribution is new and, although tested and functional, may still display odd behaviour.
@@ -130,16 +128,14 @@
         :param pulumi.Input[str] distribution: the distribution this template is based on.
         :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
         :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
         :param pulumi.Input[str] last_modification: Date of last modification of the base image.
         :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
         :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
-        :param pulumi.Input[bool] supports_distribution_kernel: This distribution supports installation using the distribution's native kernel instead of the recommended OVHcloud kernel.
-        :param pulumi.Input[bool] supports_rtm: This distribution supports RTM software.
         :param pulumi.Input[bool] supports_sql_server: This distribution supports the microsoft SQL server.
         :param pulumi.Input[str] template_name: This template name.
         """
         if available_languages is not None:
             pulumi.set(__self__, "available_languages", available_languages)
         if base_template_name is not None:
             pulumi.set(__self__, "base_template_name", base_template_name)
@@ -167,18 +163,14 @@
             pulumi.set(__self__, "hard_raid_configuration", hard_raid_configuration)
         if last_modification is not None:
             pulumi.set(__self__, "last_modification", last_modification)
         if lvm_ready is not None:
             pulumi.set(__self__, "lvm_ready", lvm_ready)
         if remove_default_partition_schemes is not None:
             pulumi.set(__self__, "remove_default_partition_schemes", remove_default_partition_schemes)
-        if supports_distribution_kernel is not None:
-            pulumi.set(__self__, "supports_distribution_kernel", supports_distribution_kernel)
-        if supports_rtm is not None:
-            pulumi.set(__self__, "supports_rtm", supports_rtm)
         if supports_sql_server is not None:
             pulumi.set(__self__, "supports_sql_server", supports_sql_server)
         if template_name is not None:
             pulumi.set(__self__, "template_name", template_name)
 
     @property
     @pulumi.getter(name="availableLanguages")
@@ -366,38 +358,14 @@
         return pulumi.get(self, "remove_default_partition_schemes")
 
     @remove_default_partition_schemes.setter
     def remove_default_partition_schemes(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "remove_default_partition_schemes", value)
 
     @property
-    @pulumi.getter(name="supportsDistributionKernel")
-    def supports_distribution_kernel(self) -> Optional[pulumi.Input[bool]]:
-        """
-        This distribution supports installation using the distribution's native kernel instead of the recommended OVHcloud kernel.
-        """
-        return pulumi.get(self, "supports_distribution_kernel")
-
-    @supports_distribution_kernel.setter
-    def supports_distribution_kernel(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "supports_distribution_kernel", value)
-
-    @property
-    @pulumi.getter(name="supportsRtm")
-    def supports_rtm(self) -> Optional[pulumi.Input[bool]]:
-        """
-        This distribution supports RTM software.
-        """
-        return pulumi.get(self, "supports_rtm")
-
-    @supports_rtm.setter
-    def supports_rtm(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "supports_rtm", value)
-
-    @property
     @pulumi.getter(name="supportsSqlServer")
     def supports_sql_server(self) -> Optional[pulumi.Input[bool]]:
         """
         This distribution supports the microsoft SQL server.
         """
         return pulumi.get(self, "supports_sql_server")
 
@@ -544,16 +512,14 @@
             __props__.__dict__["description"] = None
             __props__.__dict__["distribution"] = None
             __props__.__dict__["family"] = None
             __props__.__dict__["filesystems"] = None
             __props__.__dict__["hard_raid_configuration"] = None
             __props__.__dict__["last_modification"] = None
             __props__.__dict__["lvm_ready"] = None
-            __props__.__dict__["supports_distribution_kernel"] = None
-            __props__.__dict__["supports_rtm"] = None
             __props__.__dict__["supports_sql_server"] = None
         super(InstallationTemplate, __self__).__init__(
             'ovh:Me/installationTemplate:InstallationTemplate',
             resource_name,
             __props__,
             opts)
 
@@ -573,16 +539,14 @@
             distribution: Optional[pulumi.Input[str]] = None,
             family: Optional[pulumi.Input[str]] = None,
             filesystems: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             hard_raid_configuration: Optional[pulumi.Input[bool]] = None,
             last_modification: Optional[pulumi.Input[str]] = None,
             lvm_ready: Optional[pulumi.Input[bool]] = None,
             remove_default_partition_schemes: Optional[pulumi.Input[bool]] = None,
-            supports_distribution_kernel: Optional[pulumi.Input[bool]] = None,
-            supports_rtm: Optional[pulumi.Input[bool]] = None,
             supports_sql_server: Optional[pulumi.Input[bool]] = None,
             template_name: Optional[pulumi.Input[str]] = None) -> 'InstallationTemplate':
         """
         Get an existing InstallationTemplate resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
@@ -599,16 +563,14 @@
         :param pulumi.Input[str] distribution: the distribution this template is based on.
         :param pulumi.Input[str] family: this template family type (bsd,linux,solaris,windows).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] filesystems: Filesystems available (btrfs,ext3,ext4,ntfs,reiserfs,swap,ufs,xfs,zfs).
         :param pulumi.Input[bool] hard_raid_configuration: This distribution supports hardware raid configuration through the OVHcloud API.
         :param pulumi.Input[str] last_modification: Date of last modification of the base image.
         :param pulumi.Input[bool] lvm_ready: This distribution supports Logical Volumes (Linux LVM)
         :param pulumi.Input[bool] remove_default_partition_schemes: Remove default partition schemes at creation.
-        :param pulumi.Input[bool] supports_distribution_kernel: This distribution supports installation using the distribution's native kernel instead of the recommended OVHcloud kernel.
-        :param pulumi.Input[bool] supports_rtm: This distribution supports RTM software.
         :param pulumi.Input[bool] supports_sql_server: This distribution supports the microsoft SQL server.
         :param pulumi.Input[str] template_name: This template name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstallationTemplateState.__new__(_InstallationTemplateState)
 
@@ -624,16 +586,14 @@
         __props__.__dict__["distribution"] = distribution
         __props__.__dict__["family"] = family
         __props__.__dict__["filesystems"] = filesystems
         __props__.__dict__["hard_raid_configuration"] = hard_raid_configuration
         __props__.__dict__["last_modification"] = last_modification
         __props__.__dict__["lvm_ready"] = lvm_ready
         __props__.__dict__["remove_default_partition_schemes"] = remove_default_partition_schemes
-        __props__.__dict__["supports_distribution_kernel"] = supports_distribution_kernel
-        __props__.__dict__["supports_rtm"] = supports_rtm
         __props__.__dict__["supports_sql_server"] = supports_sql_server
         __props__.__dict__["template_name"] = template_name
         return InstallationTemplate(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="availableLanguages")
     def available_languages(self) -> pulumi.Output[Sequence[str]]:
@@ -756,30 +716,14 @@
     def remove_default_partition_schemes(self) -> pulumi.Output[bool]:
         """
         Remove default partition schemes at creation.
         """
         return pulumi.get(self, "remove_default_partition_schemes")
 
     @property
-    @pulumi.getter(name="supportsDistributionKernel")
-    def supports_distribution_kernel(self) -> pulumi.Output[bool]:
-        """
-        This distribution supports installation using the distribution's native kernel instead of the recommended OVHcloud kernel.
-        """
-        return pulumi.get(self, "supports_distribution_kernel")
-
-    @property
-    @pulumi.getter(name="supportsRtm")
-    def supports_rtm(self) -> pulumi.Output[bool]:
-        """
-        This distribution supports RTM software.
-        """
-        return pulumi.get(self, "supports_rtm")
-
-    @property
     @pulumi.getter(name="supportsSqlServer")
     def supports_sql_server(self) -> pulumi.Output[bool]:
         """
         This distribution supports the microsoft SQL server.
         """
         return pulumi.get(self, "supports_sql_server")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template_partition_scheme.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_hardware_raid.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/installation_template_partition_scheme_partition.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/installation_template_partition_scheme_partition.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/outputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,80 +20,57 @@
 ]
 
 @pulumi.output_type
 class InstallationTemplateCustomization(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "changeLog":
-            suggest = "change_log"
-        elif key == "customHostname":
+        if key == "customHostname":
             suggest = "custom_hostname"
         elif key == "postInstallationScriptLink":
             suggest = "post_installation_script_link"
         elif key == "postInstallationScriptReturn":
             suggest = "post_installation_script_return"
         elif key == "sshKeyName":
             suggest = "ssh_key_name"
-        elif key == "useDistributionKernel":
-            suggest = "use_distribution_kernel"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InstallationTemplateCustomization. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         InstallationTemplateCustomization.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         InstallationTemplateCustomization.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 change_log: Optional[str] = None,
                  custom_hostname: Optional[str] = None,
                  post_installation_script_link: Optional[str] = None,
                  post_installation_script_return: Optional[str] = None,
                  rating: Optional[int] = None,
-                 ssh_key_name: Optional[str] = None,
-                 use_distribution_kernel: Optional[bool] = None):
+                 ssh_key_name: Optional[str] = None):
         """
-        :param str change_log: Template change log details.
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param str post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         :param int rating: Rating.
         :param str ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param bool use_distribution_kernel: Use the distribution's native kernel instead of the recommended OV
         """
-        if change_log is not None:
-            pulumi.set(__self__, "change_log", change_log)
         if custom_hostname is not None:
             pulumi.set(__self__, "custom_hostname", custom_hostname)
         if post_installation_script_link is not None:
             pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         if post_installation_script_return is not None:
             pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
         if rating is not None:
             pulumi.set(__self__, "rating", rating)
         if ssh_key_name is not None:
             pulumi.set(__self__, "ssh_key_name", ssh_key_name)
-        if use_distribution_kernel is not None:
-            pulumi.set(__self__, "use_distribution_kernel", use_distribution_kernel)
-
-    @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> Optional[str]:
-        """
-        Template change log details.
-        """
-        warnings.warn("""field is not used anymore""", DeprecationWarning)
-        pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-
-        return pulumi.get(self, "change_log")
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> Optional[str]:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -130,60 +107,35 @@
     @pulumi.getter(name="sshKeyName")
     def ssh_key_name(self) -> Optional[str]:
         """
         Name of the ssh key that should be installed. Password login will be disabled.
         """
         return pulumi.get(self, "ssh_key_name")
 
-    @property
-    @pulumi.getter(name="useDistributionKernel")
-    def use_distribution_kernel(self) -> Optional[bool]:
-        """
-        Use the distribution's native kernel instead of the recommended OV
-        """
-        return pulumi.get(self, "use_distribution_kernel")
-
 
 @pulumi.output_type
 class GetInstallationTemplateCustomizationResult(dict):
     def __init__(__self__, *,
-                 change_log: str,
                  custom_hostname: str,
                  post_installation_script_link: str,
                  post_installation_script_return: str,
                  rating: int,
-                 ssh_key_name: str,
-                 use_distribution_kernel: bool):
+                 ssh_key_name: str):
         """
-        :param str change_log: (DEPRECATED) Template change log details.
         :param str custom_hostname: Set up the server using the provided hostname instead of the default hostname.
         :param str post_installation_script_link: Indicate the URL where your postinstall customisation script is located.
         :param str post_installation_script_return: indicate the string returned by your postinstall customisation script on successful execution. Advice: your script should return a unique validation string in case of succes. A good example is 'loh1Xee7eo OK OK OK UGh8Ang1Gu'.
         :param int rating: (DEPRECATED) Rating.
         :param str ssh_key_name: Name of the ssh key that should be installed. Password login will be disabled.
-        :param bool use_distribution_kernel: Use the distribution's native kernel instead of the recommended OVHcloud Kernel.
         """
-        pulumi.set(__self__, "change_log", change_log)
         pulumi.set(__self__, "custom_hostname", custom_hostname)
         pulumi.set(__self__, "post_installation_script_link", post_installation_script_link)
         pulumi.set(__self__, "post_installation_script_return", post_installation_script_return)
         pulumi.set(__self__, "rating", rating)
         pulumi.set(__self__, "ssh_key_name", ssh_key_name)
-        pulumi.set(__self__, "use_distribution_kernel", use_distribution_kernel)
-
-    @property
-    @pulumi.getter(name="changeLog")
-    def change_log(self) -> str:
-        """
-        (DEPRECATED) Template change log details.
-        """
-        warnings.warn("""field is not used anymore""", DeprecationWarning)
-        pulumi.log.warn("""change_log is deprecated: field is not used anymore""")
-
-        return pulumi.get(self, "change_log")
 
     @property
     @pulumi.getter(name="customHostname")
     def custom_hostname(self) -> str:
         """
         Set up the server using the provided hostname instead of the default hostname.
         """
@@ -220,22 +172,14 @@
     @pulumi.getter(name="sshKeyName")
     def ssh_key_name(self) -> str:
         """
         Name of the ssh key that should be installed. Password login will be disabled.
         """
         return pulumi.get(self, "ssh_key_name")
 
-    @property
-    @pulumi.getter(name="useDistributionKernel")
-    def use_distribution_kernel(self) -> bool:
-        """
-        Use the distribution's native kernel instead of the recommended OVHcloud Kernel.
-        """
-        return pulumi.get(self, "use_distribution_kernel")
-
 
 @pulumi.output_type
 class GetInstallationTemplatePartitionSchemeResult(dict):
     def __init__(__self__, *,
                  hardware_raids: Sequence['outputs.GetInstallationTemplatePartitionSchemeHardwareRaidResult'],
                  name: str,
                  partitions: Sequence['outputs.GetInstallationTemplatePartitionSchemePartitionResult'],
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/me/ssh_key.py` & `pulumi_ovh-0.42.0/pulumi_ovh/me/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart.py` & `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product.py` & `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product_options.py` & `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product_options_plan.py` & `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_options_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/order/get_cart_product_plan.py` & `pulumi_ovh-0.42.0/pulumi_ovh/order/get_cart_product_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/order/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/order/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/provider.py` & `pulumi_ovh-0.42.0/pulumi_ovh/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vps/get_vps.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vps.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,16 +94,14 @@
         return pulumi.get(self, "cluster")
 
     @property
     @pulumi.getter
     def datacenter(self) -> Mapping[str, str]:
         """
         The datacenter in which the vps is located
-        * `datacenter.longname` - The fullname of the datacenter (ex: "Strasbourg SBG1")
-        * `datacenter.name` - The short name of the datacenter (ex: "sbg1)
         """
         return pulumi.get(self, "datacenter")
 
     @property
     @pulumi.getter
     def displayname(self) -> str:
         """
@@ -144,17 +142,14 @@
         return pulumi.get(self, "memory")
 
     @property
     @pulumi.getter
     def model(self) -> Mapping[str, str]:
         """
         A dict describing the type of vps.
-        * `model.name` - The model name (ex: model1)
-        * `model.offer` - The model human description (ex: "VPS 2016 SSD 1")
-        * `model.version` - The model version (ex: "2017v2")
         """
         return pulumi.get(self, "model")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vps/get_vpss.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vps/get_vpss.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/__init__.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/_inputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/cloud_project.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/cloud_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/dedicated_server.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/dedicated_server_interface.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/dedicated_server_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/get_vracks.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/get_vracks.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/ip_address.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/ip_loadbalancing.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/ip_loadbalancing.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/outputs.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh/vrack/vrack.py` & `pulumi_ovh-0.42.0/pulumi_ovh/vrack/vrack.py`

 * *Files identical despite different names*

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh.egg-info/PKG-INFO` & `pulumi_ovh-0.42.0/pulumi_ovh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-ovh
-Version: 0.40.1
+Version: 0.42.0
 Summary: A Pulumi package for creating and managing OVH resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ovh/pulumi-ovh
 Keywords: pulumi ovh category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-ovh Version: 0.40.1 Summary: A Pulumi
+Metadata-Version: 2.1 Name: pulumi-ovh Version: 0.42.0 Summary: A Pulumi
 package for creating and managing OVH resources. Home-page: https://
 www.pulumi.com License: Apache-2.0 Project-URL: Repository, https://github.com/
 ovh/pulumi-ovh Keywords: pulumi ovh category/cloud Platform: UNKNOWN Requires-
 Python: >=3.8 Description-Content-Type: text/markdown # OVH Resource Provider
 The OVH Resource Provider lets you manage [OVHcloud](https://www.ovhcloud.com/
 en/) resources. _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_][![GoDoc](https://godoc.org/github.com/ovh/
 pulumi-ovh?status.svg)](https://pkg.go.dev/github.com/ovh/pulumi-ovh/sdk) [!
```

### Comparing `pulumi_ovh-0.40.1/pulumi_ovh.egg-info/SOURCES.txt` & `pulumi_ovh-0.42.0/pulumi_ovh.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 pulumi_ovh/py.typed
 pulumi_ovh.egg-info/PKG-INFO
 pulumi_ovh.egg-info/SOURCES.txt
 pulumi_ovh.egg-info/dependency_links.txt
 pulumi_ovh.egg-info/not-zip-safe
 pulumi_ovh.egg-info/requires.txt
 pulumi_ovh.egg-info/top_level.txt
+pulumi_ovh/cloud/__init__.py
+pulumi_ovh/cloud/get_project.py
+pulumi_ovh/cloud/get_projects.py
+pulumi_ovh/cloud/outputs.py
 pulumi_ovh/cloudproject/__init__.py
 pulumi_ovh/cloudproject/_inputs.py
 pulumi_ovh/cloudproject/alerting.py
 pulumi_ovh/cloudproject/container_registry.py
 pulumi_ovh/cloudproject/container_registry_ip_restrictions_management.py
 pulumi_ovh/cloudproject/container_registry_ip_restrictions_registry.py
 pulumi_ovh/cloudproject/container_registry_oidc.py
@@ -77,14 +81,17 @@
 pulumi_ovh/cloudprojectdatabase/get_capabilities.py
 pulumi_ovh/cloudprojectdatabase/get_certificates.py
 pulumi_ovh/cloudprojectdatabase/get_database.py
 pulumi_ovh/cloudprojectdatabase/get_database_instance.py
 pulumi_ovh/cloudprojectdatabase/get_database_instances.py
 pulumi_ovh/cloudprojectdatabase/get_database_integration.py
 pulumi_ovh/cloudprojectdatabase/get_database_integrations.py
+pulumi_ovh/cloudprojectdatabase/get_database_log_subscription.py
+pulumi_ovh/cloudprojectdatabase/get_database_log_subscriptions.py
+pulumi_ovh/cloudprojectdatabase/get_database_postgre_sql_connection_pools.py
 pulumi_ovh/cloudprojectdatabase/get_databases.py
 pulumi_ovh/cloudprojectdatabase/get_ip_restrictions.py
 pulumi_ovh/cloudprojectdatabase/get_kafka_acl.py
 pulumi_ovh/cloudprojectdatabase/get_kafka_acls.py
 pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acl.py
 pulumi_ovh/cloudprojectdatabase/get_kafka_schema_registry_acls.py
 pulumi_ovh/cloudprojectdatabase/get_kafka_topic.py
@@ -95,14 +102,15 @@
 pulumi_ovh/cloudprojectdatabase/get_user.py
 pulumi_ovh/cloudprojectdatabase/get_users.py
 pulumi_ovh/cloudprojectdatabase/integration.py
 pulumi_ovh/cloudprojectdatabase/ip_restriction.py
 pulumi_ovh/cloudprojectdatabase/kafka_acl.py
 pulumi_ovh/cloudprojectdatabase/kafka_schema_registry_acl.py
 pulumi_ovh/cloudprojectdatabase/kafka_topic.py
+pulumi_ovh/cloudprojectdatabase/log_subscription.py
 pulumi_ovh/cloudprojectdatabase/m3_db_namespace.py
 pulumi_ovh/cloudprojectdatabase/m3_db_user.py
 pulumi_ovh/cloudprojectdatabase/mongo_db_user.py
 pulumi_ovh/cloudprojectdatabase/opensearch_pattern.py
 pulumi_ovh/cloudprojectdatabase/opensearch_user.py
 pulumi_ovh/cloudprojectdatabase/outputs.py
 pulumi_ovh/cloudprojectdatabase/postgres_sql_connection_pool.py
@@ -135,16 +143,18 @@
 pulumi_ovh/dedicated/server_install_task.py
 pulumi_ovh/dedicated/server_networking.py
 pulumi_ovh/dedicated/server_reboot_task.py
 pulumi_ovh/dedicated/server_update.py
 pulumi_ovh/domain/__init__.py
 pulumi_ovh/domain/_inputs.py
 pulumi_ovh/domain/get_zone.py
+pulumi_ovh/domain/get_zone_dns_sec.py
 pulumi_ovh/domain/outputs.py
 pulumi_ovh/domain/zone.py
+pulumi_ovh/domain/zone_dns_sec.py
 pulumi_ovh/domain/zone_record.py
 pulumi_ovh/domain/zone_redirection.py
 pulumi_ovh/hosting/__init__.py
 pulumi_ovh/hosting/_inputs.py
 pulumi_ovh/hosting/get_private_database.py
 pulumi_ovh/hosting/get_private_database_allowlist.py
 pulumi_ovh/hosting/get_private_database_db.py
@@ -167,16 +177,22 @@
 pulumi_ovh/iam/get_resource_groups.py
 pulumi_ovh/iam/outputs.py
 pulumi_ovh/iam/permissions_group.py
 pulumi_ovh/iam/policy.py
 pulumi_ovh/iam/resource_group.py
 pulumi_ovh/ip/__init__.py
 pulumi_ovh/ip/_inputs.py
+pulumi_ovh/ip/firewall.py
+pulumi_ovh/ip/firewall_rule.py
+pulumi_ovh/ip/get_firewall.py
+pulumi_ovh/ip/get_firewall_rule.py
+pulumi_ovh/ip/get_mitigation.py
 pulumi_ovh/ip/get_service.py
 pulumi_ovh/ip/ip_service.py
+pulumi_ovh/ip/mitigation.py
 pulumi_ovh/ip/move.py
 pulumi_ovh/ip/outputs.py
 pulumi_ovh/ip/reverse.py
 pulumi_ovh/iploadbalancing/__init__.py
 pulumi_ovh/iploadbalancing/_inputs.py
 pulumi_ovh/iploadbalancing/get_ip_load_balancing.py
 pulumi_ovh/iploadbalancing/get_vrack_network.py
@@ -189,14 +205,15 @@
 pulumi_ovh/iploadbalancing/outputs.py
 pulumi_ovh/iploadbalancing/refresh.py
 pulumi_ovh/iploadbalancing/tcp_farm.py
 pulumi_ovh/iploadbalancing/tcp_farm_server.py
 pulumi_ovh/iploadbalancing/tcp_frontend.py
 pulumi_ovh/iploadbalancing/tcp_route.py
 pulumi_ovh/iploadbalancing/tcp_route_rule.py
+pulumi_ovh/iploadbalancing/udp_frontend.py
 pulumi_ovh/iploadbalancing/vrack_network.py
 pulumi_ovh/me/__init__.py
 pulumi_ovh/me/_inputs.py
 pulumi_ovh/me/apio_auth2_client.py
 pulumi_ovh/me/get_apio_auth2_client.py
 pulumi_ovh/me/get_apio_auth2_clients.py
 pulumi_ovh/me/get_identity_group.py
@@ -222,16 +239,19 @@
 pulumi_ovh/order/get_cart.py
 pulumi_ovh/order/get_cart_product.py
 pulumi_ovh/order/get_cart_product_options.py
 pulumi_ovh/order/get_cart_product_options_plan.py
 pulumi_ovh/order/get_cart_product_plan.py
 pulumi_ovh/order/outputs.py
 pulumi_ovh/vps/__init__.py
+pulumi_ovh/vps/_inputs.py
 pulumi_ovh/vps/get_vps.py
 pulumi_ovh/vps/get_vpss.py
+pulumi_ovh/vps/outputs.py
+pulumi_ovh/vps/vps.py
 pulumi_ovh/vrack/__init__.py
 pulumi_ovh/vrack/_inputs.py
 pulumi_ovh/vrack/cloud_project.py
 pulumi_ovh/vrack/dedicated_server.py
 pulumi_ovh/vrack/dedicated_server_interface.py
 pulumi_ovh/vrack/get_vracks.py
 pulumi_ovh/vrack/ip_address.py
```

### Comparing `pulumi_ovh-0.40.1/setup.py` & `pulumi_ovh-0.42.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.40.1"
+VERSION = "0.42.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "ovh Pulumi Package - Development Version"
```

