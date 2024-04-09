# Comparing `tmp/tutor-contrib-aspects-0.95.0.tar.gz` & `tmp/tutor-contrib-aspects-0.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.95.0.tar", last modified: Tue Apr  9 15:26:06 2024, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.96.0.tar", last modified: Tue Apr  9 16:46:17 2024, max compression
```

## Comparing `tutor-contrib-aspects-0.95.0.tar` & `tutor-contrib-aspects-0.96.0.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 15:26:06.000000 tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.463347 tutor-contrib-aspects-0.95.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/asset_command_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/commands_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/commands_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.463347 tutor-contrib-aspects-0.95.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-extra-sql
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-server-config
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-user-config
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-common-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-development-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-extra-asset-translations
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-extra-roles
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-row-level-security
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/superset-sso-assignment-rules
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/patches/xapi-db-load-config-yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.455347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.467347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.455347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/users/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.455347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/env
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.471347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/partials/
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.475347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.483348 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.483348 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    22597 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.483348 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/lms/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.491347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/superset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/base-docker-compose-services
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.459347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:26:06.495347 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 15:26:01.000000 tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.818095 tutor-contrib-aspects-0.96.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 16:46:17.818095 tutor-contrib-aspects-0.96.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.782095 tutor-contrib-aspects-0.96.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 16:46:17.818095 tutor-contrib-aspects-0.96.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.818095 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 16:46:17.000000 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-09 16:46:17.000000 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:46:17.000000 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 16:46:17.000000 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 16:46:17.000000 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 16:46:17.000000 tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.786095 tutor-contrib-aspects-0.96.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/asset_command_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.790095 tutor-contrib-aspects-0.96.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/clickhouse-extra-sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/clickhouse-server-config
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/clickhouse-user-config
+-rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/openedx-common-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/openedx-development-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/superset-extra-asset-translations
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/superset-extra-roles
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/superset-row-level-security
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/superset-sso-assignment-rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/patches/xapi-db-load-config-yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.790095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.782095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.790095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.778095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.790095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.790095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.790095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.778095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.778095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/env
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.794095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/security/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.798095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.782095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.782095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.806095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.806095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.806095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.782095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/lms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.814095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.782095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:46:17.818095 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/common_filters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 16:46:12.000000 tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
```

### Comparing `tutor-contrib-aspects-0.95.0/LICENSE` & `tutor-contrib-aspects-0.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/PKG-INFO` & `tutor-contrib-aspects-0.96.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.95.0
+Version: 0.96.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.95.0/README.rst` & `tutor-contrib-aspects-0.96.0/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/setup.py` & `tutor-contrib-aspects-0.96.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.95.0
+Version: 0.96.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.95.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.96.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/asset_command_helpers.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/asset_command_helpers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/commands_v0.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/commands_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/commands_v1.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/commands_v1.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-server-config` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/clickhouse-server-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/clickhouse-user-config` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/clickhouse-user-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/openedx-common-settings` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/patches/xapi-db-load-config-yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/patches/xapi-db-load-config-yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,14 +368,18 @@
         ("SUPERSET_USER_COURSES_CACHE_TIMEOUT", 300),
         ("SUPERSET_BLOCK_STUDENT_ACCESS", True),
         # This setting allows Superset to run behind a reverse proxy in HTTPS and
         # redirect to the correct http/s based on the headers sent from the proxy.
         # By default it is on if Caddy is enabled, but it can be set separately in
         # case you are running a different proxy or otherwise have different needs.
         ("SUPERSET_ENABLE_PROXY_FIX", "{{ENABLE_WEB_PROXY}}"),
+        # This setting allows operators to automatically refresh the datasets
+        # in the Superset database. This is useful for keeping the columns up to
+        # date with the latest changes in DBT.
+        ("SUPERSET_REFRESH_DATASETS", False),
         ######################
         # dbt Settings
         # For the most part you shouldn't have to touch these
         # DBT_PROFILE_* settings get passed into the dbt_profile.yml file.
         # For now we are pulling this from github, which should allow maximum
         # flexibility for forking, running branches, specific versions, etc.
         ("DBT_REPOSITORY", "https://github.com/openedx/aspects-dbt"),
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/conf/README.md` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/conf/README.md`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from copy import deepcopy
 from pathlib import Path
 
 from superset import security_manager
 from superset.examples.utils import load_configs_from_directory
 from superset.extensions import db
 from superset.models.dashboard import Dashboard
+from superset.connectors.sqla.models import SqlaTable
 from superset.utils.database import get_or_create_db
 from superset.models.embedded_dashboard import EmbeddedDashboard
 from pythonpath.localization import get_translation
 
 BASE_DIR = "/app/assets/superset"
 
 ASSET_FOLDER_MAPPING = {
@@ -87,14 +88,15 @@
                     write_asset_to_file(asset, asset_name, folder, file_name, roles)
                     break
 
     import_databases()
     import_assets()
     update_dashboard_roles(roles)
     update_embeddable_uuids()
+    update_datasets()
 
 
 def import_databases():
     """Import databases from settings"""
     databases = {{SUPERSET_DATABASES}}
     for database_name, uri in databases.items():
         create_superset_db(database_name, uri)
@@ -254,15 +256,14 @@
         if user:
             owners.append(user)
 
     for dashboard_uuid, role_ids in roles.items():
         dashboard = db.session.query(Dashboard).filter_by(uuid=dashboard_uuid).one()
         print("Importing dashboard roles", dashboard_uuid, role_ids)
         dashboard.roles = role_ids
-        dashboard.published = True
         if owners:
             dashboard.owners = owners
         db.session.commit()
 
 
 def update_embeddable_uuids():
     """Update the uuids of the embeddable dashboards"""
@@ -278,9 +279,21 @@
             embedded_dashboard.dashboard_id = dashboard.id
         embedded_dashboard.uuid = embeddable_uuid
 
         db.session.add(embedded_dashboard)
         db.session.commit()
 
 
+def update_datasets():
+    """Update the datasets"""
+    print("Refreshing datasets")
+    if {{SUPERSET_REFRESH_DATASETS}}:
+        datasets = (
+            db.session.query(SqlaTable).all()
+        )
+        for dataset in datasets:
+            print(f"Refreshing dataset {dataset.table_name}")
+            dataset.fetch_metadata(commit=True)
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import uuid
 from datetime import datetime
 from unittest.mock import patch
 
 import sqlparse
 from flask import g
 from superset import security_manager
-from superset.charts.data.commands.get_data_command import ChartDataCommand
+from superset.commands.chart.data.get_data_command import ChartDataCommand
 from superset.charts.schemas import ChartDataQueryContextSchema
 from superset.extensions import db
 from superset.models.dashboard import Dashboard
 from superset.models.slice import Slice
 
 logger = logging.getLogger("performance_metrics")
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 # Enable use of variables in datasets/queries
 FEATURE_FLAGS = {
     "ALERT_REPORTS": True,
     "DASHBOARD_RBAC": True,
     "EMBEDDABLE_CHARTS": True,
     "EMBEDDED_SUPERSET": True,
     "ENABLE_TEMPLATE_PROCESSING": True,
+    "TAGGING_SYSTEM": True,
 }
 
 # Add this custom template processor which returns the list of courses the current user can access
 from openedx_jinja_filters import *
 
 def can_view_courses_wrapper(*args, **kwargs):
     """
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/k8s.toml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/k8s.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Superset image with additional database drivers
 # https://hub.docker.com/r/apache/superset
 # https://github.com/apache/superset/releases
 # https://github.com/apache/superset/blob/master/Dockerfile
 # https://superset.apache.org/docs/databases/installing-database-drivers
-FROM apache/superset:3.0.1
+FROM apache/superset:4.0.0
 
 USER root
 
 COPY ./requirements.txt /app/requirements.txt
 
 RUN pip install -r /app/requirements.txt
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - grade_bucket
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     sqlExpression: null
     subject: enrollment_status
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: enrollment_status_date
+  annotation_layers: []
   color_picker:
     a: 1
     b: 135
     g: 122
     r: 0
   extra_form_data: {}
   header_font_size: 0.4
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   extra_form_data: {}
   header_font_size: 0.4
   metric:
     aggregate: COUNT_DISTINCT
     column:
       advanced_data_type: null
       certification_details: null
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     filterOptionName: filter_0fpmws3t1h6a_md2ud9xse7m
     isExtra: false
     isNew: false
     operator: ==
     operatorId: EQUALS
     sqlExpression: null
     subject: success
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - attempts
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 dataset_uuid: a5db584d-c8dd-4acc-889e-074288c38433
 description: This chart displays counts of the number of times hints (including displaying
   the answer itself) were displayed for each learner who eventually answered the problem
   correctly. If the problem had no hint or answer display configured this chart will
   group everyone into "0".
 params:
   adhoc_filters: []
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - total_hints
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - grade_bucket
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - responses
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     sqlExpression: null
     subject: enrollment_status
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   color_scheme: supersetColors
   date_format: smart_date
   extra_form_data: {}
   groupby:
   - expressionType: SQL
     label: Enrollment Mode
     sqlExpression: |-
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 cache_timeout: null
 certification_details: null
 certified_by: null
 dataset_uuid: a2823d2e-54c4-4378-98c2-817f000c14ab
 description: null
 params:
   adhoc_filters: []
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - num_posts
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 certified_by: null
 dataset_uuid: 981f30d9-b2f0-4a0b-9e95-0ee0e06db806
 description: The number of students who have responded to a question, and whether
   they have ever answered correctly. Students can answer some questions multiple times,
   but this chart counts each student only once per question.
 params:
   adhoc_filters: []
+  annotation_layers: []
   bar_stacked: true
   bottom_margin: auto
   color_scheme: supersetColors
   columns:
   - success
   extra_form_data: {}
   groupby:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - video_name_with_location
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: started_at
+  annotation_layers: []
   bar_stacked: true
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - segment_start
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 params:
   adhoc_filters:
   - clause: WHERE
     comparator: No filter
     expressionType: SIMPLE
     operator: TEMPORAL_RANGE
     subject: emission_time
+  annotation_layers: []
   bottom_margin: auto
   color_scheme: supersetColors
   columns: []
   extra_form_data: {}
   groupby:
   - video_name_with_location
   metrics:
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 _file_name: Instructor_Dashboard.yaml
 _roles:
 - '{{ SUPERSET_ROLES_MAPPING.instructor }}'
+certification_details: null
+certified_by: null
 css: ''
 dashboard_title: Instructor Dashboard
 description: null
 metadata:
   chart_configuration:
     '114':
       crossFilters:
@@ -416,105 +418,105 @@
     Unique Watchers: '#FCC700'
   timed_refresh_immune_slices: []
 position:
   CHART-AZZnl_lpMv:
     children: []
     id: CHART-AZZnl_lpMv
     meta:
-      chartId: 229
+      chartId: 22
       height: 50
       sliceName: Watches Per Video
       uuid: 829c1d5b-2844-4115-876a-34ad3b3cad64
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-7PGDduCA7
     - ROW-BO2IHCiYF8
     type: CHART
   CHART-GFCO8s2cxv:
     children: []
     id: CHART-GFCO8s2cxv
     meta:
-      chartId: 625
+      chartId: 20
       height: 50
       sliceName: Distribution Of Responses
       uuid: f1651c44-a8f4-4b44-ad49-962823009319
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-lZkhTcIAro
     type: CHART
   CHART-GJJ8VYQ03v:
     children: []
     id: CHART-GJJ8VYQ03v
     meta:
-      chartId: 783
+      chartId: 6
       height: 50
       sliceName: Posts per user
       uuid: bc191ce7-f39d-48db-86a9-d19949f4211d
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-eE0OQxuju
     - ROW-la1XxBueHN
     type: CHART
   CHART-Jr-gNVms2Q:
     children: []
     id: CHART-Jr-gNVms2Q
     meta:
-      chartId: 114
+      chartId: 13
       height: 50
       sliceName: Enrollment Events Per Day
       uuid: bb1147cc-b7bc-44b7-b06a-79b0db6626aa
       width: 8
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-8BxDuJd9Jb
     - ROW-je_Wqya3Ga
     type: CHART
   CHART-OMy4wjRBWt:
     children: []
     id: CHART-OMy4wjRBWt
     meta:
-      chartId: 682
+      chartId: 28
       height: 50
       sliceName: Watched Video Segments
       uuid: 2985a9db-c338-4008-af52-2930b81ee2e5
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-CLiLC4zxo
     - ROW-lN_IXnlUhL
     type: CHART
   CHART-RTO33WE9FH:
     children: []
     id: CHART-RTO33WE9FH
     meta:
-      chartId: 597
+      chartId: 16
       height: 50
       sliceName: Responses Per Problem
       uuid: a3e79162-4ace-4349-ab34-89aa60ae75ed
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-NR4UTAs9K
     - ROW-87X0ypdHH_
     type: CHART
   CHART-Tej2oLPBAl:
     children: []
     id: CHART-Tej2oLPBAl
     meta:
-      chartId: 701
+      chartId: 38
       height: 50
       sliceName: Transcripts / Captions Per Video
       uuid: 6b830def-f3ca-4b4c-9455-7a7b7354bce8
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
@@ -551,135 +553,135 @@
     - TAB-7PGDduCA7
     - ROW-lnHZ40DjeR
     type: CHART
   CHART-evjVO-ZSSd:
     children: []
     id: CHART-evjVO-ZSSd
     meta:
-      chartId: 156
+      chartId: 39
       height: 50
       sliceName: Enrollments By Enrollment Mode
       uuid: 05ed7102-5464-4e2f-86ae-31700b787cc3
       width: 4
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-8BxDuJd9Jb
     - ROW-je_Wqya3Ga
     type: CHART
   CHART-j3trfNh8_p:
     children: []
     id: CHART-j3trfNh8_p
     meta:
-      chartId: 325
+      chartId: 30
       height: 50
       sliceName: Pageview engagement by section/subsection
       uuid: 366a8193-30c3-4aaf-a1ac-360609dfa0ed
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-4Z1kfBQZO
     - ROW-Lt0M87yMb3
     type: CHART
   CHART-jfm-20qPKn:
     children: []
     id: CHART-jfm-20qPKn
     meta:
-      chartId: 816
-      height: 55
+      chartId: 11
+      height: 50
       sliceName: Video engagement by section/subsection
       uuid: 21861f47-9e8b-4715-b1ff-e7f4aa595c14
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-7PGDduCA7
     - ROW-HPGIhOIs65
     type: CHART
   CHART-lTr8DL3XuI:
     children: []
     id: CHART-lTr8DL3XuI
     meta:
-      chartId: 695
+      chartId: 4
       height: 50
       sliceName: Distribution Of Hints Per Correct Answer
       uuid: ee94be4c-6fdd-4295-b43c-40890d6c549d
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-GKMT8uEu6K
     type: CHART
   CHART-o56v9yEe2I:
     children: []
     id: CHART-o56v9yEe2I
     meta:
-      chartId: 770
+      chartId: 32
       height: 50
       sliceName: Distribution Of Problem Grades
       uuid: 4f7e3606-f5de-4643-97c0-bbb6340a3df2
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-lZkhTcIAro
     type: CHART
   CHART-qG1WaGKl_b:
     children: []
     id: CHART-qG1WaGKl_b
     meta:
-      chartId: 154
+      chartId: 35
       height: 50
       sliceName: Distinct forum users
       uuid: feb323ad-c819-49ca-a336-584bd9ff1a2e
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-eE0OQxuju
     - ROW-la1XxBueHN
     type: CHART
   CHART-rnb6PSwCOS:
     children: []
     id: CHART-rnb6PSwCOS
     meta:
-      chartId: 339
+      chartId: 17
       height: 50
       sliceName: Currently Enrolled Learners Per Day
       uuid: ed2fe731-6544-422f-bc55-42f399f48b2c
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-8BxDuJd9Jb
     - ROW-K8s_8uq9IP
     type: CHART
   CHART-tWnaoVNNTH:
     children: []
     id: CHART-tWnaoVNNTH
     meta:
-      chartId: 327
+      chartId: 12
       height: 50
       sliceName: Distribution Of Attempts
       uuid: db90930f-f16e-4c32-8050-0e4abae28f4c
       width: 6
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
     - TAB-pOd4znTAV
     - ROW-GKMT8uEu6K
     type: CHART
   CHART-w-k4N2T_L8:
     children: []
     id: CHART-w-k4N2T_L8
     meta:
-      chartId: 516
+      chartId: 2
       height: 50
       sliceName: Course Grade Distribution
       uuid: f9adbc85-1f50-4c04-ace3-31ba7390de5e
       width: 12
     parents:
     - ROOT_ID
     - TABS-SNeKAJcjhd
@@ -1126,10 +1128,11 @@
     - TAB-nXpinnLEX
     - TAB-4Z1kfBQZO
     id: TABS-SNeKAJcjhd
     meta: {}
     parents:
     - ROOT_ID
     type: TABS
+published: true
 slug: instructor-dashboard
 uuid: 1d6bf904-f53f-47fd-b1c9-6cd7e284d286
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,75 @@
-_file_name: course_names.yaml
+_file_name: posts_per_user.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
+  column_name: num_posts
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: UInt64
+  verbose_name: Number of Posts
+- advanced_data_type: null
+  column_name: actor_id
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: String
+  verbose_name: Actor ID
+- advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -56,22 +81,32 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: COUNT(*)
+  expression: count(*)
   extra: {}
+  metric_name: users
+  metric_type: null
+  verbose_name: Number Of Users
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: COUNT(*)
+  extra: null
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
-sql: select * from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_names
-table_name: course_names
-template_params: null
-uuid: 41278a97-d0ff-4645-9514-d79f80d275df
+sql: |-
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/posts_per_user.sql' %}{% endfilter %}
+table_name: posts_per_user
+template_params: {}
+uuid: a2823d2e-54c4-4378-98c2-817f000c14ab
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -223,12 +223,12 @@
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: superset
-sql: 'select * from '
+sql: 'select * from dashboards'
 table_name: dashboards
 template_params: null
 uuid: 3dee777a-3dd4-4fcb-a749-4d13651b3444
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-_file_name: dim_course_problems.yaml
+_file_name: indexed_events.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: problem_name_with_location
+  column_name: actor_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Name With Location
+  verbose_name: Actor ID
 - advanced_data_type: null
   column_name: course_key
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
@@ -46,37 +46,61 @@
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: problem_id
+  column_name: event_id
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: UUID
+  verbose_name: Event ID
+- advanced_data_type: null
+  column_name: emission_time
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: true
+  python_date_format: null
+  type: DateTime
+  verbose_name: Emission Time
+- advanced_data_type: null
+  column_name: object_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Id
+  verbose_name: Object ID
 - advanced_data_type: null
-  column_name: problem_name
+  column_name: verb_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Name
+  verbose_name: Verb ID
 - advanced_data_type: null
   column_name: org
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
@@ -86,29 +110,29 @@
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
-filter_select_enabled: false
-main_dttm_col: null
+filter_select_enabled: true
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*)
+  expression: COUNT(*)
   extra: {}
   metric_name: count
-  metric_type: null
-  verbose_name: null
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: true
+normalize_columns: false
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/dim_course_problems.sql' %}{% endfilter %}
-table_name: dim_course_problems
-template_params: {}
-uuid: 008e2907-fc6b-45ef-bf85-73a04c5791ff
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/indexed_events.sql' %}{% endfilter %}
+table_name: indexed_events
+template_params: null
+uuid: d6b1402a-393b-4595-9fbc-86aa9beacae9
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 _file_name: dim_course_videos.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: video_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Video Name With Location
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: video_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Video Id
 - advanced_data_type: null
   column_name: video_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Video Name
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,141 +1,151 @@
 _file_name: fact_course_grades.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
+  column_name: grade_type
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: Nullable(String)
+  verbose_name: Grade Type
+- advanced_data_type: null
+  column_name: scaled_score
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: Float64
+  verbose_name: Scaled Score
+- advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Actor Id
 - advanced_data_type: null
   column_name: grade_bucket
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Grade Bucket
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: emission_time
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: true
   python_date_format: null
   type: DateTime
   verbose_name: Emission Time
 - advanced_data_type: null
   column_name: entity_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Entity Name
 - advanced_data_type: null
-  column_name: scaled_score
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: Float
-  verbose_name: Scaled Score
-- advanced_data_type: null
-  column_name: grade_type
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Grade Type
-- advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
+  expression: COUNT(*)
+  extra: null
+  metric_name: count
+  metric_type: count
+  verbose_name: COUNT(*)
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
   expression: count(*)
   extra: {}
   metric_name: students
   metric_type: null
   verbose_name: Students
   warning_text: null
 normalize_columns: true
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,126 +1,158 @@
-_file_name: fact_enrollments.yaml
+_file_name: fact_watched_video_segments.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: enrollment_mode
+  column_name: video_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: LowCardinality(String)
-  verbose_name: Enrollment Mode
+  type: String
+  verbose_name: Video Name With Location
+- advanced_data_type: null
+  column_name: segment_start
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: Int64
+  verbose_name: Segment Start
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor Id
+  verbose_name: Actor ID
+- advanced_data_type: null
+  column_name: started_at
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: true
+  python_date_format: null
+  type: DateTime
+  verbose_name: Started At
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: emission_time
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: true
-  python_date_format: null
-  type: DateTime
-  verbose_name: Emission Time
-- advanced_data_type: null
-  column_name: enrollment_status
+  column_name: video_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Enrollment Status
+  verbose_name: Video Name
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: started_at
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*)
+  expression: count(*) - count(distinct actor_id)
   extra: {}
+  metric_name: repeat_views
+  metric_type: null
+  verbose_name: Repeat Views
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: count(*)
+  extra:
+    warning_markdown: ''
   metric_name: count
   metric_type: null
-  verbose_name: null
+  verbose_name: Total Views
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: count(distinct actor_id)
+  extra: {}
+  metric_name: unique_viewers
+  metric_type: null
+  verbose_name: Unique Viewers
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_enrollments.sql' %}{% endfilter %}
-table_name: fact_enrollments
-template_params: {}
-uuid: a234545d-08ff-480d-8361-961c3d15f14f
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_watched_video_segments.sql' %}{% endfilter %}
+table_name: fact_watched_video_segments
+template_params: null
+uuid: c2c391b3-3403-4f05-bc0b-3de53bd366ec
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,113 +1,114 @@
-_file_name: fact_enrollments_by_day.yaml
+_file_name: fact_enrollments.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: enrollment_status_date
+  column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: Date
-  verbose_name: Enrollment Status Date
+  type: String
+  verbose_name: Actor Id
 - advanced_data_type: null
-  column_name: enrollment_mode
+  column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: LowCardinality(String)
-  verbose_name: Enrollment Mode
+  type: String
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: actor_id
+  column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor Id
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: course_key
+  column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Key
+  verbose_name: Course Run
 - advanced_data_type: null
-  column_name: course_name
+  column_name: emission_time
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: String
-  verbose_name: Course Name
+  type: DateTime
+  verbose_name: Emission Time
 - advanced_data_type: null
-  column_name: course_run
+  column_name: enrollment_mode
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Run
+  verbose_name: Enrollment Mode
 - advanced_data_type: null
   column_name: enrollment_status
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Enrollment Status
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
   expression: count(*)
   extra: {}
   metric_name: count
@@ -115,12 +116,12 @@
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_enrollments_by_day.sql' %}{% endfilter %}
-table_name: fact_enrollments_by_day
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_enrollments.sql' %}{% endfilter %}
+table_name: fact_enrollments
 template_params: {}
-uuid: 352311fe-12f0-470c-8b8c-d4f6a3936b3d
+uuid: a234545d-08ff-480d-8361-961c3d15f14f
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,125 +1,126 @@
 _file_name: fact_forum_interactions.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Actor Id
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: event_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: UUID
   verbose_name: Event ID
 - advanced_data_type: null
   column_name: emission_time
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: true
   python_date_format: null
   type: DateTime
   verbose_name: Emission Time
 - advanced_data_type: null
   column_name: object_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Object ID
 - advanced_data_type: null
   column_name: verb_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Verb ID
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
   expression: count(*)
   extra: {}
   metric_name: count
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,134 +1,135 @@
-_file_name: fact_learner_problem_course_summary.yaml
+_file_name: fact_learner_problem_summary.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: num_answers_displayed
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: UInt64
   verbose_name: Number of Answers Displayed
 - advanced_data_type: null
   column_name: num_hints_displayed
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: UInt64
   verbose_name: Number of Hints Displayed
 - advanced_data_type: null
   column_name: problem_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Problem Name With Location
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Actor ID
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: problem_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Problem Name
 - advanced_data_type: null
   column_name: attempts
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: Int16
   verbose_name: Attempts
 - advanced_data_type: null
   column_name: success
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: Bool
   verbose_name: Success
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -140,23 +141,32 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
+  expression: COUNT(*)
+  extra: null
+  metric_name: count
+  metric_type: count
+  verbose_name: COUNT(*)
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
   expression: count(*)
   extra: {}
-  metric_name: count
+  metric_name: students
   metric_type: null
-  verbose_name: null
+  verbose_name: Students
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_learner_problem_course_summary.sql' %}{% endfilter %}
-table_name: fact_learner_problem_course_summary
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_learner_problem_summary.sql' %}{% endfilter %}
+table_name: fact_learner_problem_summary
 template_params: null
-uuid: 981f30d9-b2f0-4a0b-9e95-0ee0e06db806
+uuid: 9362354c-1541-43c2-b769-da9818236298
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,134 +1,135 @@
-_file_name: fact_learner_problem_summary.yaml
+_file_name: fact_learner_problem_course_summary.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: num_answers_displayed
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: UInt64
   verbose_name: Number of Answers Displayed
 - advanced_data_type: null
   column_name: num_hints_displayed
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: UInt64
   verbose_name: Number of Hints Displayed
 - advanced_data_type: null
   column_name: problem_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Problem Name With Location
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Actor ID
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: problem_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Problem Name
 - advanced_data_type: null
   column_name: attempts
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: Int16
   verbose_name: Attempts
 - advanced_data_type: null
   column_name: success
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: Bool
   verbose_name: Success
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -142,21 +143,21 @@
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
   expression: count(*)
   extra: {}
-  metric_name: students
+  metric_name: count
   metric_type: null
-  verbose_name: Students
+  verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_learner_problem_summary.sql' %}{% endfilter %}
-table_name: fact_learner_problem_summary
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_learner_problem_course_summary.sql' %}{% endfilter %}
+table_name: fact_learner_problem_course_summary
 template_params: null
-uuid: 9362354c-1541-43c2-b769-da9818236298
+uuid: 981f30d9-b2f0-4a0b-9e95-0ee0e06db806
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 _file_name: fact_pageview_engagement.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: section/subsection page engagement
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: null
 - advanced_data_type: null
   column_name: section/subsection name
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: null
 - advanced_data_type: null
   column_name: content level
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: null
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: null
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: null
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: null
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,118 +1,106 @@
-_file_name: fact_problem_grades.yaml
+_file_name: fact_video_watches.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: actor_id
+  column_name: video_name_with_location
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor Id
+  verbose_name: Video Name With Location
 - advanced_data_type: null
-  column_name: grade_bucket
+  column_name: watched_segment_count
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Grade Bucket
+  type: Int32
+  verbose_name: Watched Segment Count
 - advanced_data_type: null
-  column_name: course_key
+  column_name: watched_entire_video
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Course Key
+  type: Boolean
+  verbose_name: Watched Entire Video
 - advanced_data_type: null
-  column_name: course_name
+  column_name: actor_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Name
+  verbose_name: Actor ID
 - advanced_data_type: null
-  column_name: course_run
+  column_name: course_key
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Run
-- advanced_data_type: null
-  column_name: emission_time
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: true
-  python_date_format: null
-  type: DateTime
-  verbose_name: Emission Time
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: entity_name
+  column_name: course_name
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Entity Name
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: scaled_score
+  column_name: course_run
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Float
-  verbose_name: Scaled Score
+  type: String
+  verbose_name: Course Run
 - advanced_data_type: null
-  column_name: grade_type
+  column_name: video_name
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Grade Type
+  verbose_name: Video Name
 - advanced_data_type: null
   column_name: org
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
@@ -128,23 +116,42 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
+  expression: count(*) - count(distinct actor_id)
+  extra: {}
+  metric_name: repeat_views
+  metric_type: null
+  verbose_name: Repeat Views
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
   expression: count(*)
+  extra:
+    warning_markdown: ''
+  metric_name: count
+  metric_type: null
+  verbose_name: Total Views
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: count(distinct actor_id)
   extra: {}
-  metric_name: students
+  metric_name: unique_viewers
   metric_type: null
-  verbose_name: Students
+  verbose_name: Unique Viewers
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_problem_grades.sql' %}{% endfilter %}
-table_name: fact_problem_grades
-template_params: {}
-uuid: b31154e0-afed-4445-b90d-a501d555784e
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_video_watches.sql' %}{% endfilter %}
+table_name: fact_video_watches
+template_params: null
+uuid: d0070c9a-5b1c-4e52-867b-79aa46a8cdcf
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,150 +1,125 @@
-_file_name: fact_problem_responses.yaml
+_file_name: query_log.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: problem_name_with_location
+  column_name: event_time
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Problem Name With Location
-- advanced_data_type: null
-  column_name: actor_id
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Actor ID
-- advanced_data_type: null
-  column_name: course_name
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: String
-  verbose_name: Course Name
+  type: DateTime
+  verbose_name: Event Time
 - advanced_data_type: null
-  column_name: course_run
+  column_name: query
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Run
+  verbose_name: Query
 - advanced_data_type: null
-  column_name: emission_time
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: true
-  python_date_format: null
-  type: DateTime
-  verbose_name: Emission Time
-- advanced_data_type: null
-  column_name: problem_name
+  column_name: tables
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Problem Name
+  type: Array(LowCardinality(String))
+  verbose_name: null
 - advanced_data_type: null
-  column_name: attempts
+  column_name: http_user_agent
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Int16
-  verbose_name: Attempts
+  type: LowCardinality(String)
+  verbose_name: null
 - advanced_data_type: null
-  column_name: success
+  column_name: memory_usage_mb
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Bool
-  verbose_name: Success
+  type: Float64
+  verbose_name: null
 - advanced_data_type: null
-  column_name: org
+  column_name: query_duration_ms
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Organization
+  type: UInt64
+  verbose_name: null
 - advanced_data_type: null
-  column_name: responses
+  column_name: result_rows
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Responses
+  type: UInt64
+  verbose_name: null
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
-extra: {}
+extra: null
 fetch_values_predicate: null
-filter_select_enabled: false
+filter_select_enabled: true
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*)
-  extra: {}
-  metric_name: total_responses
-  metric_type: null
-  verbose_name: Responses
+  expression: COUNT(*)
+  extra:
+    warning_markdown: ''
+  metric_name: count
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: true
+normalize_columns: false
 offset: 0
 params: null
 schema: main
-sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_problem_responses.sql' %}{% endfilter %}
-table_name: fact_problem_responses
+sql: |
+  SELECT
+      query_duration_ms,
+      result_rows,
+      memory_usage / (1024 * 1024 ) AS memory_usage_mb,
+      event_time,
+      tables,
+      query,
+      http_user_agent
+  FROM system.query_log
+  WHERE (has(databases, '{{ASPECTS_XAPI_DATABASE}}') OR has(databases, '{{ASPECTS_EVENT_SINK_DATABASE}}') OR has(databases, '{{DBT_PROFILE_TARGET_DATABASE}}')) AND (http_user_agent LIKE 'aspects-%') AND (type = 'QueryFinish')
+  ORDER BY event_time DESC
+table_name: query_log
 template_params: null
-uuid: 511dd5f1-3925-4e9e-ad8a-a227b5680047
+uuid: 53099fd2-6739-45e5-9a93-fcb9fa70119f
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,98 +1,87 @@
-_file_name: fact_transcript_usage.yaml
+_file_name: dim_course_problems.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: video_name_with_location
+  column_name: problem_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Name With Location
-- advanced_data_type: null
-  column_name: actor_id
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Actor ID
+  verbose_name: Problem Name With Location
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: emission_time
+  column_name: problem_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: DateTime
-  verbose_name: Emission Time
+  type: String
+  verbose_name: Problem Id
 - advanced_data_type: null
-  column_name: video_name
+  column_name: problem_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Name
+  verbose_name: Problem Name
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -104,34 +93,23 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(distinct actor_id)
-  extra:
-    warning_markdown: ''
-  metric_name: unique_transcript_users
-  metric_type: null
-  verbose_name: Unique Transcript Users
-  warning_text: null
-- currency: null
-  d3format: null
-  description: null
   expression: count(*)
-  extra:
-    warning_markdown: ''
-  metric_name: total_transcript_usage
+  extra: {}
+  metric_name: count
   metric_type: null
-  verbose_name: Total transcript usage
+  verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_transcript_usage.sql' %}{% endfilter %}
-table_name: fact_transcript_usage
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/dim_course_problems.sql' %}{% endfilter %}
+table_name: dim_course_problems
 template_params: {}
-uuid: a96a4b13-a429-442d-83ca-5d6f94010909
+uuid: 008e2907-fc6b-45ef-bf85-73a04c5791ff
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 _file_name: fact_video_engagement.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: section/subsection page engagement
   description: null
   expression: null
   extra: null
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,99 @@
-_file_name: fact_video_plays.yaml
+_file_name: hints_per_success.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: video_name_with_location
+  column_name: problem_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Name With Location
+  verbose_name: Problem Name With Location
+- advanced_data_type: null
+  column_name: total_hints
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: UInt64
+  verbose_name: Total Hints
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Actor ID
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: emission_time
+  column_name: problem_name
   description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: true
-  python_date_format: null
-  type: DateTime
-  verbose_name: Emission Time
-- advanced_data_type: null
-  column_name: video_name
-  description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Name
+  verbose_name: Problem Name
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -104,34 +105,32 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(distinct actor_id)
-  extra:
-    warning_markdown: ''
-  metric_name: unique_watchers
-  metric_type: null
-  verbose_name: Unique Watchers
+  expression: COUNT(*)
+  extra: null
+  metric_name: count
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
 - currency: null
   d3format: null
   description: null
   expression: count(*)
-  extra:
-    warning_markdown: ''
-  metric_name: total_plays
+  extra: {}
+  metric_name: students
   metric_type: null
-  verbose_name: Total plays
+  verbose_name: Students
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_video_plays.sql' %}{% endfilter %}
-table_name: fact_video_plays
-template_params: {}
-uuid: 6ec360a5-e247-42e7-b301-fa8275fc93f9
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/hints_per_success.sql' %}{% endfilter %}
+table_name: hints_per_success
+template_params: null
+uuid: a5db584d-c8dd-4acc-889e-074288c38433
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,157 +1,90 @@
-_file_name: fact_video_watches.yaml
+_file_name: slowest_clickhouse_queries.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: video_name_with_location
+  column_name: memory_usage_kb
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Video Name With Location
-- advanced_data_type: null
-  column_name: watched_segment_count
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: Int32
-  verbose_name: Watched Segment Count
-- advanced_data_type: null
-  column_name: watched_entire_video
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: Boolean
-  verbose_name: Watched Entire Video
-- advanced_data_type: null
-  column_name: actor_id
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Actor ID
-- advanced_data_type: null
-  column_name: course_key
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Course Key
+  type: Float64
+  verbose_name: Memory Usage (KB)
 - advanced_data_type: null
-  column_name: course_name
+  column_name: duration_secs
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Course Name
+  type: Float64
+  verbose_name: Duration (Seconds)
 - advanced_data_type: null
-  column_name: course_run
+  column_name: read_rows
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Course Run
+  type: UInt64
+  verbose_name: Read Rows
 - advanced_data_type: null
-  column_name: video_name
+  column_name: event_time
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: String
-  verbose_name: Video Name
+  type: DateTime
+  verbose_name: Event Time
 - advanced_data_type: null
-  column_name: org
+  column_name: query
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Organization
+  verbose_name: Query
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
-filter_select_enabled: false
-main_dttm_col: null
+filter_select_enabled: true
+main_dttm_col: event_time
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*) - count(distinct actor_id)
+  expression: COUNT(*)
   extra: {}
-  metric_name: repeat_views
-  metric_type: null
-  verbose_name: Repeat Views
-  warning_text: null
-- currency: null
-  d3format: null
-  description: null
-  expression: count(*)
-  extra:
-    warning_markdown: ''
   metric_name: count
-  metric_type: null
-  verbose_name: Total Views
-  warning_text: null
-- currency: null
-  d3format: null
-  description: null
-  expression: count(distinct actor_id)
-  extra: {}
-  metric_name: unique_viewers
-  metric_type: null
-  verbose_name: Unique Viewers
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: true
+normalize_columns: false
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_video_watches.sql' %}{% endfilter %}
-table_name: fact_video_watches
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/slowest_clickhouse_queries.sql' %}{% endfilter %}
+table_name: slowest_clickhouse_queries
 template_params: null
-uuid: d0070c9a-5b1c-4e52-867b-79aa46a8cdcf
+uuid: e8748c23-6220-413d-bd61-de8306163e10
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,157 +1,172 @@
-_file_name: fact_watched_video_segments.yaml
+_file_name: fact_problem_grades.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: video_name_with_location
+  column_name: entity_name_with_location
   description: null
-  expression: null
+  expression: ''
+  extra: null
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: Nullable(String)
+  verbose_name: Entity Name With Location
+- advanced_data_type: null
+  column_name: grade_type
+  description: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Video Name With Location
+  type: Nullable(String)
+  verbose_name: Grade Type
 - advanced_data_type: null
-  column_name: segment_start
+  column_name: scaled_score
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Int32
-  verbose_name: Segment Start
+  type: Float64
+  verbose_name: Scaled Score
 - advanced_data_type: null
   column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor ID
+  verbose_name: Actor Id
 - advanced_data_type: null
-  column_name: started_at
+  column_name: grade_bucket
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: DateTime
-  verbose_name: Started At
+  type: String
+  verbose_name: Grade Bucket
 - advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: video_name
+  column_name: emission_time
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: true
+  python_date_format: null
+  type: DateTime
+  verbose_name: Emission Time
+- advanced_data_type: null
+  column_name: entity_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Name
+  verbose_name: Entity Name
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*) - count(distinct actor_id)
-  extra: {}
-  metric_name: repeat_views
-  metric_type: null
-  verbose_name: Repeat Views
-  warning_text: null
-- currency: null
-  d3format: null
-  description: null
-  expression: count(*)
-  extra:
-    warning_markdown: ''
+  expression: COUNT(*)
+  extra: null
   metric_name: count
-  metric_type: null
-  verbose_name: Total Views
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
 - currency: null
   d3format: null
   description: null
-  expression: count(distinct actor_id)
+  expression: count(*)
   extra: {}
-  metric_name: unique_viewers
+  metric_name: students
   metric_type: null
-  verbose_name: Unique Viewers
+  verbose_name: Students
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_watched_video_segments.sql' %}{% endfilter %}
-table_name: fact_watched_video_segments
-template_params: null
-uuid: c2c391b3-3403-4f05-bc0b-3de53bd366ec
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_problem_grades.sql' %}{% endfilter %}
+table_name: fact_problem_grades
+template_params: {}
+uuid: b31154e0-afed-4445-b90d-a501d555784e
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,126 +1,127 @@
-_file_name: hints_per_success.yaml
+_file_name: fact_enrollments_by_day.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: problem_name_with_location
+  column_name: enrollment_status_date
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: String
-  verbose_name: Problem Name With Location
+  type: Date
+  verbose_name: Enrollment Status Date
 - advanced_data_type: null
-  column_name: total_hints
+  column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: UInt64
-  verbose_name: Total Hints
+  type: String
+  verbose_name: Actor Id
 - advanced_data_type: null
-  column_name: actor_id
+  column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor ID
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: course_key
+  column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Key
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: course_name
+  column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Name
+  verbose_name: Course Run
 - advanced_data_type: null
-  column_name: course_run
+  column_name: enrollment_mode
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Run
+  verbose_name: Enrollment Mode
 - advanced_data_type: null
-  column_name: problem_name
+  column_name: enrollment_status
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Name
+  verbose_name: Enrollment Status
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: enrollment_status_date
 metrics:
 - currency: null
   d3format: null
   description: null
   expression: count(*)
   extra: {}
-  metric_name: students
+  metric_name: count
   metric_type: null
-  verbose_name: Students
+  verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/hints_per_success.sql' %}{% endfilter %}
-table_name: hints_per_success
-template_params: null
-uuid: a5db584d-c8dd-4acc-889e-074288c38433
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_enrollments_by_day.sql' %}{% endfilter %}
+table_name: fact_enrollments_by_day
+template_params: {}
+uuid: 352311fe-12f0-470c-8b8c-d4f6a3936b3d
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,138 +1,184 @@
-_file_name: indexed_events.yaml
+_file_name: fact_problem_responses.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: actor_id
+  column_name: problem_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor ID
+  verbose_name: Problem Name With Location
 - advanced_data_type: null
-  column_name: course_key
+  column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Key
+  verbose_name: Actor ID
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: event_id
+  column_name: emission_time
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: UUID
-  verbose_name: Event ID
+  type: DateTime
+  verbose_name: Emission Time
 - advanced_data_type: null
-  column_name: emission_time
+  column_name: problem_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: DateTime
-  verbose_name: Emission Time
+  type: String
+  verbose_name: Problem Name
 - advanced_data_type: null
-  column_name: object_id
+  column_name: course_key
   description: null
-  expression: null
-  extra: {}
+  expression: ''
+  extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Object ID
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: verb_id
+  column_name: problem_id
   description: null
-  expression: null
-  extra: {}
+  expression: ''
+  extra: null
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Verb ID
+  verbose_name: Problem ID
+- advanced_data_type: null
+  column_name: attempts
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: Int16
+  verbose_name: Attempts
+- advanced_data_type: null
+  column_name: success
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: Bool
+  verbose_name: Success
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Organization
+- advanced_data_type: null
+  column_name: responses
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: String
+  verbose_name: Responses
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
-filter_select_enabled: true
+filter_select_enabled: false
 main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
   expression: COUNT(*)
-  extra: {}
+  extra: null
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: false
+- currency: null
+  d3format: null
+  description: null
+  expression: count(*)
+  extra: {}
+  metric_name: total_responses
+  metric_type: null
+  verbose_name: Responses
+  warning_text: null
+normalize_columns: true
 offset: 0
 params: null
 schema: main
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/indexed_events.sql' %}{% endfilter %}
-table_name: indexed_events
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_problem_responses.sql' %}{% endfilter %}
+table_name: fact_problem_responses
 template_params: null
-uuid: d6b1402a-393b-4595-9fbc-86aa9beacae9
+uuid: 511dd5f1-3925-4e9e-ad8a-a227b5680047
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,51 @@
-_file_name: posts_per_user.yaml
+_file_name: course_names.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: num_posts
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: UInt64
-  verbose_name: Number of Posts
-- advanced_data_type: null
-  column_name: actor_id
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Actor ID
-- advanced_data_type: null
   column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Key
 - advanced_data_type: null
   column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Name
 - advanced_data_type: null
   column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -80,23 +57,22 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*)
+  expression: COUNT(*)
   extra: {}
-  metric_name: users
-  metric_type: null
-  verbose_name: Number Of Users
+  metric_name: count
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
-sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/posts_per_user.sql' %}{% endfilter %}
-table_name: posts_per_user
-template_params: {}
-uuid: a2823d2e-54c4-4378-98c2-817f000c14ab
+sql: select * from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_names
+table_name: course_names
+template_params: null
+uuid: 41278a97-d0ff-4645-9514-d79f80d275df
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,147 @@
-_file_name: query_log.yaml
+_file_name: fact_transcript_usage.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: event_time
+  column_name: video_name_with_location
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: DateTime
-  verbose_name: Event Time
+  type: String
+  verbose_name: Video Name With Location
 - advanced_data_type: null
-  column_name: query
+  column_name: actor_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Query
+  verbose_name: Actor ID
 - advanced_data_type: null
-  column_name: tables
+  column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Array(LowCardinality(String))
-  verbose_name: null
+  type: String
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: http_user_agent
+  column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: LowCardinality(String)
-  verbose_name: null
+  type: String
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: memory_usage_mb
+  column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Float64
-  verbose_name: null
+  type: String
+  verbose_name: Course Run
+- advanced_data_type: null
+  column_name: emission_time
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: true
+  python_date_format: null
+  type: DateTime
+  verbose_name: Emission Time
 - advanced_data_type: null
-  column_name: query_duration_ms
+  column_name: video_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: UInt64
-  verbose_name: null
+  type: String
+  verbose_name: Video Name
 - advanced_data_type: null
-  column_name: result_rows
+  column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: UInt64
-  verbose_name: null
+  type: String
+  verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
-extra: null
+extra: {}
 fetch_values_predicate: null
-filter_select_enabled: true
-main_dttm_col: null
+filter_select_enabled: false
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: COUNT(*)
+  expression: count(distinct actor_id)
   extra:
     warning_markdown: ''
+  metric_name: unique_transcript_users
+  metric_type: null
+  verbose_name: Unique Transcript Users
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: count(*)
+  extra:
+    warning_markdown: ''
+  metric_name: total_transcript_usage
+  metric_type: null
+  verbose_name: Total transcript usage
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: COUNT(*)
+  extra: null
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: false
+normalize_columns: true
 offset: 0
 params: null
 schema: main
-sql: |
-  SELECT
-      query_duration_ms,
-      result_rows,
-      memory_usage / (1024 * 1024 ) AS memory_usage_mb,
-      event_time,
-      tables,
-      query,
-      http_user_agent
-  FROM system.query_log
-  WHERE (has(databases, '{{ASPECTS_XAPI_DATABASE}}') OR has(databases, '{{ASPECTS_EVENT_SINK_DATABASE}}') OR has(databases, '{{DBT_PROFILE_TARGET_DATABASE}}')) AND (http_user_agent LIKE 'aspects-%') AND (type = 'QueryFinish')
-  ORDER BY event_time DESC
-table_name: query_log
-template_params: null
-uuid: 53099fd2-6739-45e5-9a93-fcb9fa70119f
+sql: |-
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_transcript_usage.sql' %}{% endfilter %}
+table_name: fact_transcript_usage
+template_params: {}
+uuid: a96a4b13-a429-442d-83ca-5d6f94010909
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,199 @@
-_file_name: slowest_clickhouse_queries.yaml
+_file_name: superset_action_log.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: memory_usage_kb
+  column_name: user_registration_date
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: true
+  python_date_format: null
+  type: DATETIME
+  verbose_name: User Registration Date
+- advanced_data_type: null
+  column_name: action_date
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: true
+  python_date_format: null
+  type: DATETIME
+  verbose_name: Action Date
+- advanced_data_type: null
+  column_name: action_count
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Float64
-  verbose_name: Memory Usage (KB)
+  type: INT
+  verbose_name: Action Count
 - advanced_data_type: null
-  column_name: duration_secs
+  column_name: dashboard_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Float64
-  verbose_name: Duration (Seconds)
+  type: INT
+  verbose_name: Dashboard ID
 - advanced_data_type: null
-  column_name: read_rows
+  column_name: dashboard_status
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: UInt64
-  verbose_name: Read Rows
+  type: STRING
+  verbose_name: Dashboard Status
 - advanced_data_type: null
-  column_name: event_time
+  column_name: dashboard_title
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: DateTime
-  verbose_name: Event Time
+  type: STRING
+  verbose_name: Dashboard Title
 - advanced_data_type: null
-  column_name: query
+  column_name: slice_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Query
-database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
+  type: INT
+  verbose_name: Slice ID
+- advanced_data_type: null
+  column_name: user_id
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: INT
+  verbose_name: User ID
+- advanced_data_type: null
+  column_name: user_name
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: STRING
+  verbose_name: User Name
+- advanced_data_type: null
+  column_name: datasource_id
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: null
+  verbose_name: Datasource ID
+- advanced_data_type: null
+  column_name: datasource_name
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: null
+  python_date_format: null
+  type: null
+  verbose_name: Datasource Name
+- advanced_data_type: null
+  column_name: datasource_type
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: null
+  python_date_format: null
+  type: null
+  verbose_name: Datasource Type
+- advanced_data_type: null
+  column_name: slice_name
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: null
+  python_date_format: null
+  type: null
+  verbose_name: Slice Name
+- advanced_data_type: null
+  column_name: action
+  description: null
+  expression: null
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: STRING
+  verbose_name: Action
+database_uuid: 06cd566f-e22a-4a79-b0e0-4c947de93ee0
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
-filter_select_enabled: true
-main_dttm_col: event_time
+filter_select_enabled: false
+main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: COUNT(*)
-  extra: {}
+  expression: count(*)
+  extra:
+    warning_markdown: ''
   metric_name: count
-  metric_type: count
-  verbose_name: COUNT(*)
+  metric_type: null
+  verbose_name: null
   warning_text: null
 normalize_columns: false
 offset: 0
 params: null
-schema: main
+schema: superset
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/slowest_clickhouse_queries.sql' %}{% endfilter %}
-table_name: slowest_clickhouse_queries
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/superset_action_log.sql' %}{% endfilter %}
+table_name: superset_action_log
 template_params: null
-uuid: e8748c23-6220-413d-bd61-de8306163e10
+uuid: c33517b3-daa5-4fac-b7f2-ae012b999d12
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,199 +1,191 @@
-_file_name: superset_action_log.yaml
+_file_name: xapi_events_all_parsed.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: user_registration_date
-  description: null
-  expression: null
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: true
-  python_date_format: null
-  type: DATETIME
-  verbose_name: User Registration Date
-- advanced_data_type: null
-  column_name: action_date
-  description: null
-  expression: null
+  column_name: video_event
+  description: Set to true when the event is a video event.
+  expression: |-
+    verb_id LIKE '%video%'
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: true
+  is_dttm: false
   python_date_format: null
-  type: DATETIME
-  verbose_name: Action Date
+  type: null
+  verbose_name: Video Event
 - advanced_data_type: null
-  column_name: action_count
-  description: null
-  expression: null
+  column_name: verb
+  description: Short name for the verb; the final word in the verb_id path.
+  expression: |-
+    splitByChar('/', verb_id)[-1]
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: INT
-  verbose_name: Action Count
+  type: null
+  verbose_name: Verb
 - advanced_data_type: null
-  column_name: dashboard_id
-  description: null
-  expression: null
+  column_name: course_key_short
+  description: 'Course key without the course-v1: prefix'
+  expression: |-
+    splitByChar(':', splitByChar('/', course_id)[-1])[-1]
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: INT
-  verbose_name: Dashboard ID
+  type: null
+  verbose_name: Course Key Short
 - advanced_data_type: null
-  column_name: dashboard_status
-  description: null
-  expression: null
+  column_name: object_type
+  description: 'Parsed JSON: last word in the event.object.definition.type field'
+  expression: |-
+    splitByChar('/', event.object.definition.type)[-1]
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: STRING
-  verbose_name: Dashboard Status
+  type: null
+  verbose_name: Object Type
 - advanced_data_type: null
-  column_name: dashboard_title
-  description: null
-  expression: null
+  column_name: course_key
+  description: Course key part of the course_id URL
+  expression: |-
+    splitByChar('/', course_id)[-1]
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: STRING
-  verbose_name: Dashboard Title
+  type: null
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: slice_id
+  column_name: actor_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: INT
-  verbose_name: Slice ID
+  type: String
+  verbose_name: Actor ID
 - advanced_data_type: null
-  column_name: user_id
+  column_name: course_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: INT
-  verbose_name: User ID
+  type: String
+  verbose_name: Course ID
 - advanced_data_type: null
-  column_name: user_name
+  column_name: event_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: STRING
-  verbose_name: User Name
+  type: UUID
+  verbose_name: Event ID
 - advanced_data_type: null
-  column_name: datasource_id
+  column_name: emission_time
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: null
-  verbose_name: Datasource ID
+  type: DateTime
+  verbose_name: Emission Time
 - advanced_data_type: null
-  column_name: datasource_name
+  column_name: object_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
-  is_active: true
-  is_dttm: null
+  is_active: null
+  is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Datasource Name
+  type: String
+  verbose_name: Object ID
 - advanced_data_type: null
-  column_name: datasource_type
+  column_name: verb_id
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: null
+  is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Datasource Type
+  type: String
+  verbose_name: Verb ID
 - advanced_data_type: null
-  column_name: slice_name
+  column_name: event_str
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: null
+  is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Slice Name
+  type: String
+  verbose_name: Event String
 - advanced_data_type: null
-  column_name: action
+  column_name: org
   description: null
   expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: STRING
-  verbose_name: Action
-database_uuid: 06cd566f-e22a-4a79-b0e0-4c947de93ee0
+  type: String
+  verbose_name: Organization
+database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: null
+main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
-  expression: count(*)
+  expression: COUNT(*)
   extra:
     warning_markdown: ''
   metric_name: count
-  metric_type: null
-  verbose_name: null
+  metric_type: count
+  verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: false
+normalize_columns: true
 offset: 0
 params: null
 schema: main
-sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/superset_action_log.sql' %}{% endfilter %}
-table_name: superset_action_log
+sql: SELECT * FROM {{ASPECTS_XAPI_DATABASE}}.xapi_events_all_parsed
+table_name: xapi_events_all_parsed
 template_params: null
-uuid: c33517b3-daa5-4fac-b7f2-ae012b999d12
+uuid: 2a2498dc-03ce-41a0-b798-d84f808f7da6
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,159 @@
-_file_name: xapi_events_all_parsed.yaml
+_file_name: fact_video_plays.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: video_event
-  description: Set to true when the event is a video event.
-  expression: |-
-    verb_id LIKE '%video%'
+  column_name: video_name_with_location
+  description: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Video Event
+  type: String
+  verbose_name: Video Name With Location
 - advanced_data_type: null
-  column_name: verb
-  description: Short name for the verb; the final word in the verb_id path.
-  expression: |-
-    splitByChar('/', verb_id)[-1]
+  column_name: video_position
+  description: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Verb
+  type: Decimal(9, 2)
+  verbose_name: Video Position
 - advanced_data_type: null
-  column_name: course_key_short
-  description: 'Course key without the course-v1: prefix'
-  expression: |-
-    splitByChar(':', splitByChar('/', course_id)[-1])[-1]
+  column_name: video_duration
+  description: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Course Key Short
+  type: Int64
+  verbose_name: Video Duration
 - advanced_data_type: null
-  column_name: object_type
-  description: 'Parsed JSON: last word in the event.object.definition.type field'
-  expression: |-
-    splitByChar('/', event.object.definition.type)[-1]
+  column_name: actor_id
+  description: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Object Type
+  type: String
+  verbose_name: Actor ID
 - advanced_data_type: null
-  column_name: course_key
-  description: Course key part of the course_id URL
-  expression: |-
-    splitByChar('/', course_id)[-1]
+  column_name: visualization_bucket
+  description: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: null
-  verbose_name: Course Key
+  type: String
+  verbose_name: Visualization Bucket
 - advanced_data_type: null
-  column_name: actor_id
+  column_name: course_key
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Actor ID
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: course_id
+  column_name: course_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course ID
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: event_id
+  column_name: course_run
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: UUID
-  verbose_name: Event ID
+  type: String
+  verbose_name: Course Run
 - advanced_data_type: null
   column_name: emission_time
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: true
   python_date_format: null
   type: DateTime
   verbose_name: Emission Time
 - advanced_data_type: null
-  column_name: object_id
+  column_name: video_id
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
-  is_active: null
+  is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Object ID
+  verbose_name: Video ID
 - advanced_data_type: null
-  column_name: verb_id
+  column_name: video_name
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Verb ID
+  verbose_name: Video Name
 - advanced_data_type: null
-  column_name: event_str
+  column_name: graded
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Event String
+  type: Bool
+  verbose_name: Graded
 - advanced_data_type: null
   column_name: org
   description: null
-  expression: null
+  expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
@@ -169,23 +165,44 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: emission_time
 metrics:
 - currency: null
   d3format: null
   description: null
+  expression: count(distinct actor_id)
+  extra:
+    warning_markdown: ''
+  metric_name: unique_watchers
+  metric_type: null
+  verbose_name: Unique Watchers
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
+  expression: count(*)
+  extra:
+    warning_markdown: ''
+  metric_name: total_plays
+  metric_type: null
+  verbose_name: Total plays
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
   expression: COUNT(*)
   extra:
     warning_markdown: ''
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
 schema: main
-sql: SELECT * FROM {{ASPECTS_XAPI_DATABASE}}.xapi_events_all_parsed
-table_name: xapi_events_all_parsed
-template_params: null
-uuid: 2a2498dc-03ce-41a0-b798-d84f808f7da6
+sql: |-
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_video_plays.sql' %}{% endfilter %}
+table_name: fact_video_plays
+template_params: {}
+uuid: 6ec360a5-e247-42e7-b301-fa8275fc93f9
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql`

 * *Files 3% similar despite different names*

```diff
@@ -82,18 +82,18 @@
         success,
         attempts,
         0 AS num_hints_displayed,
         0 AS num_answers_displayed
     FROM int_problem_results
     WHERE 1=1
     {% raw %}
-    {% if from_dttm is not none %}
+    {% if from_dttm %}
     and emission_time > '{{ from_dttm }}'
     {% endif %}
-    {% if to_dttm is not none %}
+    {% if to_dttm %}
     and emission_time < '{{ to_dttm }}'
     {% endif %}
     {% endraw %}
     UNION ALL
     SELECT
         org,
         course_key,
@@ -105,18 +105,18 @@
         NULL AS success,
         NULL AS attempts,
         caseWithExpression(help_type, 'hint', 1, 0) AS num_hints_displayed,
         caseWithExpression(help_type, 'answer', 1, 0) AS num_answers_displayed
     FROM {{ DBT_PROFILE_TARGET_DATABASE }}.int_problem_hints
     WHERE 1=1
     {% raw %}
-    {% if from_dttm is not none %}
+    {% if from_dttm %}
     and emission_time > '{{ from_dttm }}'
     {% endif %}
-    {% if to_dttm is not none %}
+    {% if to_dttm %}
     and emission_time < '{{ to_dttm }}'
     {% endif %}
     {% endraw %}
     {% include 'openedx-assets/queries/common_filters.sql' %}
 )
 
 SELECT
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
                 then 'All pages viewed'
                 else 'At least one page viewed'
             end as engagement_level
         from {{ DBT_PROFILE_TARGET_DATABASE }}.fact_navigation_completion
         where
             1 = 1
             {% raw %}
-            {% if from_dttm is not none %}
+            {% if from_dttm %}
                 and visited_on > date('{{ from_dttm }}')
             {% endif %}
-            {% if to_dttm is not none %}
+            {% if to_dttm %}
                 and visited_on < date('{{ to_dttm }}')
             {% endif %}
             {% endraw %}
             {% include 'openedx-assets/queries/common_filters.sql' %}
         group by
             org,
             course_key,
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
                 then 'All problems attempted'
                 else 'At least one problem attempted'
             end as engagement_level
         from {{ DBT_PROFILE_TARGET_DATABASE }}.fact_problem_engagement
         where
             1 = 1
             {% raw %}
-            {% if from_dttm is not none %}
+            {% if from_dttm %}
                 and attempted_on > date('{{ from_dttm }}')
             {% endif %}
-            {% if to_dttm is not none %}
+            {% if to_dttm %}
                 and attempted_on < date('{{ to_dttm }}')
             {% endif %}
             {% endraw %}
             {% include 'openedx-assets/queries/common_filters.sql' %}
         group by
             org,
             course_key,
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
                 then 'All videos viewed'
                 else 'At least one video viewed'
             end as engagement_level
         from {{ DBT_PROFILE_TARGET_DATABASE }}.fact_video_engagement
         where
             1 = 1
             {% raw %}
-            {% if from_dttm is not none %}
+            {% if from_dttm %}
                 and viewed_on > date('{{ from_dttm }}')
             {% endif %}
-            {% if to_dttm is not none %}
+            {% if to_dttm %}
                 and viewed_on < date('{{ to_dttm }}')
             {% endif %}
             {% endraw %}
             {% include 'openedx-assets/queries/common_filters.sql' %}
         group by
             org,
             course_key,
```

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/indexed_events.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.95.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql` & `tutor-contrib-aspects-0.96.0/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql`

 * *Files identical despite different names*

