# Comparing `tmp/tutor-contrib-aspects-0.94.0.tar.gz` & `tmp/tutor-contrib-aspects-0.95.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.94.0.tar", last modified: Mon Apr  8 14:12:40 2024, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.95.0.tar", last modified: Tue Apr  9 15:26:06 2024, max compression
```

## Comparing `tutor-contrib-aspects-0.94.0.tar` & `tutor-contrib-aspects-0.95.0.tar`

### file list

```diff
@@ -1,274 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.402155 tutor-contrib-aspects-0.94.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-08 14:12:40.402155 tutor-contrib-aspects-0.94.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.362155 tutor-contrib-aspects-0.94.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 14:12:40.402155 tutor-contrib-aspects-0.94.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.402155 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-08 14:12:40.000000 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18366 2024-04-08 14:12:40.000000 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:12:40.000000 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 14:12:40.000000 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 14:12:40.000000 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 14:12:40.000000 tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.362155 tutor-contrib-aspects-0.94.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/asset_command_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/commands_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/commands_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.366155 tutor-contrib-aspects-0.94.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/clickhouse-extra-sql
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/clickhouse-server-config
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/clickhouse-user-config
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/openedx-common-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/openedx-development-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/superset-extra-asset-translations
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/superset-extra-roles
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/superset-row-level-security
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/superset-sso-assignment-rules
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/patches/xapi-db-load-config-yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.370155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.370155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.370155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.370155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.370155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/users/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/env
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.374155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/security/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/security/partials/
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.378155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.382155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.382155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.390155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.390155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    21489 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.390155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.358155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/lms/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.398155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/superset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/base-docker-compose-services
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.362155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:12:40.402155 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 14:12:35.000000 tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.463347 tutor-contrib-aspects-0.95.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/asset_command_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.463347 tutor-contrib-aspects-0.95.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-extra-sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-server-config
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-user-config
+-rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-common-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-development-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-extra-asset-translations
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-extra-roles
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-row-level-security
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-sso-assignment-rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/xapi-db-load-config-yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.455347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.455347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.455347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/env
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.483348 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.483348 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    22597 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.483348 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/lms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
```

### Comparing `tutor-contrib-aspects-0.94.0/LICENSE` & `tutor-contrib-aspects-0.95.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/PKG-INFO` & `tutor-contrib-aspects-0.95.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.94.0
+Version: 0.95.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.94.0/README.rst` & `tutor-contrib-aspects-0.95.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/setup.py` & `tutor-contrib-aspects-0.95.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.94.0
+Version: 0.95.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.94.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
+tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
@@ -177,14 +178,15 @@
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
+tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
 tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
@@ -211,14 +213,15 @@
 tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
 tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
 tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
 tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
 tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
 tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
 tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
 tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
 tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
 tutoraspects/templates/openedx-assets/queries/indexed_events.sql
 tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
 tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
 tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
 tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
```

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/asset_command_helpers.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/asset_command_helpers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/commands_v0.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/commands_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/commands_v1.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/commands_v1.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/clickhouse-server-config` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-server-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/clickhouse-user-config` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-user-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/openedx-common-settings` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/patches/xapi-db-load-config-yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/patches/xapi-db-load-config-yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/conf/README.md` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/conf/README.md`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/k8s.toml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/k8s.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         - 682
         - 695
         - 701
         - 770
         - 783
         - 816
         - 901
+        - 921
         scope: global
       id: 114
     '156':
       crossFilters:
         chartsInScope:
         - 114
         - 154
@@ -42,14 +43,15 @@
         - 682
         - 695
         - 701
         - 770
         - 783
         - 816
         - 901
+        - 921
         scope: global
       id: 156
     '325':
       crossFilters:
         chartsInScope:
         - 114
         - 154
@@ -63,14 +65,15 @@
         - 682
         - 695
         - 701
         - 770
         - 783
         - 816
         - 901
+        - 921
         scope: global
       id: 325
     '816':
       crossFilters:
         chartsInScope:
         - 114
         - 154
@@ -84,14 +87,15 @@
         - 625
         - 682
         - 695
         - 701
         - 770
         - 783
         - 901
+        - 921
         scope: global
       id: 816
     '901':
       crossFilters:
         chartsInScope:
         - 114
         - 154
@@ -105,16 +109,39 @@
         - 625
         - 682
         - 695
         - 701
         - 770
         - 783
         - 816
+        - 921
         scope: global
       id: 901
+    '921':
+      crossFilters:
+        chartsInScope:
+        - 114
+        - 154
+        - 156
+        - 229
+        - 325
+        - 327
+        - 339
+        - 516
+        - 597
+        - 625
+        - 682
+        - 695
+        - 701
+        - 770
+        - 783
+        - 816
+        - 901
+        scope: global
+      id: 921
   color_scheme: ''
   color_scheme_domain: []
   cross_filters_enabled: false
   default_filters: '{}'
   expanded_slices: {}
   global_chart_configuration:
     chartsInScope:
@@ -131,14 +158,15 @@
     - 682
     - 695
     - 701
     - 770
     - 783
     - 816
     - 901
+    - 921
     scope:
       excluded: []
       rootPath:
       - ROOT_ID
   label_colors: {}
   native_filter_configuration:
   - cascadeParentIds: []
@@ -376,16 +404,20 @@
     targets:
     - column:
         name: video_name_with_location
       datasetUuid: 417b2035-8fa1-4c60-a405-4b1947c3c966
     type: NATIVE_FILTER
   refresh_frequency: 0
   shared_label_colors:
-    audit: '#454E7C'
-    registered: '#1FA8C9'
+    All videos viewed: '#E04355'
+    At least one video viewed: '#3CCCCB'
+    Full view: '#A868B7'
+    Partial view: '#8FD3E4'
+    Total plays: '#FF7F44'
+    Unique Watchers: '#FCC700'
   timed_refresh_immune_slices: []
 position:
   CHART-AZZnl_lpMv:
     children: []
     id: CHART-AZZnl_lpMv
     meta:
       chartId: 229
@@ -500,14 +532,29 @@
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-NR4UTAs9K
     - ROW-GWTTmZ2jDJ
     type: CHART
+  CHART-VwIFwB80km:
+    children: []
+    id: CHART-VwIFwB80km
+    meta:
+      chartId: 921
+      height: 64
+      sliceName: Partial and full views per video
+      uuid: 5052449a-424c-41bf-b8b0-d920424c4784
+      width: 12
+    parents:
+    - ROOT_ID
+    - TABS-SNeKAJcjhd
+    - TAB-7PGDduCA7
+    - ROW-lnHZ40DjeR
+    type: CHART
   CHART-evjVO-ZSSd:
     children: []
     id: CHART-evjVO-ZSSd
     meta:
       chartId: 156
       height: 50
       sliceName: Enrollments By Enrollment Mode
@@ -535,15 +582,15 @@
     - ROW-Lt0M87yMb3
     type: CHART
   CHART-jfm-20qPKn:
     children: []
     id: CHART-jfm-20qPKn
     meta:
       chartId: 816
-      height: 50
+      height: 55
       sliceName: Video engagement by section/subsection
       uuid: 21861f47-9e8b-4715-b1ff-e7f4aa595c14
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-7PGDduCA7
@@ -921,14 +968,25 @@
     meta:
       background: BACKGROUND_TRANSPARENT
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-eE0OQxuju
     type: ROW
+  ROW-lnHZ40DjeR:
+    children:
+    - CHART-VwIFwB80km
+    id: ROW-lnHZ40DjeR
+    meta:
+      background: BACKGROUND_TRANSPARENT
+    parents:
+    - ROOT_ID
+    - TABS-SNeKAJcjhd
+    - TAB-7PGDduCA7
+    type: ROW
   ROW-nNEywSG0jX:
     children:
     - MARKDOWN-NaNsE4EBKf
     id: ROW-nNEywSG0jX
     meta:
       background: BACKGROUND_TRANSPARENT
     parents:
@@ -960,14 +1018,15 @@
     - TABS-SNeKAJcjhd
     type: TAB
   TAB-7PGDduCA7:
     children:
     - ROW-nNEywSG0jX
     - ROW-BO2IHCiYF8
     - ROW-HPGIhOIs65
+    - ROW-lnHZ40DjeR
     id: TAB-7PGDduCA7
     meta:
       defaultText: Tab title
       placeholder: Tab title
       text: Video Engagement
     parents:
     - ROOT_ID
```

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
     select
         emission_time,
         org,
         course_key,
         splitByString('/xblock/', object_id)[-1] as video_id,
         actor_id,
         verb_id,
-        video_position
+        video_position,
+        video_duration
     from {{ ASPECTS_XAPI_DATABASE }}.{{ ASPECTS_VIDEO_PLAYBACK_EVENTS_TABLE }}
     where 1=1
     {% include 'openedx-assets/queries/common_filters.sql' %}
 ), starts as (
     select *
     from video_events
     where verb_id = 'https://w3id.org/xapi/video/verbs/played'
@@ -30,15 +31,16 @@
         starts.course_key as course_key,
         starts.video_id as video_id,
         starts.actor_id,
         cast(starts.video_position as Int32) as start_position,
         cast(ends.video_position as Int32) as end_position,
         starts.emission_time as started_at,
         ends.emission_time as ended_at,
-        ends.verb_id as end_type
+        ends.verb_id as end_type,
+        starts.video_duration as video_duration
     from
         starts
         left asof join ends
             on (starts.org = ends.org
                 and starts.course_key = ends.course_key
                 and starts.video_id = ends.video_id
                 and starts.actor_id = ends.actor_id
@@ -50,15 +52,16 @@
         blocks.course_name as course_name,
         blocks.course_run as course_run,
         blocks.block_name as video_name,
         blocks.display_name_with_location as video_name_with_location,
         segments.actor_id as actor_id,
         segments.started_at as started_at,
         segments.start_position - (segments.start_position % 5) as start_position,
-        segments.end_position - (segments.end_position % 5) as end_position
+        segments.end_position - (segments.end_position % 5) as end_position,
+        segments.video_duration as video_duration
     from
         segments
         join {{ DBT_PROFILE_TARGET_DATABASE }}.dim_course_blocks blocks
             on (segments.course_key = blocks.course_key
                 and segments.video_id = blocks.block_id)
 )
 
@@ -67,15 +70,16 @@
     course_key,
     course_name,
     course_run,
     video_name,
     video_name_with_location,
     actor_id,
     started_at,
-    arrayJoin(range(start_position, end_position, 5)) as segment_start
+    arrayJoin(range(start_position, end_position, 5)) as segment_start,
+    video_duration
 from enriched_segments
 where
     {% raw %}
     {% if get_filters('video_name_with_location', remove_filter=True) == [] %}
     1=1
     {% elif filter_values('video_name_with_location') != [] %}
     video_name_with_location in {{ filter_values('video_name_with_location') | where_in }}
```

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.94.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql` & `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql`

 * *Files identical despite different names*
