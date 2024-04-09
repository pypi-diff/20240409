# Comparing `tmp/tutor-contrib-aspects-0.96.1.tar.gz` & `tmp/tutor-contrib-aspects-0.96.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.96.1.tar", last modified: Tue Apr  9 17:16:51 2024, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.96.2.tar", last modified: Tue Apr  9 17:23:50 2024, max compression
```

## Comparing `tutor-contrib-aspects-0.96.1.tar` & `tutor-contrib-aspects-0.96.2.tar`

### file list

```diff
@@ -1,277 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.208344 tutor-contrib-aspects-0.96.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 17:16:51.204344 tutor-contrib-aspects-0.96.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.164344 tutor-contrib-aspects-0.96.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 17:16:51.208344 tutor-contrib-aspects-0.96.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.204344 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 17:16:51.000000 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-09 17:16:51.000000 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:16:51.000000 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 17:16:51.000000 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 17:16:51.000000 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 17:16:51.000000 tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.168344 tutor-contrib-aspects-0.96.1/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/asset_command_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/commands_v0.py
--rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/commands_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.172344 tutor-contrib-aspects-0.96.1/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/clickhouse-extra-sql
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/clickhouse-server-config
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/clickhouse-user-config
--rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/openedx-common-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/openedx-development-settings
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/superset-extra-asset-translations
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/superset-extra-roles
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/superset-row-level-security
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/superset-sso-assignment-rules
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/patches/xapi-db-load-config-yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.172344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.164344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.172344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.160344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.172344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.172344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.172344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.176344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.176344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.160344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/users/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.160344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/env
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/conf/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/security/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.180344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/security/partials/
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
--rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.184344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.184344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.184344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.184344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.184344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.184344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/localization/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.164344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.164344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.192344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.192344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.196344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.164344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/lms/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.200344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/superset/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/base-docker-compose-services
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.164344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:16:51.204344 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/common_filters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 17:16:46.000000 tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.815600 tutor-contrib-aspects-0.96.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 17:23:50.815600 tutor-contrib-aspects-0.96.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.775599 tutor-contrib-aspects-0.96.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 17:23:50.815600 tutor-contrib-aspects-0.96.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.815600 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-09 17:23:50.000000 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-09 17:23:50.000000 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:23:50.000000 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 17:23:50.000000 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 17:23:50.000000 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 17:23:50.000000 tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.775599 tutor-contrib-aspects-0.96.2/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12852 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/asset_command_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/commands_v0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9922 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/commands_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.779599 tutor-contrib-aspects-0.96.2/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/clickhouse-extra-sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/clickhouse-server-config
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/clickhouse-user-config
+-rw-r--r--   0 runner    (1001) docker     (127)    18341 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/openedx-common-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/openedx-dev-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/openedx-development-settings
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/superset-extra-asset-translations
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/superset-extra-roles
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/superset-row-level-security
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/superset-sso-assignment-rules
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/patches/xapi-db-load-config-yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27978 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.783599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.783599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.783599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.783599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.783599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/scripts/xapi-db-load-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/dev_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/dev_config/server_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/clickhouse/users/user_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/env
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      537 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.787599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/conf/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/scripts/import-assets.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/security/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76456 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.791599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.795599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.795599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/localization/datasets_strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   373791 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.803599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.803599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27120 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.803599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/OpenedX_Clickhouse.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/databases/Superset_Metadata.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.771599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/lms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql-post-migration.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.811599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/superset/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2779 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.775599 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:23:50.815600 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/common_filters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_forum_interactions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/hints_per_success.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/indexed_events.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/int_problem_responses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/posts_per_user.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/slowest_clickhouse_queries.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 17:23:45.000000 tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql
```

### Comparing `tutor-contrib-aspects-0.96.1/LICENSE` & `tutor-contrib-aspects-0.96.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/PKG-INFO` & `tutor-contrib-aspects-0.96.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.96.1
+Version: 0.96.2
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.96.1/README.rst` & `tutor-contrib-aspects-0.96.2/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/setup.py` & `tutor-contrib-aspects-0.96.2/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.96.1
+Version: 0.96.2
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/openedx/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/openedx/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/openedx/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tutor-contrib-aspects-0.96.1/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.96.2/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/asset_command_helpers.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/asset_command_helpers.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/commands_v0.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/commands_v0.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/commands_v1.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/commands_v1.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/clickhouse-server-config` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/clickhouse-server-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/clickhouse-user-config` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/clickhouse-user-config`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/openedx-common-settings` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/openedx-common-settings`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/patches/xapi-db-load-config-yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/patches/xapi-db-load-config-yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0010_course_dictionaries.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0011_vector_replacingmergetree_xapi_raw.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0014_add_course_names_fields.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0015_add_course_key_blocks.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0016_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0017_add_graded_course_block_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0020_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0023_extend_display_names.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0026_event_sink_external_id.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0027_partition_event_sink_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0028_user_pii.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0029_drop_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0030_rename_vector_json_column.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0031_add_email_user_profile.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0032_partition_tables_by_year_and_month.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0033_ccx_function.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0034_load_test_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/logging.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/conf/README.md` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/conf/README.md`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/localization.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/security/partials/read_only_permissions.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/k8s.toml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/k8s.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/localization/locale.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Active_Users_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Actor_IDs_over_time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Chart_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Charts_by_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/ClickHouse_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Enrollments_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Course_Grade_Distribution.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Courses_Per_Organization.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Currently_Enrolled_Learners_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Dashboard_Count.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distinct_forum_users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Attempts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Hints_Per_Correct_Answer.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Problem_Grades.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Distribution_Of_Responses.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollment_Events_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Enrollment_Mode.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Enrollments_By_Type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Event_type.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Events_per_course.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_Received_Event.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Last_course_syncronized.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Charts.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most-used_Dashboards.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Most_Active_Courses_Per_Day.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Pageview_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Partial_and_full_views_per_video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Posts_per_user.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Problem_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Query_performance.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Responses_Per_Problem.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Slowest_ClickHouse_Queries.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Active_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Superset_Registered_Users_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Actors_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Total_Organizations.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Transcripts_Captions_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Unique_actors.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/User_Actions.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Video_engagement_by_section_subsection.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watched_Video_Segments.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/Watches_Per_Video.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/charts/xAPI_Events_Over_Time_v2.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Individual_Learner_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Instructor_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Learner_Groups_Reports.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/dashboards/Operator_Dashboard.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/ab_user.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -186,13 +186,13 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: false
 offset: 0
 params: null
-schema: superset
-sql: select * from superset.ab_user
+schema: {{ SUPERSET_DB_NAME }}
+sql: select * from ab_user
 table_name: ab_user
 template_params: null
 uuid: 304a5d6d-c589-483a-8e8d-3fadbccef648
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/clickhouse_computed_metrics.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_blocks.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -123,13 +123,13 @@
   extra: {}
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 offset: 0
 params: null
-schema: main
+schema: {{ASPECTS_EVENT_SINK_DATABASE}}
 sql: "select * from {{ASPECTS_EVENT_SINK_DATABASE}}.{{ ASPECTS_EVENT_SINK_NODES_TABLE }}"
 table_name: "{{ ASPECTS_EVENT_SINK_NODES_TABLE }}"
 template_params: null
 uuid: 1b73d066-fd6c-411d-a99d-fc585f9474b1
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_names.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -66,13 +66,13 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ASPECTS_EVENT_SINK_DATABASE}}
 sql: select * from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_names
 table_name: course_names
 template_params: null
 uuid: 41278a97-d0ff-4645-9514-d79f80d275df
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/course_overviews.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -173,13 +173,13 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ ASPECTS_EVENT_SINK_DATABASE }}
 sql: select * from {{ ASPECTS_EVENT_SINK_DATABASE }}.course_overviews
 table_name: course_overviews
 template_params: null
 uuid: 46183302-6fa6-41a3-b6a7-79ff6c1c8402
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dashboards.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -222,13 +222,13 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: superset
+schema: {{ SUPERSET_DB_NAME }}
 sql: 'select * from dashboards'
 table_name: dashboards
 template_params: null
 uuid: 3dee777a-3dd4-4fcb-a749-4d13651b3444
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-_file_name: dim_course_problems.yaml
+_file_name: dim_course_videos.yaml
 always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: problem_name_with_location
+  column_name: video_name_with_location
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Name With Location
+  verbose_name: Video Name With Location
 - advanced_data_type: null
   column_name: course_key
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
@@ -47,37 +47,37 @@
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: problem_id
+  column_name: video_id
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Id
+  verbose_name: Video Id
 - advanced_data_type: null
-  column_name: problem_name
+  column_name: video_name
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Problem Name
+  verbose_name: Video Name
 - advanced_data_type: null
   column_name: org
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
@@ -102,14 +102,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/dim_course_problems.sql' %}{% endfilter %}
-table_name: dim_course_problems
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/dim_course_videos.sql' %}{% endfilter %}
+table_name: dim_course_videos
 template_params: {}
-uuid: 008e2907-fc6b-45ef-bf85-73a04c5791ff
+uuid: 417b2035-8fa1-4c60-a405-4b1947c3c966
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_videos.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-_file_name: dim_course_videos.yaml
+_file_name: fact_watched_video_segments.yaml
 always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
   column_name: video_name_with_location
   description: null
   expression: ''
@@ -11,61 +11,85 @@
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Video Name With Location
 - advanced_data_type: null
-  column_name: course_key
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
+- advanced_data_type: null
+  column_name: actor_id
   description: null
   expression: ''
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
-  column_name: course_name
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
+- advanced_data_type: null
+  column_name: course_key
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Name
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: course_run
+  column_name: course_name
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Course Run
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: video_id
+  column_name: course_run
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Id
+  verbose_name: Course Run
 - advanced_data_type: null
   column_name: video_name
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
@@ -88,28 +112,47 @@
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
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/dim_course_videos.sql' %}{% endfilter %}
-table_name: dim_course_videos
-template_params: {}
-uuid: 417b2035-8fa1-4c60-a405-4b1947c3c966
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_watched_video_segments.sql' %}{% endfilter %}
+table_name: fact_watched_video_segments
+template_params: null
+uuid: c2c391b3-3403-4f05-bc0b-3de53bd366ec
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_course_grades.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,14 @@
   metric_name: students
   metric_type: null
   verbose_name: Students
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_course_grades.sql' %}{% endfilter %}
 table_name: fact_course_grades
 template_params: {}
 uuid: d777bd95-2110-46db-a1c4-8358be81a85a
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_enrollments.sql' %}{% endfilter %}
 table_name: fact_enrollments
 template_params: {}
 uuid: a234545d-08ff-480d-8361-961c3d15f14f
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_enrollments_by_day.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_enrollments_by_day.sql' %}{% endfilter %}
 table_name: fact_enrollments_by_day
 template_params: {}
 uuid: 352311fe-12f0-470c-8b8c-d4f6a3936b3d
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_forum_interactions.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_forum_interactions.sql' %}{% endfilter %}
 table_name: fact_forum_interactions
 template_params: {}
 uuid: 39d1e786-c0c8-4c56-81c8-56fb0df88001
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_course_summary.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_learner_problem_course_summary.sql' %}{% endfilter %}
 table_name: fact_learner_problem_course_summary
 template_params: null
 uuid: 981f30d9-b2f0-4a0b-9e95-0ee0e06db806
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_learner_problem_summary.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,14 @@
   metric_name: students
   metric_type: null
   verbose_name: Students
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_learner_problem_summary.sql' %}{% endfilter %}
 table_name: fact_learner_problem_summary
 template_params: null
 uuid: 9362354c-1541-43c2-b769-da9818236298
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_pageview_engagement.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_pageview_engagement.sql' %}{% endfilter %}
 table_name: fact_pageview_engagement
 template_params: {}
 uuid: 9febd6be-5102-4dbf-86b9-45ebd3cbbc45
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_engagement.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_grades.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -159,14 +159,14 @@
   metric_name: students
   metric_type: null
   verbose_name: Students
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_problem_grades.sql' %}{% endfilter %}
 table_name: fact_problem_grades
 template_params: {}
 uuid: b31154e0-afed-4445-b90d-a501d555784e
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_problem_responses.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,14 @@
   metric_name: total_responses
   metric_type: null
   verbose_name: Responses
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_problem_responses.sql' %}{% endfilter %}
 table_name: fact_problem_responses
 template_params: null
 uuid: 511dd5f1-3925-4e9e-ad8a-a227b5680047
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_transcript_usage.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,14 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_transcript_usage.sql' %}{% endfilter %}
 table_name: fact_transcript_usage
 template_params: {}
 uuid: a96a4b13-a429-442d-83ca-5d6f94010909
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_engagement.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_video_engagement.sql' %}{% endfilter %}
 table_name: fact_video_engagement
 template_params: {}
 uuid: 247a55b3-d44e-442e-ba92-71bf7976b192
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_plays.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,14 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_video_plays.sql' %}{% endfilter %}
 table_name: fact_video_plays
 template_params: {}
 uuid: 6ec360a5-e247-42e7-b301-fa8275fc93f9
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_video_watches.yaml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/fact_watched_video_segments.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,48 @@
-_file_name: fact_watched_video_segments.yaml
+_file_name: hints_per_success.yaml
 always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: video_name_with_location
+  column_name: problem_name_with_location
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
-  verbose_name: Video Name With Location
+  verbose_name: Problem Name With Location
 - advanced_data_type: null
-  column_name: segment_start
+  column_name: total_hints
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: Int64
-  verbose_name: Segment Start
+  type: UInt64
+  verbose_name: Total Hints
 - advanced_data_type: null
   column_name: actor_id
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Actor ID
 - advanced_data_type: null
-  column_name: started_at
-  description: null
-  expression: ''
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: true
-  python_date_format: null
-  type: DateTime
-  verbose_name: Started At
-- advanced_data_type: null
   column_name: course_key
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
@@ -83,25 +71,25 @@
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: video_name
+  column_name: problem_name
   description: null
   expression: ''
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
   expression: ''
   extra: {}
   filterable: true
   groupby: true
@@ -112,47 +100,37 @@
   verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
 default_endpoint: null
 description: null
 extra: {}
 fetch_values_predicate: null
 filter_select_enabled: false
-main_dttm_col: started_at
+main_dttm_col: null
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
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/fact_watched_video_segments.sql' %}{% endfilter %}
-table_name: fact_watched_video_segments
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/hints_per_success.sql' %}{% endfilter %}
+table_name: hints_per_success
 template_params: null
-uuid: c2c391b3-3403-4f05-bc0b-3de53bd366ec
+uuid: a5db584d-c8dd-4acc-889e-074288c38433
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/hints_per_success.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-_file_name: hints_per_success.yaml
+_file_name: posts_per_user.yaml
 always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: problem_name_with_location
-  description: null
-  expression: ''
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Problem Name With Location
-- advanced_data_type: null
-  column_name: total_hints
+  column_name: num_posts
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: UInt64
-  verbose_name: Total Hints
+  verbose_name: Number of Posts
 - advanced_data_type: null
   column_name: actor_id
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
@@ -71,26 +59,14 @@
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
   type: String
   verbose_name: Course Run
 - advanced_data_type: null
-  column_name: problem_name
-  description: null
-  expression: ''
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Problem Name
-- advanced_data_type: null
   column_name: org
   description: null
   expression: ''
   extra: {}
   filterable: true
   groupby: true
   is_active: true
@@ -105,32 +81,32 @@
 fetch_values_predicate: null
 filter_select_enabled: false
 main_dttm_col: null
 metrics:
 - currency: null
   d3format: null
   description: null
+  expression: count(*)
+  extra: {}
+  metric_name: users
+  metric_type: null
+  verbose_name: Number Of Users
+  warning_text: null
+- currency: null
+  d3format: null
+  description: null
   expression: COUNT(*)
   extra: null
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
-- currency: null
-  d3format: null
-  description: null
-  expression: count(*)
-  extra: {}
-  metric_name: students
-  metric_type: null
-  verbose_name: Students
-  warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/hints_per_success.sql' %}{% endfilter %}
-table_name: hints_per_success
-template_params: null
-uuid: a5db584d-c8dd-4acc-889e-074288c38433
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/posts_per_user.sql' %}{% endfilter %}
+table_name: posts_per_user
+template_params: {}
+uuid: a2823d2e-54c4-4378-98c2-817f000c14ab
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/indexed_events.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,14 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: false
 offset: 0
 params: null
-schema: main
+schema: {{ ASPECTS_XAPI_DATABASE }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/indexed_events.sql' %}{% endfilter %}
 table_name: indexed_events
 template_params: null
 uuid: d6b1402a-393b-4595-9fbc-86aa9beacae9
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/posts_per_user.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,112 +1,90 @@
-_file_name: posts_per_user.yaml
-always_filter_main_dttm: false
+_file_name: slowest_clickhouse_queries.yaml
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: num_posts
+  column_name: memory_usage_kb
   description: null
-  expression: ''
+  expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: UInt64
-  verbose_name: Number of Posts
+  type: Float64
+  verbose_name: Memory Usage (KB)
 - advanced_data_type: null
-  column_name: actor_id
+  column_name: duration_secs
   description: null
-  expression: ''
+  expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Actor ID
-- advanced_data_type: null
-  column_name: course_key
-  description: null
-  expression: ''
-  extra: {}
-  filterable: true
-  groupby: true
-  is_active: true
-  is_dttm: false
-  python_date_format: null
-  type: String
-  verbose_name: Course Key
+  type: Float64
+  verbose_name: Duration (Seconds)
 - advanced_data_type: null
-  column_name: course_name
+  column_name: read_rows
   description: null
-  expression: ''
+  expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
   is_dttm: false
   python_date_format: null
-  type: String
-  verbose_name: Course Name
+  type: UInt64
+  verbose_name: Read Rows
 - advanced_data_type: null
-  column_name: course_run
+  column_name: event_time
   description: null
-  expression: ''
+  expression: null
   extra: {}
   filterable: true
   groupby: true
   is_active: true
-  is_dttm: false
+  is_dttm: true
   python_date_format: null
-  type: String
-  verbose_name: Course Run
+  type: DateTime
+  verbose_name: Event Time
 - advanced_data_type: null
-  column_name: org
+  column_name: query
   description: null
-  expression: ''
+  expression: null
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
-  expression: count(*)
-  extra: {}
-  metric_name: users
-  metric_type: null
-  verbose_name: Number Of Users
-  warning_text: null
-- currency: null
-  d3format: null
-  description: null
   expression: COUNT(*)
-  extra: null
+  extra: {}
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
-normalize_columns: true
+normalize_columns: false
 offset: 0
 params: null
-schema: main
+schema: system
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/posts_per_user.sql' %}{% endfilter %}
-table_name: posts_per_user
-template_params: {}
-uuid: a2823d2e-54c4-4378-98c2-817f000c14ab
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/slowest_clickhouse_queries.sql' %}{% endfilter %}
+table_name: slowest_clickhouse_queries
+template_params: null
+uuid: e8748c23-6220-413d-bd61-de8306163e10
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/query_log.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: false
 offset: 0
 params: null
-schema: main
+schema: system
 sql: |
   SELECT
       query_duration_ms,
       result_rows,
       memory_usage / (1024 * 1024 ) AS memory_usage_mb,
       event_time,
       tables,
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slices.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -269,13 +269,13 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: superset
-sql: select * from superset.slices
+schema: {{ SUPERSET_DB_NAME }}
+sql: select * from slices
 table_name: slices
 template_params: null
 uuid: aaf1ae12-73c1-4b88-b07d-7a8988333018
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/slowest_clickhouse_queries.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/dim_course_problems.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,115 @@
-_file_name: slowest_clickhouse_queries.yaml
+_file_name: dim_course_problems.yaml
+always_filter_main_dttm: false
 cache_timeout: null
 columns:
 - advanced_data_type: null
-  column_name: memory_usage_kb
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
-  type: Float64
-  verbose_name: Memory Usage (KB)
+  type: String
+  verbose_name: Problem Name With Location
 - advanced_data_type: null
-  column_name: duration_secs
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
-  type: Float64
-  verbose_name: Duration (Seconds)
+  type: String
+  verbose_name: Course Key
 - advanced_data_type: null
-  column_name: read_rows
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
-  type: UInt64
-  verbose_name: Read Rows
+  type: String
+  verbose_name: Course Name
 - advanced_data_type: null
-  column_name: event_time
+  column_name: course_run
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
+  verbose_name: Course Run
+- advanced_data_type: null
+  column_name: problem_id
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: String
+  verbose_name: Problem Id
+- advanced_data_type: null
+  column_name: problem_name
+  description: null
+  expression: ''
+  extra: {}
+  filterable: true
+  groupby: true
+  is_active: true
+  is_dttm: false
+  python_date_format: null
+  type: String
+  verbose_name: Problem Name
 - advanced_data_type: null
-  column_name: query
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
   type: String
-  verbose_name: Query
+  verbose_name: Organization
 database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
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
+  expression: count(*)
   extra: {}
   metric_name: count
-  metric_type: count
-  verbose_name: COUNT(*)
+  metric_type: null
+  verbose_name: null
   warning_text: null
-normalize_columns: false
+normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ DBT_PROFILE_TARGET_DATABASE }}
 sql: |-
-  {% filter indent(width=2) %}{% include 'openedx-assets/queries/slowest_clickhouse_queries.sql' %}{% endfilter %}
-table_name: slowest_clickhouse_queries
-template_params: null
-uuid: e8748c23-6220-413d-bd61-de8306163e10
+  {% filter indent(width=2) %}{% include 'openedx-assets/queries/dim_course_problems.sql' %}{% endfilter %}
+table_name: dim_course_problems
+template_params: {}
+uuid: 008e2907-fc6b-45ef-bf85-73a04c5791ff
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/superset_action_log.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,14 @@
   metric_name: count
   metric_type: null
   verbose_name: null
   warning_text: null
 normalize_columns: false
 offset: 0
 params: null
-schema: superset
+schema: {{ SUPERSET_DB_NAME }}
 sql: |-
   {% filter indent(width=2) %}{% include 'openedx-assets/queries/superset_action_log.sql' %}{% endfilter %}
 table_name: superset_action_log
 template_params: null
 uuid: c33517b3-daa5-4fac-b7f2-ae012b999d12
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/user_pii.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 _file_name: user_pii.yaml
 table_name: user_pii
 main_dttm_col: null
 description: null
 default_endpoint: null
 offset: 0
 cache_timeout: null
-schema: main
-sql: 'select * from event_sink.user_pii'
+schema: {{ ASPECTS_EVENT_SINK_DATABASE }}
+sql: 'select * from {{ ASPECTS_EVENT_SINK_DATABASE }}.user_pii'
 params: null
 template_params: null
 filter_select_enabled: true
 fetch_values_predicate: null
 extra: {}
 normalize_columns: false
 uuid: 5f3d28a1-ebb4-4e4a-95ea-2930623d774d
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/build/aspects-superset/openedx-assets/assets/datasets/xapi_events_all_parsed.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -179,13 +179,13 @@
   metric_name: count
   metric_type: count
   verbose_name: COUNT(*)
   warning_text: null
 normalize_columns: true
 offset: 0
 params: null
-schema: main
+schema: {{ ASPECTS_XAPI_DATABASE }}
 sql: SELECT * FROM {{ASPECTS_XAPI_DATABASE}}.xapi_events_all_parsed
 table_name: xapi_events_all_parsed
 template_params: null
 uuid: 2a2498dc-03ce-41a0-b798-d84f808f7da6
 version: 1.0.0
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/clickhouse/deduplicate.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/lms/init-lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/mysql/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/dim_course_problems.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_course_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_enrollments_by_day.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_course_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_learner_problem_summary.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_pageview_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_problem_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_problem_grades.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_problem_responses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_video_engagement.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_video_watches.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/fact_watched_video_segments.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/indexed_events.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/indexed_events.sql`

 * *Files 18% similar despite different names*

```diff
@@ -18,10 +18,10 @@
   object_id,
   events.course_key,
   events.org,
   events.verb_id,
   emission_time
 FROM events
 JOIN
-   event_sink.course_names courses
+   {{ ASPECTS_EVENT_SINK_DATABASE }}.course_names courses
 ON
   (events.course_key = courses.course_key)
```

### Comparing `tutor-contrib-aspects-0.96.1/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql` & `tutor-contrib-aspects-0.96.2/tutoraspects/templates/openedx-assets/queries/superset_action_log.sql`

 * *Files identical despite different names*

