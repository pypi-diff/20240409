# Comparing `tmp/pypigeon-0.2.6.tar.gz` & `tmp/pypigeon-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypigeon-0.2.6.tar", last modified: Mon Mar 11 17:02:26 2024, max compression
+gzip compressed data, was "pypigeon-0.2.8.tar", last modified: Tue Apr  9 11:38:27 2024, max compression
```

## Comparing `pypigeon-0.2.6.tar` & `pypigeon-0.2.8.tar`

### file list

```diff
@@ -1,352 +1,384 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.747470 pypigeon-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.691469 pypigeon-0.2.6/.openapi-python-client/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-11 17:01:23.000000 pypigeon-0.2.6/.openapi-python-client/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.695469 pypigeon-0.2.6/.openapi-python-client/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-11 17:01:23.000000 pypigeon-0.2.6/.openapi-python-client/templates/endpoint_init.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-03-11 17:01:23.000000 pypigeon-0.2.6/.openapi-python-client/templates/endpoint_macros.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-03-11 17:01:23.000000 pypigeon-0.2.6/.openapi-python-client/templates/endpoint_module.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-03-11 17:01:23.000000 pypigeon-0.2.6/.openapi-python-client/templates/model.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-11 17:01:23.000000 pypigeon-0.2.6/.openapi-python-client/templates/types.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-11 17:02:26.747470 pypigeon-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-11 17:01:23.000000 pypigeon-0.2.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2364 2024-03-11 17:01:23.000000 pypigeon-0.2.6/autogenerate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.695469 pypigeon-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.699469 pypigeon-0.2.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.699469 pypigeon-0.2.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.699469 pypigeon-0.2.6/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/pcmd_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/pigeon_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-03-11 17:01:23.000000 pypigeon-0.2.6/docs/source/pypigeon_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.699469 pypigeon-0.2.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-11 17:01:23.000000 pypigeon-0.2.6/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (127)   222200 2024-03-11 17:01:23.000000 pypigeon-0.2.6/examples/pigeon-example-1.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   121655 2024-03-11 17:01:23.000000 pypigeon-0.2.6/examples/pigeon-example-2.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.703469 pypigeon-0.2.6/pypigeon/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    13347 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/item_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.707469 pypigeon-0.2.6/pypigeon/pcmd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.707469 pypigeon-0.2.6/pypigeon/pcmd/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/commands/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/commands/base_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/commands/cde.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pcmd/commands/pdd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.707469 pypigeon-0.2.6/pypigeon/pigeon_core/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/.opcignore
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.707469 pypigeon-0.2.6/pypigeon/pigeon_core/api/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.707469 pypigeon-0.2.6/pypigeon/pigeon_core/api/account/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/account/account_create_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/account/account_delete_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/account/account_get_account.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.707469 pypigeon-0.2.6/pypigeon/pigeon_core/api/admin/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/admin/admin_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/admin/admin_put_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.711469 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_activate_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_authenticate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_get_csrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_get_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_new_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_provider_authorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_provider_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_provider_signin_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_providers_req.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_signin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_signout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.711469 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_delete_cdeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_get_cdeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_list_cdesets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_list_data_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_new_cdeset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.711469 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_create_collection_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_delete_collection_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_cde_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_collection_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_update_collection_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_update_collection_metapatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.715469 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/cdes_get_data_element_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/cdes_get_data_element_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_copy_to_cdeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_ref_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_element_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_dictionaries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.715469 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_inbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members_pending.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_outbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_process_inbox_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.715469 pypigeon-0.2.6/pypigeon/pigeon_core/api/general/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/general/root_get_datastores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.715469 pypigeon-0.2.6/pypigeon/pigeon_core/api/group/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_create_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_delete_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_get_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.719469 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_copy_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_create_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_delete_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_get_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_get_item_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_get_item_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_list_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_put_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_put_item_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.719469 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_get_collection_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_get_dictionary_search_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item_inverse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.719469 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_get_table_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_list_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_preview_table_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.723469 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_create_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_delete_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_outbox_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user_apc_inbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user_apc_liked.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user_apc_outbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_receive_in_user_inbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_send_to_user_outbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.747470 pypigeon-0.2.6/pypigeon/pigeon_core/models/
--rw-r--r--   0 runner    (1001) docker     (127)    19944 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/account_create_account_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_activate_session_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_authenticate_user_authentication_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_authenticate_user_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_get_csrf_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_get_session_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_provider_authorized_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_provider_login_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_provider_signin_provider_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_provider_signin_provider_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_providers_req_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/cdes_list_data_elements_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/cdes_new_cdeset_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/cdeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/cdeset_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_cde_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_cde_stats_item_distrib_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_cde_stats_per_cde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_stats_item_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_stats_item_stats_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_copy_to_cdeset_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_create_a_new_data_element_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_create_a_new_data_element_data_element_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_create_new_data_element_version_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_create_new_data_element_version_data_element_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_list_data_element_refs_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_list_data_elements_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_list_dictionaries_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_get_collection_apc_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_get_collections_collection_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_copy_item_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_list_items_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_put_item_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_put_item_body_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_put_item_body_content_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_element_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_error_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_list_tables_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_preview_table_data_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_dictionary_source_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_concept.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_concept_applies_to.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_definition_definition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference_external_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_number_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_number_range_number_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_text_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_text_range_text_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_value_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_value_set_value_set_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/datastore_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options_options_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options_options_additional_property_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_address_or_object_type_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_collection_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_collection_page_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/group_create_group_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/group_get_groups_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/group_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_column_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_parser_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status_detail_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_storage_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/item_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection_version_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/new_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/oauth_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/parser_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/parser_options_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/parser_options_additional_property_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/root_get_datastores_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_collections_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_collections_response_hits_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_collections_response_hits_item_items_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits_search_dictionaries_hit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_inverse_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_inverse_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_inverse_result_queries_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_get_collection_terms_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_get_dictionary_search_options_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_collections_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_collections_body_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_body_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_body_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_inverse_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_inverse_body_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/server_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/session_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/session_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_0_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_1_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_2_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_cache_cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_0_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_1_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_workers_backend_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data_data_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/table_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/termset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/termset_additional_property_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/update_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/update_collection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/user_get_users_response_200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/user_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/models/user_membership_role_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pypigeon/pigeon_core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.747470 pypigeon-0.2.6/pypigeon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-03-11 17:02:26.000000 pypigeon-0.2.6/pypigeon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18751 2024-03-11 17:02:26.000000 pypigeon-0.2.6/pypigeon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 17:02:26.000000 pypigeon-0.2.6/pypigeon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-11 17:02:26.000000 pypigeon-0.2.6/pypigeon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-11 17:02:26.000000 pypigeon-0.2.6/pypigeon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 17:02:26.000000 pypigeon-0.2.6/pypigeon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-11 17:01:23.000000 pypigeon-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 17:02:26.747470 pypigeon-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.747470 pypigeon-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-11 17:01:23.000000 pypigeon-0.2.6/tests/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-03-11 17:01:23.000000 pypigeon-0.2.6/tests/collections_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-11 17:01:23.000000 pypigeon-0.2.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:02:26.747470 pypigeon-0.2.6/tests/pigeon_core/
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-03-11 17:01:23.000000 pypigeon-0.2.6/tests/pigeon_core/login_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-11 17:01:23.000000 pypigeon-0.2.6/tests/pigeon_core/paginator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.448609 pypigeon-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.388610 pypigeon-0.2.8/.openapi-python-client/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 11:37:37.000000 pypigeon-0.2.8/.openapi-python-client/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.388610 pypigeon-0.2.8/.openapi-python-client/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 11:37:37.000000 pypigeon-0.2.8/.openapi-python-client/templates/endpoint_init.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-09 11:37:37.000000 pypigeon-0.2.8/.openapi-python-client/templates/endpoint_macros.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-09 11:37:37.000000 pypigeon-0.2.8/.openapi-python-client/templates/endpoint_module.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-09 11:37:37.000000 pypigeon-0.2.8/.openapi-python-client/templates/model.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 11:37:37.000000 pypigeon-0.2.8/.openapi-python-client/templates/types.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-09 11:38:27.448609 pypigeon-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 11:37:37.000000 pypigeon-0.2.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2921 2024-04-09 11:37:37.000000 pypigeon-0.2.8/autogenerate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.388610 pypigeon-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.388610 pypigeon-0.2.8/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.388610 pypigeon-0.2.8/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.388610 pypigeon-0.2.8/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/pcmd_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/pigeon_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-09 11:37:37.000000 pypigeon-0.2.8/docs/source/pypigeon_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.392610 pypigeon-0.2.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 11:37:37.000000 pypigeon-0.2.8/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)   222200 2024-04-09 11:37:37.000000 pypigeon-0.2.8/examples/pigeon-example-1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   121655 2024-04-09 11:37:37.000000 pypigeon-0.2.8/examples/pigeon-example-2.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.392610 pypigeon-0.2.8/pypigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19180 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13347 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/item_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.392610 pypigeon-0.2.8/pypigeon/pcmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.392610 pypigeon-0.2.8/pypigeon/pcmd/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/base_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/cde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/pdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pcmd/commands/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.396610 pypigeon-0.2.8/pypigeon/pigeon_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/.opcignore
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.396610 pypigeon-0.2.8/pypigeon/pigeon_core/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.396610 pypigeon-0.2.8/pypigeon/pigeon_core/api/account/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/account/account_create_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/account/account_delete_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/account/account_get_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.396610 pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/admin_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/admin_grant_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/admin_list_admins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/admin_put_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.400610 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_activate_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_authenticate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_get_csrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_get_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_new_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_provider_authorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_provider_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_provider_signin_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_providers_req.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_signout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.400610 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_delete_cdeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_get_data_element_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_get_data_element_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_get_ordered_cdeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_list_cdesets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_list_data_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_new_cdeset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.400610 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_create_collection_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_delete_collection_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_cde_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_collection_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_update_collection_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_update_collection_metapatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.404610 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_copy_to_cdeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_ref_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_element_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_new_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_set_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_update_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.408609 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_inbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members_pending.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_outbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_process_inbox_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.408609 pypigeon-0.2.8/pypigeon/pigeon_core/api/general/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/general/parsers_get_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/general/parsers_resolve_prql_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/general/root_get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/general/root_resolve_data_element_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.408609 pypigeon-0.2.8/pypigeon/pigeon_core/api/group/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_create_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_delete_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_get_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.412610 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_copy_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_create_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_delete_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_get_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_get_item_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_get_item_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_list_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_put_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_put_item_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.412610 pypigeon-0.2.8/pypigeon/pigeon_core/api/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/metadata/metadata_get_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/metadata/metadata_set_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.412610 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_get_collection_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_get_dictionary_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item_inverse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.412610 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_get_table_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_list_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6652 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_preview_table_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.416610 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_create_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_delete_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_outbox_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user_apc_inbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user_apc_liked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user_apc_outbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_receive_in_user_inbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_send_to_user_outbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.444609 pypigeon-0.2.8/pypigeon/pigeon_core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    20189 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/account_create_account_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/admin_grant_admin_admin_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/admin_grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/admin_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/admin_operations_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_activate_session_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_authenticate_user_authentication_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_authenticate_user_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_get_csrf_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_get_session_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_provider_authorized_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_provider_login_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_provider_signin_provider_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_provider_signin_provider_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_providers_req_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_signout_no_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/bundle_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/cdes_list_data_elements_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/cdes_new_cdeset_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/cdeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/cdeset_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_cde_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_cde_stats_item_distrib_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_cde_stats_per_cde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_stats_item_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_stats_item_stats_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_copy_to_cdeset_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_bundles_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_data_element_refs_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_data_elements_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_dictionaries_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_get_collection_apc_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_get_collections_collection_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_copy_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_list_items_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_put_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_put_item_body_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_put_item_body_content_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_element_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_error_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_list_tables_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_preview_table_data_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/column_schema_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_dictionary_source_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_concept.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_concept_applies_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_definition_definition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference_external_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_number_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_number_range_number_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_text_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_text_range_text_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_value_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_value_set_value_set_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/datastore_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options_options_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options_options_additional_property_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_address_or_object_type_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_collection_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_collection_page_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/group_create_group_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/group_get_groups_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/group_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_column_enum_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_parser_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status_detail_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_storage_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/item_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/metadata_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/metadata_fields_data_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection_version_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_data_element_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/new_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/oauth_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/parser_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/parser_options_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/parser_options_additional_property_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/parsers_get_parsers_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/parsers_resolve_prql_modules_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/preferred_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/prql_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/root_get_datastores_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_collections_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_collections_response_hits_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_collections_response_hits_item_items_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits_search_dictionaries_hit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_inverse_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_inverse_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_inverse_result_queries_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_get_collection_terms_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_get_dictionary_search_options_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_collections_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_collections_body_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_body_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_body_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_inverse_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_inverse_body_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/server_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/session_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/session_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_0_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_1_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_2_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_cache_cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_0_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_1_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_workers_backend_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/termset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/termset_additional_property_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/update_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/update_collection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/user_get_users_response_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/models/user_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pypigeon/pigeon_core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.448609 pypigeon-0.2.8/pypigeon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-09 11:38:27.000000 pypigeon-0.2.8/pypigeon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20431 2024-04-09 11:38:27.000000 pypigeon-0.2.8/pypigeon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:38:27.000000 pypigeon-0.2.8/pypigeon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 11:38:27.000000 pypigeon-0.2.8/pypigeon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 11:38:27.000000 pypigeon-0.2.8/pypigeon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 11:38:27.000000 pypigeon-0.2.8/pypigeon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-09 11:37:37.000000 pypigeon-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:38:27.448609 pypigeon-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.444609 pypigeon-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 11:37:37.000000 pypigeon-0.2.8/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-04-09 11:37:37.000000 pypigeon-0.2.8/tests/collections_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 11:37:37.000000 pypigeon-0.2.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:38:27.444609 pypigeon-0.2.8/tests/pigeon_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-09 11:37:37.000000 pypigeon-0.2.8/tests/pigeon_core/login_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 11:37:37.000000 pypigeon-0.2.8/tests/pigeon_core/paginator_test.py
```

### Comparing `pypigeon-0.2.6/.openapi-python-client/templates/endpoint_macros.py.jinja` & `pypigeon-0.2.8/.openapi-python-client/templates/endpoint_macros.py.jinja`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/.openapi-python-client/templates/endpoint_module.py.jinja` & `pypigeon-0.2.8/.openapi-python-client/templates/endpoint_module.py.jinja`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/.openapi-python-client/templates/model.py.jinja` & `pypigeon-0.2.8/.openapi-python-client/templates/model.py.jinja`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/.openapi-python-client/templates/types.py.jinja` & `pypigeon-0.2.8/.openapi-python-client/templates/types.py.jinja`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/PKG-INFO` & `pypigeon-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pypigeon
-Version: 0.2.6
+Version: 0.2.8
 Summary: an easy-to-use Python client for Pigeon
 Author-email: BioTeam <contact@bioteam.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: httpx<0.26.0,>=0.20.0
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: python-dateutil
 Requires-Dist: pyarrow
 Requires-Dist: pandas
 Requires-Dist: tqdm
+Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-httpx<0.26.0,>=0.20.0; extra == "dev"
 Requires-Dist: openapi-python-client==0.17.2; extra == "dev"
 Requires-Dist: reorder-python-imports; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black==23.12.1; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: types-tqdm; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-tabulate; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 
 # PyPigeon
```

### Comparing `pypigeon-0.2.6/README.md` & `pypigeon-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/Makefile` & `pypigeon-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/make.bat` & `pypigeon-0.2.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/source/_templates/custom-module-template.rst` & `pypigeon-0.2.8/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/source/conf.py` & `pypigeon-0.2.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/source/index.rst` & `pypigeon-0.2.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/source/pcmd_cli.rst` & `pypigeon-0.2.8/docs/source/pcmd_cli.rst`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/source/pigeon_core.rst` & `pypigeon-0.2.8/docs/source/pigeon_core.rst`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/docs/source/pypigeon_api.rst` & `pypigeon-0.2.8/docs/source/pypigeon_api.rst`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/examples/example.py` & `pypigeon-0.2.8/examples/example.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/examples/pigeon-example-1.ipynb` & `pypigeon-0.2.8/examples/pigeon-example-1.ipynb`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/examples/pigeon-example-2.ipynb` & `pypigeon-0.2.8/examples/pigeon-example-2.ipynb`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/client.py` & `pypigeon-0.2.8/pypigeon/client.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/collections.py` & `pypigeon-0.2.8/pypigeon/collections.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/item_io.py` & `pypigeon-0.2.8/pypigeon/item_io.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pcmd/cli.py` & `pypigeon-0.2.8/pypigeon/pcmd/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import argparse
+import json
 import os.path
 import sys
 from getpass import getpass
 from typing import Optional
 from urllib.parse import urlparse
 
 from pypigeon.client import login as interactive_login
 from pypigeon.client import make_base_url
 from pypigeon.client import PigeonClient
 from pypigeon.pigeon_core import Client as CoreClient
+from pypigeon.pigeon_core.errors import UnexpectedStatus
 from pypigeon.pigeon_core.login import Login
 from pypigeon.pigeon_core.login import LoginError
 from pypigeon.pigeon_core.login import to_token_file
 from pypigeon.pigeon_core.login import token_file_get_base_url
 
 from .commands import Commands
 
@@ -67,16 +69,16 @@
         "--username",
         metavar="USERNAME",
         help="disable interactive login; log in with USERNAME",
     )
     argparser.add_argument(
         "-O",
         "--output-type",
-        default="yaml",
-        choices=["yaml", "json"],
+        default="auto",
+        choices=["auto", "yaml", "json", "table"],
         help="set output type",
     )
     Commands._add_to_parser(argparser.add_subparsers(title="commands", required=True))
 
     args = argparser.parse_args()
 
     token_file = os.path.expanduser(args.token_file)
@@ -92,11 +94,21 @@
         sys.exit(1)
 
     client = login(base_url, token_file, args.username)
     if token_file:
         to_token_file(client._client, token_file)
 
     if hasattr(args, "func"):
-        args.func(args.cls(client, args))
+        try:
+            args.func(args.cls(client, args))
+        except UnexpectedStatus as ex:
+            print(str(ex))
+            try:
+                parsed = json.loads(ex.content)
+                print("error:", parsed["error"])
+                if parsed["detail"]:
+                    print("detail:", parsed["detail"])
+            except (json.JSONDecodeError, KeyError):
+                print(ex.content)
 
     else:
         argparser.print_usage()
```

### Comparing `pypigeon-0.2.6/pypigeon/pcmd/commands/auth.py` & `pypigeon-0.2.8/pypigeon/pcmd/commands/auth.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pcmd/commands/base_commands.py` & `pypigeon-0.2.8/pypigeon/pcmd/commands/base_commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,58 @@
 import argparse
 import json
+import sys
 import textwrap
 import types
 from typing import Any
 from typing import Callable
+from typing import Optional
 
 import yaml
 from pypigeon.client import PigeonClient
+from tabulate import tabulate
 
 
 class BaseCommands:
     _func_args: dict[Callable[..., None], list[tuple[tuple[Any, ...], dict[str, Any]]]]
 
     def __init__(self, client: PigeonClient, args: argparse.Namespace) -> None:
         self.client = client
         self.core = client._client
         self.args = args
 
-    def _output(self, data: Any) -> None:
-        if self.args.output_type == "yaml":
+    def _output(
+        self,
+        data: Any,
+        header: Optional[str] = None,
+        preferred_type: Optional[str] = None,
+    ) -> None:
+        output_type = self.args.output_type
+        if output_type == "auto":
+            output_type = preferred_type or "yaml"
+
+        if output_type == "yaml":
+            if header:
+                print("#", header)
             print(yaml.dump(data))
 
-        elif self.args.output_type == "json":
+        elif output_type == "json":
             print(json.dumps(data, indent=2))
 
+        elif output_type == "table":
+            try:
+                print(tabulate(data, headers="keys"))
+            except TypeError:
+                print(
+                    'This command does not support "table" output. Please choose'
+                    " another output format."
+                )
+                sys.exit(1)
         else:
-            raise ValueError(f"unknown output type: {self.args.output_type}")
+            raise ValueError(f"unknown output type: {output_type}")
 
     @classmethod
     def _add_to_parser(
         cls, subparsers: "argparse._SubParsersAction[argparse.ArgumentParser]"
     ) -> None:
         for method in dir(cls):
             if method.startswith("_"):
```

### Comparing `pypigeon-0.2.6/pypigeon/pcmd/commands/cde.py` & `pypigeon-0.2.8/pypigeon/pcmd/commands/cde.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pypigeon.pigeon_core.api.cde import cdes_delete_cdeset
-from pypigeon.pigeon_core.api.cde import cdes_get_cdeset
 from pypigeon.pigeon_core.api.cde import cdes_list_cdesets
 from pypigeon.pigeon_core.api.cde import cdes_new_cdeset
 from pypigeon.pigeon_core.api.data_dictionaries import (
     collections_dictionaries_copy_to_cdeset,
 )
 from pypigeon.pigeon_core.models import CdesNewCdesetBody
 from pypigeon.pigeon_core.models import CollectionsDictionariesCopyToCdesetBody
@@ -56,18 +55,23 @@
 
         Admin access is required, as well as access to the specified PDD.
 
         """
         if self.args.description:
             description = self.args.description
         else:
-            cdeset_info = cdes_get_cdeset.sync(
-                cdeset_name=self.args.cdeset_name, client=self.core
-            )
-            description = cdeset_info.description
+            description = ""
+            for cdeset in cdes_list_cdesets.sync(client=self.core).cdesets:
+                if cdeset.name == self.args.cdeset_name:
+                    description = cdeset.description
+
+            if not description:
+                raise ValueError(
+                    f"did not find existing CDE set: {self.args.cdeset_name}"
+                )
 
         collections_dictionaries_copy_to_cdeset.sync(
             collection_id=self.args.collection_id,
             version_id=self.args.version_id,
             item_id=self.args.item_id,
             body=CollectionsDictionariesCopyToCdesetBody(
                 name=self.args.cdeset_name,
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/account/account_create_account.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/account/account_create_account.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/account/account_delete_account.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/account/account_delete_account.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/account/account_get_account.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/account/account_get_account.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/admin/admin_get_config.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/admin_get_config.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/admin/admin_put_config.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/admin/admin_put_config.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_activate_session.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_activate_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: AuthenticatedClient,
     body: AuthActivateSessionBody,
 ) -> Response[Union[Any, ServerError]]:
     """Activate a placeholder session ID using the current session
 
     By providing an activation code, the related placeholder
     session will assume the identity of the current session.
 
@@ -97,15 +97,15 @@
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: AuthenticatedClient,
     body: AuthActivateSessionBody,
 ) -> Union[Any]:
     """Activate a placeholder session ID using the current session
 
     By providing an activation code, the related placeholder
     session will assume the identity of the current session.
 
@@ -131,15 +131,15 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: AuthenticatedClient,
     body: AuthActivateSessionBody,
 ) -> Response[Union[Any, ServerError]]:
     """Activate a placeholder session ID using the current session
 
     By providing an activation code, the related placeholder
     session will assume the identity of the current session.
 
@@ -164,15 +164,15 @@
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
+    client: AuthenticatedClient,
     body: AuthActivateSessionBody,
 ) -> Union[Any]:
     """Activate a placeholder session ID using the current session
 
     By providing an activation code, the related placeholder
     session will assume the identity of the current session.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_authenticate_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_authenticate_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Athenticates a local user."""
+"""Authenticates a local user."""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
@@ -66,15 +66,15 @@
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
     body: AuthAuthenticateUserAuthenticationRequest,
 ) -> Response[Union[AuthAuthenticateUserResponse200, ServerError]]:
-    """Athenticates a local user.
+    """Authenticates a local user.
 
     Args:
         body (AuthAuthenticateUserAuthenticationRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -95,15 +95,15 @@
 
 
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
     body: AuthAuthenticateUserAuthenticationRequest,
 ) -> Union[AuthAuthenticateUserResponse200]:
-    """Athenticates a local user.
+    """Authenticates a local user.
 
     Args:
         body (AuthAuthenticateUserAuthenticationRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -123,15 +123,15 @@
 
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
     body: AuthAuthenticateUserAuthenticationRequest,
 ) -> Response[Union[AuthAuthenticateUserResponse200, ServerError]]:
-    """Athenticates a local user.
+    """Authenticates a local user.
 
     Args:
         body (AuthAuthenticateUserAuthenticationRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -150,15 +150,15 @@
 
 
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
     body: AuthAuthenticateUserAuthenticationRequest,
 ) -> Union[AuthAuthenticateUserResponse200]:
-    """Athenticates a local user.
+    """Authenticates a local user.
 
     Args:
         body (AuthAuthenticateUserAuthenticationRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_get_csrf.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_get_csrf.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_get_session.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_get_session.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_new_session.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_new_session.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_provider_authorized.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_provider_authorized.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_provider_login.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_provider_login.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_provider_signin_provider.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_provider_signin_provider.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_providers_req.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_providers_req.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_signin.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_signin.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/auth/auth_signout.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_list_cdesets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,147 @@
-"""Displays the built-in/unbranded sign out page."""
+"""List available CDE sets"""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
+from ...models.cdeset_list import CdesetList
+from ...models.server_error import ServerError
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/auth/signout",
+        "method": "get",
+        "url": "/cde",
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Any:
-    if response.status_code == HTTPStatus.NO_CONTENT:
-        return None
+) -> Union[CdesetList, ServerError]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = CdesetList.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
+        response_500 = ServerError.from_dict(response.json())
+
+        return response_500
 
     raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Any]:
+) -> Response[Union[CdesetList, ServerError]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
-) -> Response[Any]:
-    """Displays the built-in/unbranded sign out page.
+) -> Response[Union[CdesetList, ServerError]]:
+    """List available CDE sets
+
+    TODO
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[Union[CdesetList, ServerError]]
     """
 
     kwargs = _get_kwargs()
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
+def sync(
+    *,
+    client: Union[AuthenticatedClient, Client],
+) -> Union[CdesetList]:
+    """List available CDE sets
+
+    TODO
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[CdesetList]
+    """
+
+    response = sync_detailed(
+        client=client,
+    )
+    if isinstance(response.parsed, ServerError):
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+
+    return response.parsed
+
+
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
-) -> Response[Any]:
-    """Displays the built-in/unbranded sign out page.
+) -> Response[Union[CdesetList, ServerError]]:
+    """List available CDE sets
+
+    TODO
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[Union[CdesetList, ServerError]]
     """
 
     kwargs = _get_kwargs()
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Union[AuthenticatedClient, Client],
+) -> Union[CdesetList]:
+    """List available CDE sets
+
+    TODO
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        Union[CdesetList]
+    """
+
+    response = await asyncio_detailed(
+        client=client,
+    )
+    if isinstance(response.parsed, ServerError):
+        raise errors.UnexpectedStatus(response.status_code, response.content)
+
+    return response.parsed
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_delete_cdeset.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_delete_cdeset.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_get_cdeset.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user_apc_inbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,173 @@
-"""Get a short summary of a CDE set"""
+"""Retrieve a user's inbox"""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
-from ...models.cdeset import Cdeset
+from ...models.federation_collection_page import FederationCollectionPage
 from ...models.server_error import ServerError
 from ...types import Response
 
 
 def _get_kwargs(
-    cdeset_name: str,
+    user_name: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/cde/{cdeset_name}".format(
-            cdeset_name=cdeset_name,
+        "url": "/user/{user_name}/inbox".format(
+            user_name=user_name,
         ),
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Union[Cdeset, ServerError]:
+) -> Union[FederationCollectionPage, ServerError]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Cdeset.from_dict(response.json())
+        response_200 = FederationCollectionPage.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = ServerError.from_dict(response.json())
+    if response.status_code == HTTPStatus.UNAUTHORIZED:
+        response_401 = ServerError.from_dict(response.json())
 
-        return response_404
+        return response_401
+    if response.status_code == HTTPStatus.FORBIDDEN:
+        response_403 = ServerError.from_dict(response.json())
+
+        return response_403
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = ServerError.from_dict(response.json())
 
         return response_500
 
     raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[Cdeset, ServerError]]:
+) -> Response[Union[FederationCollectionPage, ServerError]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    cdeset_name: str,
+    user_name: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[Cdeset, ServerError]]:
-    """Get a short summary of a CDE set
+    client: AuthenticatedClient,
+) -> Response[Union[FederationCollectionPage, ServerError]]:
+    """Retrieve a user's inbox
 
     Args:
-        cdeset_name (str):
+        user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Cdeset, ServerError]]
+        Response[Union[FederationCollectionPage, ServerError]]
     """
 
     kwargs = _get_kwargs(
-        cdeset_name=cdeset_name,
+        user_name=user_name,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    cdeset_name: str,
+    user_name: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Union[Cdeset]:
-    """Get a short summary of a CDE set
+    client: AuthenticatedClient,
+) -> Union[FederationCollectionPage]:
+    """Retrieve a user's inbox
 
     Args:
-        cdeset_name (str):
+        user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Cdeset]
+        Union[FederationCollectionPage]
     """
 
     response = sync_detailed(
-        cdeset_name=cdeset_name,
+        user_name=user_name,
         client=client,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
 
 
 async def asyncio_detailed(
-    cdeset_name: str,
+    user_name: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[Cdeset, ServerError]]:
-    """Get a short summary of a CDE set
+    client: AuthenticatedClient,
+) -> Response[Union[FederationCollectionPage, ServerError]]:
+    """Retrieve a user's inbox
 
     Args:
-        cdeset_name (str):
+        user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[Cdeset, ServerError]]
+        Response[Union[FederationCollectionPage, ServerError]]
     """
 
     kwargs = _get_kwargs(
-        cdeset_name=cdeset_name,
+        user_name=user_name,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    cdeset_name: str,
+    user_name: str,
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Union[Cdeset]:
-    """Get a short summary of a CDE set
+    client: AuthenticatedClient,
+) -> Union[FederationCollectionPage]:
+    """Retrieve a user's inbox
 
     Args:
-        cdeset_name (str):
+        user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[Cdeset]
+        Union[FederationCollectionPage]
     """
 
     response = await asyncio_detailed(
-        cdeset_name=cdeset_name,
+        user_name=user_name,
         client=client,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_list_cdesets.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/auth/auth_signout.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,145 +1,137 @@
-"""List available CDE sets"""
+"""Displays the built-in/unbranded sign out page."""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
-from ...models.cdeset_list import CdesetList
+from ...models.auth_signout_no_data import AuthSignoutNoData
 from ...models.server_error import ServerError
 from ...types import Response
 
 
 def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
-        "method": "get",
-        "url": "/cde",
+        "method": "post",
+        "url": "/auth/signout",
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Union[CdesetList, ServerError]:
+) -> Union[AuthSignoutNoData, ServerError]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = CdesetList.from_dict(response.json())
+        response_200 = AuthSignoutNoData.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = ServerError.from_dict(response.json())
 
         return response_500
 
     raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[CdesetList, ServerError]]:
+) -> Response[Union[AuthSignoutNoData, ServerError]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[CdesetList, ServerError]]:
-    """List available CDE sets
-
-    TODO
+    client: AuthenticatedClient,
+) -> Response[Union[AuthSignoutNoData, ServerError]]:
+    """Displays the built-in/unbranded sign out page.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[CdesetList, ServerError]]
+        Response[Union[AuthSignoutNoData, ServerError]]
     """
 
     kwargs = _get_kwargs()
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Union[CdesetList]:
-    """List available CDE sets
-
-    TODO
+    client: AuthenticatedClient,
+) -> Union[AuthSignoutNoData]:
+    """Displays the built-in/unbranded sign out page.
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[CdesetList]
+        Union[AuthSignoutNoData]
     """
 
     response = sync_detailed(
         client=client,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Response[Union[CdesetList, ServerError]]:
-    """List available CDE sets
-
-    TODO
+    client: AuthenticatedClient,
+) -> Response[Union[AuthSignoutNoData, ServerError]]:
+    """Displays the built-in/unbranded sign out page.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[CdesetList, ServerError]]
+        Response[Union[AuthSignoutNoData, ServerError]]
     """
 
     kwargs = _get_kwargs()
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
-    client: Union[AuthenticatedClient, Client],
-) -> Union[CdesetList]:
-    """List available CDE sets
-
-    TODO
+    client: AuthenticatedClient,
+) -> Union[AuthSignoutNoData]:
+    """Displays the built-in/unbranded sign out page.
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[CdesetList]
+        Union[AuthSignoutNoData]
     """
 
     response = await asyncio_detailed(
         client=client,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_list_data_elements.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_list_data_elements.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/cde/cdes_new_cdeset.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_new_cdeset.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_create_collection.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_create_collection.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_create_collection_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_create_collection_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_delete_collection_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_delete_collection_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_cde_stats.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_cde_stats.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_collection_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_collection_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_collections.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_collections.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_get_stats.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_get_stats.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_update_collection_meta.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_update_collection_meta.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/collections/collections_update_collection_metapatch.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/collections/collections_update_collection_metapatch.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/cdes_get_data_element_latest.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_get_data_element_latest.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/cdes_get_data_element_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/cde/cdes_get_data_element_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_copy_to_cdeset.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_copy_to_cdeset.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
-from ...models.collections_dictionaries_create_a_new_data_element_data_element import (
-    CollectionsDictionariesCreateANewDataElementDataElement,
-)
 from ...models.data_element import DataElement
+from ...models.new_data_element import NewDataElement
 from ...models.server_error import ServerError
 from ...types import Response
 
 
 def _get_kwargs(
     collection_id: str,
     version_id: str,
     item_id: str,
     *,
-    body: CollectionsDictionariesCreateANewDataElementDataElement,
+    body: NewDataElement,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "post",
         "url": "/collections/{collection_id}/{version_id}/dictionaries/{item_id}/elements".format(
             collection_id=collection_id,
@@ -92,25 +90,25 @@
 
 def sync_detailed(
     collection_id: str,
     version_id: str,
     item_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateANewDataElementDataElement,
+    body: NewDataElement,
 ) -> Response[Union[DataElement, ServerError]]:
     """Create a new data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
-        body (CollectionsDictionariesCreateANewDataElementDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[DataElement, ServerError]]
@@ -132,25 +130,25 @@
 
 def sync(
     collection_id: str,
     version_id: str,
     item_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateANewDataElementDataElement,
+    body: NewDataElement,
 ) -> Union[DataElement]:
     """Create a new data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
-        body (CollectionsDictionariesCreateANewDataElementDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[DataElement]
@@ -171,25 +169,25 @@
 
 async def asyncio_detailed(
     collection_id: str,
     version_id: str,
     item_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateANewDataElementDataElement,
+    body: NewDataElement,
 ) -> Response[Union[DataElement, ServerError]]:
     """Create a new data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
-        body (CollectionsDictionariesCreateANewDataElementDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[DataElement, ServerError]]
@@ -209,25 +207,25 @@
 
 async def asyncio(
     collection_id: str,
     version_id: str,
     item_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateANewDataElementDataElement,
+    body: NewDataElement,
 ) -> Union[DataElement]:
     """Create a new data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
-        body (CollectionsDictionariesCreateANewDataElementDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[DataElement]
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element_ref.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element_ref.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_ref_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_ref_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
-from ...models.collections_dictionaries_create_new_data_element_version_data_element import (
-    CollectionsDictionariesCreateNewDataElementVersionDataElement,
-)
 from ...models.data_element import DataElement
+from ...models.new_data_element import NewDataElement
 from ...models.server_error import ServerError
 from ...types import Response
 
 
 def _get_kwargs(
     collection_id: str,
     version_id: str,
     item_id: str,
     element_id: str,
     *,
-    body: CollectionsDictionariesCreateNewDataElementVersionDataElement,
+    body: NewDataElement,
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "put",
         "url": "/collections/{collection_id}/{version_id}/dictionaries/{item_id}/elements/{element_id}".format(
             collection_id=collection_id,
@@ -95,26 +93,26 @@
 def sync_detailed(
     collection_id: str,
     version_id: str,
     item_id: str,
     element_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateNewDataElementVersionDataElement,
+    body: NewDataElement,
 ) -> Response[Union[DataElement, ServerError]]:
     """Update a single data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
         element_id (str):
-        body (CollectionsDictionariesCreateNewDataElementVersionDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[DataElement, ServerError]]
@@ -138,26 +136,26 @@
 def sync(
     collection_id: str,
     version_id: str,
     item_id: str,
     element_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateNewDataElementVersionDataElement,
+    body: NewDataElement,
 ) -> Union[DataElement]:
     """Update a single data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
         element_id (str):
-        body (CollectionsDictionariesCreateNewDataElementVersionDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[DataElement]
@@ -180,26 +178,26 @@
 async def asyncio_detailed(
     collection_id: str,
     version_id: str,
     item_id: str,
     element_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateNewDataElementVersionDataElement,
+    body: NewDataElement,
 ) -> Response[Union[DataElement, ServerError]]:
     """Update a single data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
         element_id (str):
-        body (CollectionsDictionariesCreateNewDataElementVersionDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[DataElement, ServerError]]
@@ -221,26 +219,26 @@
 async def asyncio(
     collection_id: str,
     version_id: str,
     item_id: str,
     element_id: str,
     *,
     client: AuthenticatedClient,
-    body: CollectionsDictionariesCreateNewDataElementVersionDataElement,
+    body: NewDataElement,
 ) -> Union[DataElement]:
     """Update a single data element in a data dictionary
 
     TODO
 
     Args:
         collection_id (str):
         version_id (str):
         item_id (str):
         element_id (str):
-        body (CollectionsDictionariesCreateNewDataElementVersionDataElement): Pigeon Data Element
+        body (NewDataElement): Pigeon Data Element
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[DataElement]
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_data_element.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_data_element.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_latest.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_latest.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_latest.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_latest.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_element_refs.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_element_refs.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_elements.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_elements.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_dictionaries.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_inbox.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_inbox.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members_pending.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members_pending.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_outbox.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_get_collection_apc_outbox.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/federation/collections_process_inbox_message.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/federation/collections_process_inbox_message.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/general/root_get_datastores.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/general/root_get_datastores.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[RootGetDatastoresResponse200, ServerError]]:
     """List Datastores
 
-    List the datastores available for users to save files to, along with some useful metrics.
+    List the datastores available for users to save files to,
+    along with some useful metrics.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[RootGetDatastoresResponse200, ServerError]]
@@ -76,15 +77,16 @@
 
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Union[RootGetDatastoresResponse200]:
     """List Datastores
 
-    List the datastores available for users to save files to, along with some useful metrics.
+    List the datastores available for users to save files to,
+    along with some useful metrics.
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[RootGetDatastoresResponse200]
@@ -101,15 +103,16 @@
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[RootGetDatastoresResponse200, ServerError]]:
     """List Datastores
 
-    List the datastores available for users to save files to, along with some useful metrics.
+    List the datastores available for users to save files to,
+    along with some useful metrics.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[RootGetDatastoresResponse200, ServerError]]
@@ -124,15 +127,16 @@
 
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Union[RootGetDatastoresResponse200]:
     """List Datastores
 
-    List the datastores available for users to save files to, along with some useful metrics.
+    List the datastores available for users to save files to,
+    along with some useful metrics.
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[RootGetDatastoresResponse200]
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_create_group.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_create_group.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_delete_group.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_delete_group.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_get_group.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_get_group.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/group/group_get_groups.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/group/group_get_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     *,
     client: AuthenticatedClient,
     users: Union[Unset, bool] = UNSET,
 ) -> Response[Union[GroupGetGroupsResponse200, ServerError]]:
     """List groups
 
     List all the groups that are visible to the current user,
-    whether logged in or not.'
+    whether logged in or not.
 
     Args:
         users (Union[Unset, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -97,15 +97,15 @@
     *,
     client: AuthenticatedClient,
     users: Union[Unset, bool] = UNSET,
 ) -> Union[GroupGetGroupsResponse200]:
     """List groups
 
     List all the groups that are visible to the current user,
-    whether logged in or not.'
+    whether logged in or not.
 
     Args:
         users (Union[Unset, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -128,15 +128,15 @@
     *,
     client: AuthenticatedClient,
     users: Union[Unset, bool] = UNSET,
 ) -> Response[Union[GroupGetGroupsResponse200, ServerError]]:
     """List groups
 
     List all the groups that are visible to the current user,
-    whether logged in or not.'
+    whether logged in or not.
 
     Args:
         users (Union[Unset, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -158,15 +158,15 @@
     *,
     client: AuthenticatedClient,
     users: Union[Unset, bool] = UNSET,
 ) -> Union[GroupGetGroupsResponse200]:
     """List groups
 
     List all the groups that are visible to the current user,
-    whether logged in or not.'
+    whether logged in or not.
 
     Args:
         users (Union[Unset, bool]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_copy_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_copy_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_create_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_create_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_delete_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_delete_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_get_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_get_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_get_item_data.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_get_item_data.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_get_item_status.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_get_item_status.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_list_items.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_list_items.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_put_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_put_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/items/collections_items_put_item_data.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/items/collections_items_put_item_data.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_get_collection_terms.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_get_collection_terms.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_get_dictionary_search_options.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_get_dictionary_search_options.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_collections.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_collections.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_dictionaries.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item_inverse.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item_inverse.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data_elements.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_get_table_data_elements.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_get_table_info.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_get_table_info.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_list_tables.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_list_tables.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/tables/collections_tables_preview_table_data.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/tables/collections_tables_preview_table_data.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_create_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_create_user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_delete_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_delete_user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_outbox_activity.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_outbox_activity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""""""
+"""Retrieve a specific activity from the user's outbox"""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
@@ -65,15 +65,16 @@
 
 def sync_detailed(
     user_name: str,
     activity_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[Union[ServerError, User]]:
-    """
+    """Retrieve a specific activity from the user's outbox
+
     Args:
         user_name (str):
         activity_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -96,15 +97,16 @@
 
 def sync(
     user_name: str,
     activity_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Union[User]:
-    """
+    """Retrieve a specific activity from the user's outbox
+
     Args:
         user_name (str):
         activity_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -126,15 +128,16 @@
 
 async def asyncio_detailed(
     user_name: str,
     activity_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[Union[ServerError, User]]:
-    """
+    """Retrieve a specific activity from the user's outbox
+
     Args:
         user_name (str):
         activity_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -155,15 +158,16 @@
 
 async def asyncio(
     user_name: str,
     activity_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Union[User]:
-    """
+    """Retrieve a specific activity from the user's outbox
+
     Args:
         user_name (str):
         activity_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user_apc_inbox.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_user_apc_outbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""""""
+"""Read a user's outbox"""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
@@ -15,15 +15,15 @@
 
 
 def _get_kwargs(
     user_name: str,
 ) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/user/{user_name}/inbox".format(
+        "url": "/user/{user_name}/outbox".format(
             user_name=user_name,
         ),
     }
 
     return _kwargs
 
 
@@ -62,15 +62,16 @@
 
 
 def sync_detailed(
     user_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[Union[FederationCollectionPage, ServerError]]:
-    """
+    """Read a user's outbox
+
     Args:
         user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -90,15 +91,16 @@
 
 
 def sync(
     user_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Union[FederationCollectionPage]:
-    """
+    """Read a user's outbox
+
     Args:
         user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -117,15 +119,16 @@
 
 
 async def asyncio_detailed(
     user_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Response[Union[FederationCollectionPage, ServerError]]:
-    """
+    """Read a user's outbox
+
     Args:
         user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -143,15 +146,16 @@
 
 
 async def asyncio(
     user_name: str,
     *,
     client: AuthenticatedClient,
 ) -> Union[FederationCollectionPage]:
-    """
+    """Read a user's outbox
+
     Args:
         user_name (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user_apc_liked.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/general/parsers_get_parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,151 @@
-""""""
+"""List Parsers"""
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
-from ...models.federation_collection_page import FederationCollectionPage
+from ...models.parsers_get_parsers_response_200 import ParsersGetParsersResponse200
 from ...models.server_error import ServerError
 from ...types import Response
 
 
-def _get_kwargs(
-    user_name: str,
-) -> Dict[str, Any]:
+def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/user/{user_name}/liked".format(
-            user_name=user_name,
-        ),
+        "url": "/parsers",
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Union[FederationCollectionPage, ServerError]:
+) -> Union[ParsersGetParsersResponse200, ServerError]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = FederationCollectionPage.from_dict(response.json())
+        response_200 = ParsersGetParsersResponse200.from_dict(response.json())
 
         return response_200
-    if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = ServerError.from_dict(response.json())
-
-        return response_401
-    if response.status_code == HTTPStatus.FORBIDDEN:
-        response_403 = ServerError.from_dict(response.json())
-
-        return response_403
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
         response_500 = ServerError.from_dict(response.json())
 
         return response_500
 
     raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[FederationCollectionPage, ServerError]]:
+) -> Response[Union[ParsersGetParsersResponse200, ServerError]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    user_name: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[Union[FederationCollectionPage, ServerError]]:
-    """
-    Args:
-        user_name (str):
+    client: Union[AuthenticatedClient, Client],
+) -> Response[Union[ParsersGetParsersResponse200, ServerError]]:
+    """List Parsers
+
+    List the parsers available for items, their applicable item
+    types, and configuration options.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[FederationCollectionPage, ServerError]]
+        Response[Union[ParsersGetParsersResponse200, ServerError]]
     """
 
-    kwargs = _get_kwargs(
-        user_name=user_name,
-    )
+    kwargs = _get_kwargs()
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    user_name: str,
     *,
-    client: AuthenticatedClient,
-) -> Union[FederationCollectionPage]:
-    """
-    Args:
-        user_name (str):
+    client: Union[AuthenticatedClient, Client],
+) -> Union[ParsersGetParsersResponse200]:
+    """List Parsers
+
+    List the parsers available for items, their applicable item
+    types, and configuration options.
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[FederationCollectionPage]
+        Union[ParsersGetParsersResponse200]
     """
 
     response = sync_detailed(
-        user_name=user_name,
         client=client,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
 
 
 async def asyncio_detailed(
-    user_name: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[Union[FederationCollectionPage, ServerError]]:
-    """
-    Args:
-        user_name (str):
+    client: Union[AuthenticatedClient, Client],
+) -> Response[Union[ParsersGetParsersResponse200, ServerError]]:
+    """List Parsers
+
+    List the parsers available for items, their applicable item
+    types, and configuration options.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[FederationCollectionPage, ServerError]]
+        Response[Union[ParsersGetParsersResponse200, ServerError]]
     """
 
-    kwargs = _get_kwargs(
-        user_name=user_name,
-    )
+    kwargs = _get_kwargs()
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    user_name: str,
     *,
-    client: AuthenticatedClient,
-) -> Union[FederationCollectionPage]:
-    """
-    Args:
-        user_name (str):
+    client: Union[AuthenticatedClient, Client],
+) -> Union[ParsersGetParsersResponse200]:
+    """List Parsers
+
+    List the parsers available for items, their applicable item
+    types, and configuration options.
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[FederationCollectionPage]
+        Union[ParsersGetParsersResponse200]
     """
 
     response = await asyncio_detailed(
-        user_name=user_name,
         client=client,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_user_apc_outbox.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/metadata/metadata_set_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,54 @@
-""""""
+"""Update metadata field schema"""
 from http import HTTPStatus
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient
 from ...client import Client
-from ...models.federation_collection_page import FederationCollectionPage
+from ...models.metadata_fields import MetadataFields
 from ...models.server_error import ServerError
 from ...types import Response
 
 
 def _get_kwargs(
-    user_name: str,
+    *,
+    body: MetadataFields,
 ) -> Dict[str, Any]:
+    headers: Dict[str, Any] = {}
+
     _kwargs: Dict[str, Any] = {
-        "method": "get",
-        "url": "/user/{user_name}/outbox".format(
-            user_name=user_name,
-        ),
+        "method": "put",
+        "url": "/metadata/fields",
     }
 
+    _body = body.to_dict()
+
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Union[FederationCollectionPage, ServerError]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = FederationCollectionPage.from_dict(response.json())
+) -> Union[Any, ServerError]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, {"attribute": "None", "return_type": "None"})
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        response_400 = ServerError.from_dict(response.json())
 
-        return response_200
+        return response_400
     if response.status_code == HTTPStatus.UNAUTHORIZED:
         response_401 = ServerError.from_dict(response.json())
 
         return response_401
     if response.status_code == HTTPStatus.FORBIDDEN:
         response_403 = ServerError.from_dict(response.json())
 
@@ -48,122 +59,126 @@
         return response_500
 
     raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[FederationCollectionPage, ServerError]]:
+) -> Response[Union[Any, ServerError]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    user_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[Union[FederationCollectionPage, ServerError]]:
-    """
+    body: MetadataFields,
+) -> Response[Union[Any, ServerError]]:
+    """Update metadata field schema
+
     Args:
-        user_name (str):
+        body (MetadataFields):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[FederationCollectionPage, ServerError]]
+        Response[Union[Any, ServerError]]
     """
 
     kwargs = _get_kwargs(
-        user_name=user_name,
+        body=body,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    user_name: str,
     *,
     client: AuthenticatedClient,
-) -> Union[FederationCollectionPage]:
-    """
+    body: MetadataFields,
+) -> Union[Any]:
+    """Update metadata field schema
+
     Args:
-        user_name (str):
+        body (MetadataFields):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[FederationCollectionPage]
+        Union[Any]
     """
 
     response = sync_detailed(
-        user_name=user_name,
         client=client,
+        body=body,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
 
 
 async def asyncio_detailed(
-    user_name: str,
     *,
     client: AuthenticatedClient,
-) -> Response[Union[FederationCollectionPage, ServerError]]:
-    """
+    body: MetadataFields,
+) -> Response[Union[Any, ServerError]]:
+    """Update metadata field schema
+
     Args:
-        user_name (str):
+        body (MetadataFields):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[FederationCollectionPage, ServerError]]
+        Response[Union[Any, ServerError]]
     """
 
     kwargs = _get_kwargs(
-        user_name=user_name,
+        body=body,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    user_name: str,
     *,
     client: AuthenticatedClient,
-) -> Union[FederationCollectionPage]:
-    """
+    body: MetadataFields,
+) -> Union[Any]:
+    """Update metadata field schema
+
     Args:
-        user_name (str):
+        body (MetadataFields):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[FederationCollectionPage]
+        Union[Any]
     """
 
     response = await asyncio_detailed(
-        user_name=user_name,
         client=client,
+        body=body,
     )
     if isinstance(response.parsed, ServerError):
         raise errors.UnexpectedStatus(response.status_code, response.content)
 
     return response.parsed
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_get_users.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_get_users.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_receive_in_user_inbox.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_receive_in_user_inbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""""""
+"""Deliver an activity to the user's inbox"""
 from http import HTTPStatus
 from typing import Any
 from typing import cast
 from typing import Dict
 from typing import Union
 
 import httpx
@@ -89,15 +89,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Response[Union[Any, ServerError]]:
-    """
+    """Deliver an activity to the user's inbox
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -124,15 +125,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Union[Any]:
-    """
+    """Deliver an activity to the user's inbox
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
@@ -158,15 +160,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Response[Union[Any, ServerError]]:
-    """
+    """Deliver an activity to the user's inbox
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -191,15 +194,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Union[Any]:
-    """
+    """Deliver an activity to the user's inbox
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/api/user/user_send_to_user_outbox.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/api/user/user_send_to_user_outbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""""""
+"""Send an activity as a user"""
 from http import HTTPStatus
 from typing import Any
 from typing import cast
 from typing import Dict
 from typing import Union
 
 import httpx
@@ -89,15 +89,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Response[Union[Any, ServerError]]:
-    """
+    """Send an activity as a user
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -124,15 +125,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Union[Any]:
-    """
+    """Send an activity as a user
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
@@ -158,15 +160,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Response[Union[Any, ServerError]]:
-    """
+    """Send an activity as a user
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -191,15 +194,16 @@
     *,
     client: AuthenticatedClient,
     body: Union[
         FederationActivity,
         FederationActivity,
     ],
 ) -> Union[Any]:
-    """
+    """Send an activity as a user
+
     Args:
         user_name (str):
         body (FederationActivity):
         body (FederationActivity):
 
     Raises:
         errors.UnexpectedStatus: If the server returns a status code greater than or equal to 300.
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/client.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/client.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/login.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/login.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/__init__.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """ Contains all the data models used in inputs/outputs """
 from .account import Account
 from .account_create_account_body import AccountCreateAccountBody
+from .admin_grant_admin_admin_list_request import AdminGrantAdminAdminListRequest
+from .admin_grants import AdminGrants
+from .admin_list import AdminList
+from .admin_operations_item import AdminOperationsItem
 from .auth_activate_session_body import AuthActivateSessionBody
 from .auth_authenticate_user_authentication_request import (
     AuthAuthenticateUserAuthenticationRequest,
 )
 from .auth_authenticate_user_response_200 import AuthAuthenticateUserResponse200
 from .auth_get_csrf_response_200 import AuthGetCsrfResponse200
 from .auth_get_session_response_200 import AuthGetSessionResponse200
 from .auth_provider_authorized_provider import AuthProviderAuthorizedProvider
 from .auth_provider_login_provider import AuthProviderLoginProvider
 from .auth_provider_signin_provider_provider import AuthProviderSigninProviderProvider
 from .auth_provider_signin_provider_response_200 import (
     AuthProviderSigninProviderResponse200,
 )
 from .auth_providers_req_response_200 import AuthProvidersReqResponse200
+from .auth_signout_no_data import AuthSignoutNoData
+from .bundle import Bundle
+from .bundle_definition import BundleDefinition
 from .cdes_list_data_elements_response_200 import CdesListDataElementsResponse200
 from .cdes_new_cdeset_body import CdesNewCdesetBody
 from .cdeset import Cdeset
 from .cdeset_list import CdesetList
 from .collection import Collection
 from .collection_cde_stats import CollectionCdeStats
 from .collection_cde_stats_item_distrib_item import CollectionCdeStatsItemDistribItem
@@ -28,25 +35,16 @@
 from .collection_stats_item_stats import CollectionStatsItemStats
 from .collection_stats_item_stats_additional_property import (
     CollectionStatsItemStatsAdditionalProperty,
 )
 from .collections_dictionaries_copy_to_cdeset_body import (
     CollectionsDictionariesCopyToCdesetBody,
 )
-from .collections_dictionaries_create_a_new_data_element_data_element import (
-    CollectionsDictionariesCreateANewDataElementDataElement,
-)
-from .collections_dictionaries_create_a_new_data_element_data_element_data_type import (
-    CollectionsDictionariesCreateANewDataElementDataElementDataType,
-)
-from .collections_dictionaries_create_new_data_element_version_data_element import (
-    CollectionsDictionariesCreateNewDataElementVersionDataElement,
-)
-from .collections_dictionaries_create_new_data_element_version_data_element_data_type import (
-    CollectionsDictionariesCreateNewDataElementVersionDataElementDataType,
+from .collections_dictionaries_list_bundles_response_200 import (
+    CollectionsDictionariesListBundlesResponse200,
 )
 from .collections_dictionaries_list_data_element_refs_response_200 import (
     CollectionsDictionariesListDataElementRefsResponse200,
 )
 from .collections_dictionaries_list_data_elements_response_200 import (
     CollectionsDictionariesListDataElementsResponse200,
 )
@@ -94,17 +92,19 @@
 )
 from .collections_tables_list_tables_response_200 import (
     CollectionsTablesListTablesResponse200,
 )
 from .collections_tables_preview_table_data_body import (
     CollectionsTablesPreviewTableDataBody,
 )
+from .column_schema_type import ColumnSchemaType
 from .data_dictionary import DataDictionary
 from .data_dictionary_source_item import DataDictionarySourceItem
 from .data_element import DataElement
+from .data_element_bundle import DataElementBundle
 from .data_element_concept import DataElementConcept
 from .data_element_concept_applies_to import DataElementConceptAppliesTo
 from .data_element_data_type import DataElementDataType
 from .data_element_definition import DataElementDefinition
 from .data_element_definition_definition_type import DataElementDefinitionDefinitionType
 from .data_element_permissible_values_external_reference import (
     DataElementPermissibleValuesExternalReference,
@@ -153,41 +153,47 @@
 from .group import Group
 from .group_create_group_body import GroupCreateGroupBody
 from .group_get_groups_response_200 import GroupGetGroupsResponse200
 from .group_role import GroupRole
 from .identity import Identity
 from .item import Item
 from .item_column import ItemColumn
-from .item_column_type import ItemColumnType
+from .item_column_enum_map import ItemColumnEnumMap
 from .item_metadata import ItemMetadata
 from .item_parser import ItemParser
 from .item_parser_options import ItemParserOptions
 from .item_status import ItemStatus
 from .item_status_additional_property import ItemStatusAdditionalProperty
 from .item_status_detail import ItemStatusDetail
 from .item_status_detail_status import ItemStatusDetailStatus
 from .item_status_details import ItemStatusDetails
 from .item_storage import ItemStorage
 from .item_storage_checksum import ItemStorageChecksum
 from .item_type import ItemType
+from .metadata_fields import MetadataFields
+from .metadata_fields_data_elements import MetadataFieldsDataElements
 from .new_collection import NewCollection
 from .new_collection_metadata import NewCollectionMetadata
 from .new_collection_version import NewCollectionVersion
 from .new_collection_version_metadata import NewCollectionVersionMetadata
+from .new_data_element import NewDataElement
+from .new_data_element_data_type import NewDataElementDataType
 from .new_user import NewUser
 from .oauth_provider import OauthProvider
+from .ordered_dictionary import OrderedDictionary
 from .pagination import Pagination
 from .parser import Parser
 from .parser_options import ParserOptions
 from .parser_options_additional_property import ParserOptionsAdditionalProperty
 from .parser_options_additional_property_type import ParserOptionsAdditionalPropertyType
 from .parsers_get_parsers_response_200 import ParsersGetParsersResponse200
 from .parsers_resolve_prql_modules_response_200 import (
     ParsersResolvePrqlModulesResponse200,
 )
+from .preferred_order import PreferredOrder
 from .prql_module import PrqlModule
 from .root_get_datastores_response_200 import RootGetDatastoresResponse200
 from .search_collections_response import SearchCollectionsResponse
 from .search_collections_response_hits_item import SearchCollectionsResponseHitsItem
 from .search_collections_response_hits_item_items_item import (
     SearchCollectionsResponseHitsItemItemsItem,
 )
@@ -267,51 +273,53 @@
     SystemConfigurationWorkersBackendType,
 )
 from .table import Table
 from .table_data import TableData
 from .table_data_data_item import TableDataDataItem
 from .table_data_data_model import TableDataDataModel
 from .table_data_model import TableDataModel
-from .table_error import TableError
 from .termset import Termset
 from .termset_additional_property_item import TermsetAdditionalPropertyItem
 from .update_collection import UpdateCollection
 from .update_collection_metadata import UpdateCollectionMetadata
 from .user import User
 from .user_get_users_response_200 import UserGetUsersResponse200
 from .user_membership import UserMembership
-from .user_membership_role_type_1 import UserMembershipRoleType1
 
 __all__ = (
     "Account",
     "AccountCreateAccountBody",
+    "AdminGrantAdminAdminListRequest",
+    "AdminGrants",
+    "AdminList",
+    "AdminOperationsItem",
     "AuthActivateSessionBody",
     "AuthAuthenticateUserAuthenticationRequest",
     "AuthAuthenticateUserResponse200",
     "AuthGetCsrfResponse200",
     "AuthGetSessionResponse200",
     "AuthProviderAuthorizedProvider",
     "AuthProviderLoginProvider",
     "AuthProviderSigninProviderProvider",
     "AuthProviderSigninProviderResponse200",
     "AuthProvidersReqResponse200",
+    "AuthSignoutNoData",
+    "Bundle",
+    "BundleDefinition",
     "Cdeset",
     "CdesetList",
     "CdesListDataElementsResponse200",
     "CdesNewCdesetBody",
     "Collection",
     "CollectionCdeStats",
     "CollectionCdeStatsItemDistribItem",
     "CollectionCdeStatsPerCde",
     "CollectionMetadata",
     "CollectionsDictionariesCopyToCdesetBody",
-    "CollectionsDictionariesCreateANewDataElementDataElement",
-    "CollectionsDictionariesCreateANewDataElementDataElementDataType",
-    "CollectionsDictionariesCreateNewDataElementVersionDataElement",
-    "CollectionsDictionariesCreateNewDataElementVersionDataElementDataType",
+    "CollectionsDictionariesListBundlesResponse200",
     "CollectionsDictionariesListDataElementRefsResponse200",
     "CollectionsDictionariesListDataElementsResponse200",
     "CollectionsDictionariesListDictionariesResponse200",
     "CollectionsGetCollectionApcMembersFilter",
     "CollectionsGetCollectionsCollectionList",
     "CollectionsItemsCopyItemBody",
     "CollectionsItemsCreateItemFilesFormStyleUpload",
@@ -327,17 +335,19 @@
     "CollectionsTablesGetTableDataElementsResponse200ElementMap",
     "CollectionsTablesGetTableDataElementsResponse200ErrorMap",
     "CollectionsTablesListTablesResponse200",
     "CollectionsTablesPreviewTableDataBody",
     "CollectionStats",
     "CollectionStatsItemStats",
     "CollectionStatsItemStatsAdditionalProperty",
+    "ColumnSchemaType",
     "DataDictionary",
     "DataDictionarySourceItem",
     "DataElement",
+    "DataElementBundle",
     "DataElementConcept",
     "DataElementConceptAppliesTo",
     "DataElementDataType",
     "DataElementDefinition",
     "DataElementDefinitionDefinitionType",
     "DataElementPermissibleValuesExternalReference",
     "DataElementPermissibleValuesExternalReferenceExternalReference",
@@ -366,39 +376,45 @@
     "Group",
     "GroupCreateGroupBody",
     "GroupGetGroupsResponse200",
     "GroupRole",
     "Identity",
     "Item",
     "ItemColumn",
-    "ItemColumnType",
+    "ItemColumnEnumMap",
     "ItemMetadata",
     "ItemParser",
     "ItemParserOptions",
     "ItemStatus",
     "ItemStatusAdditionalProperty",
     "ItemStatusDetail",
     "ItemStatusDetails",
     "ItemStatusDetailStatus",
     "ItemStorage",
     "ItemStorageChecksum",
     "ItemType",
+    "MetadataFields",
+    "MetadataFieldsDataElements",
     "NewCollection",
     "NewCollectionMetadata",
     "NewCollectionVersion",
     "NewCollectionVersionMetadata",
+    "NewDataElement",
+    "NewDataElementDataType",
     "NewUser",
     "OauthProvider",
+    "OrderedDictionary",
     "Pagination",
     "Parser",
     "ParserOptions",
     "ParserOptionsAdditionalProperty",
     "ParserOptionsAdditionalPropertyType",
     "ParsersGetParsersResponse200",
     "ParsersResolvePrqlModulesResponse200",
+    "PreferredOrder",
     "PrqlModule",
     "RootGetDatastoresResponse200",
     "SearchCollectionsResponse",
     "SearchCollectionsResponseHitsItem",
     "SearchCollectionsResponseHitsItemItemsItem",
     "SearchDictionariesByItemColumnHits",
     "SearchDictionariesByItemColumnHitsSearchDictionariesHit",
@@ -438,17 +454,15 @@
     "SystemConfigurationWorkers",
     "SystemConfigurationWorkersBackendType",
     "Table",
     "TableData",
     "TableDataDataItem",
     "TableDataDataModel",
     "TableDataModel",
-    "TableError",
     "Termset",
     "TermsetAdditionalPropertyItem",
     "UpdateCollection",
     "UpdateCollectionMetadata",
     "User",
     "UserGetUsersResponse200",
     "UserMembership",
-    "UserMembershipRoleType1",
 )
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/account.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/account.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/account_create_account_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/account_create_account_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_activate_session_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_activate_session_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_authenticate_user_authentication_request.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_authenticate_user_authentication_request.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_authenticate_user_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_authenticate_user_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_get_csrf_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_get_csrf_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_get_session_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_get_session_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_provider_signin_provider_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_provider_signin_provider_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/auth_providers_req_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/auth_providers_req_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/cdes_list_data_elements_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/cdes_list_data_elements_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/cdes_new_cdeset_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/cdes_new_cdeset_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/cdeset.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/cdeset.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/cdeset_list.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/cdeset_list.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_cde_stats.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_cde_stats.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_cde_stats_item_distrib_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_cde_stats_item_distrib_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_cde_stats_per_cde.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_cde_stats_per_cde.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_metadata.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_metadata.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_stats.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_stats.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_stats_item_stats.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_stats_item_stats.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collection_stats_item_stats_additional_property.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collection_stats_item_stats_additional_property.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_copy_to_cdeset_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_copy_to_cdeset_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_create_a_new_data_element_data_element.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/new_data_element.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,57 +3,54 @@
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 from attrs import define as _attrs_define
 
-from ..models.collections_dictionaries_create_a_new_data_element_data_element_data_type import (
-    CollectionsDictionariesCreateANewDataElementDataElementDataType,
-)
 from ..models.data_element_concept import DataElementConcept
 from ..models.data_element_definition import DataElementDefinition
 from ..models.data_element_permissible_values_external_reference import (
     DataElementPermissibleValuesExternalReference,
 )
 from ..models.data_element_permissible_values_number_range import (
     DataElementPermissibleValuesNumberRange,
 )
 from ..models.data_element_permissible_values_text_range import (
     DataElementPermissibleValuesTextRange,
 )
 from ..models.data_element_permissible_values_value_set import (
     DataElementPermissibleValuesValueSet,
 )
+from ..models.new_data_element_data_type import NewDataElementDataType
 from ..types import UNSET
 from ..types import Unset
 
 
-T = TypeVar("T", bound="CollectionsDictionariesCreateANewDataElementDataElement")
+T = TypeVar("T", bound="NewDataElement")
 
 
 @_attrs_define
-class CollectionsDictionariesCreateANewDataElementDataElement:
+class NewDataElement:
     """Pigeon Data Element
 
     Attributes:
-        data_type (CollectionsDictionariesCreateANewDataElementDataElementDataType): The data type valid for this data
-            element.
+        data_type (NewDataElementDataType): The data type valid for this data element.
         name (str): The title or name of the data element.
         concepts (Union[Unset, List['DataElementConcept']]): Linked concepts for the data element.
         definition (Union[Unset, List['DataElementDefinition']]): Any definitions that describe or inform the context of
             the data element.
         permissible_values (Union[Unset, List[Union['DataElementPermissibleValuesExternalReference',
             'DataElementPermissibleValuesNumberRange', 'DataElementPermissibleValuesTextRange',
             'DataElementPermissibleValuesValueSet']]]): Describes the values that this data element properly represents.
         permit_null (Union[Unset, bool]): If true, nulls will not cause validation failures. Default: False.
         sensitivity (Union[Unset, bool]): Whether this data element references sensitive data (PHI, PII, etc.)
     """
 
-    data_type: CollectionsDictionariesCreateANewDataElementDataElementDataType
+    data_type: NewDataElementDataType
     name: str
     concepts: Union[Unset, List["DataElementConcept"]] = UNSET
     definition: Union[Unset, List["DataElementDefinition"]] = UNSET
     permissible_values: Union[
         Unset,
         List[
             Union[
@@ -129,19 +126,17 @@
         if sensitivity is not UNSET:
             field_dict["sensitivity"] = sensitivity
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        """Create an instance of :py:class:`CollectionsDictionariesCreateANewDataElementDataElement` from a dict"""
+        """Create an instance of :py:class:`NewDataElement` from a dict"""
         d = src_dict.copy()
-        data_type = CollectionsDictionariesCreateANewDataElementDataElementDataType(
-            d.pop("dataType")
-        )
+        data_type = NewDataElementDataType(d.pop("dataType"))
 
         name = d.pop("name")
 
         concepts = []
         _concepts = d.pop("concepts", UNSET)
         for concepts_item_data in _concepts or []:
             concepts_item = DataElementConcept.from_dict(concepts_item_data)
@@ -211,18 +206,18 @@
 
             permissible_values.append(permissible_values_item)
 
         permit_null = d.pop("permitNull", UNSET)
 
         sensitivity = d.pop("sensitivity", UNSET)
 
-        collections_dictionaries_create_a_new_data_element_data_element = cls(
+        new_data_element = cls(
             data_type=data_type,
             name=name,
             concepts=concepts,
             definition=definition,
             permissible_values=permissible_values,
             permit_null=permit_null,
             sensitivity=sensitivity,
         )
 
-        return collections_dictionaries_create_a_new_data_element_data_element
+        return new_data_element
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_create_new_data_element_version_data_element.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 from attrs import define as _attrs_define
 
-from ..models.collections_dictionaries_create_new_data_element_version_data_element_data_type import (
-    CollectionsDictionariesCreateNewDataElementVersionDataElementDataType,
-)
 from ..models.data_element_concept import DataElementConcept
+from ..models.data_element_data_type import DataElementDataType
 from ..models.data_element_definition import DataElementDefinition
 from ..models.data_element_permissible_values_external_reference import (
     DataElementPermissibleValuesExternalReference,
 )
 from ..models.data_element_permissible_values_number_range import (
     DataElementPermissibleValuesNumberRange,
 )
@@ -24,37 +22,42 @@
 from ..models.data_element_permissible_values_value_set import (
     DataElementPermissibleValuesValueSet,
 )
 from ..types import UNSET
 from ..types import Unset
 
 
-T = TypeVar("T", bound="CollectionsDictionariesCreateNewDataElementVersionDataElement")
+T = TypeVar("T", bound="DataElement")
 
 
 @_attrs_define
-class CollectionsDictionariesCreateNewDataElementVersionDataElement:
+class DataElement:
     """Pigeon Data Element
 
     Attributes:
-        data_type (CollectionsDictionariesCreateNewDataElementVersionDataElementDataType): The data type valid for this
-            data element.
+        data_type (DataElementDataType): The data type valid for this data element.
+        id (str):
         name (str): The title or name of the data element.
+        url (str):
+        version (str):
         concepts (Union[Unset, List['DataElementConcept']]): Linked concepts for the data element.
         definition (Union[Unset, List['DataElementDefinition']]): Any definitions that describe or inform the context of
             the data element.
         permissible_values (Union[Unset, List[Union['DataElementPermissibleValuesExternalReference',
             'DataElementPermissibleValuesNumberRange', 'DataElementPermissibleValuesTextRange',
             'DataElementPermissibleValuesValueSet']]]): Describes the values that this data element properly represents.
         permit_null (Union[Unset, bool]): If true, nulls will not cause validation failures. Default: False.
         sensitivity (Union[Unset, bool]): Whether this data element references sensitive data (PHI, PII, etc.)
     """
 
-    data_type: CollectionsDictionariesCreateNewDataElementVersionDataElementDataType
+    data_type: DataElementDataType
+    id: str
     name: str
+    url: str
+    version: str
     concepts: Union[Unset, List["DataElementConcept"]] = UNSET
     definition: Union[Unset, List["DataElementDefinition"]] = UNSET
     permissible_values: Union[
         Unset,
         List[
             Union[
                 "DataElementPermissibleValuesExternalReference",
@@ -66,15 +69,18 @@
     ] = UNSET
     permit_null: Union[Unset, bool] = False
     sensitivity: Union[Unset, bool] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
         data_type = self.data_type.value
+        id = self.id
         name = self.name
+        url = self.url
+        version = self.version
         concepts: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.concepts, Unset):
             concepts = []
             for concepts_item_data in self.concepts:
                 concepts_item = concepts_item_data.to_dict()
                 concepts.append(concepts_item)
 
@@ -111,15 +117,18 @@
         permit_null = self.permit_null
         sensitivity = self.sensitivity
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
                 "dataType": data_type,
+                "id": id,
                 "name": name,
+                "url": url,
+                "version": version,
             }
         )
         if concepts is not UNSET:
             field_dict["concepts"] = concepts
         if definition is not UNSET:
             field_dict["definition"] = definition
         if permissible_values is not UNSET:
@@ -129,24 +138,26 @@
         if sensitivity is not UNSET:
             field_dict["sensitivity"] = sensitivity
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        """Create an instance of :py:class:`CollectionsDictionariesCreateNewDataElementVersionDataElement` from a dict"""
+        """Create an instance of :py:class:`DataElement` from a dict"""
         d = src_dict.copy()
-        data_type = (
-            CollectionsDictionariesCreateNewDataElementVersionDataElementDataType(
-                d.pop("dataType")
-            )
-        )
+        data_type = DataElementDataType(d.pop("dataType"))
+
+        id = d.pop("id")
 
         name = d.pop("name")
 
+        url = d.pop("url")
+
+        version = d.pop("version")
+
         concepts = []
         _concepts = d.pop("concepts", UNSET)
         for concepts_item_data in _concepts or []:
             concepts_item = DataElementConcept.from_dict(concepts_item_data)
 
             concepts.append(concepts_item)
 
@@ -213,18 +224,21 @@
 
             permissible_values.append(permissible_values_item)
 
         permit_null = d.pop("permitNull", UNSET)
 
         sensitivity = d.pop("sensitivity", UNSET)
 
-        collections_dictionaries_create_new_data_element_version_data_element = cls(
+        data_element = cls(
             data_type=data_type,
+            id=id,
             name=name,
+            url=url,
+            version=version,
             concepts=concepts,
             definition=definition,
             permissible_values=permissible_values,
             permit_null=permit_null,
             sensitivity=sensitivity,
         )
 
-        return collections_dictionaries_create_new_data_element_version_data_element
+        return data_element
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_list_data_element_refs_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_data_element_refs_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_list_data_elements_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_data_elements_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_dictionaries_list_dictionaries_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_dictionaries_list_dictionaries_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_get_collections_collection_list.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_get_collections_collection_list.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_copy_item_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_copy_item_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload_metadata.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content_checksum.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_create_item_json_new_item_request_content_checksum.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_list_items_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_list_items_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_put_item_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_put_item_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_put_item_body_content.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_put_item_body_content.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_items_put_item_body_content_checksum.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_items_put_item_body_content_checksum.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_element_map.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_element_map.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_error_map.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_error_map.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_list_tables_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_list_tables_response_200.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 from attrs import define as _attrs_define
 
+from ..models.error import Error
 from ..models.pagination import Pagination
 from ..models.table import Table
-from ..models.table_error import TableError
 
 
 T = TypeVar("T", bound="CollectionsTablesListTablesResponse200")
 
 
 @_attrs_define
 class CollectionsTablesListTablesResponse200:
     """CollectionsTablesListTablesResponse200 model
 
     Attributes:
-        errors (List['TableError']):
+        errors (List['Error']):
         pagination (Pagination):
         tables (List['Table']):
     """
 
-    errors: List["TableError"]
+    errors: List["Error"]
     pagination: "Pagination"
     tables: List["Table"]
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
         errors = []
         for errors_item_data in self.errors:
@@ -55,15 +55,15 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """Create an instance of :py:class:`CollectionsTablesListTablesResponse200` from a dict"""
         d = src_dict.copy()
         errors = []
         _errors = d.pop("errors")
         for errors_item_data in _errors:
-            errors_item = TableError.from_dict(errors_item_data)
+            errors_item = Error.from_dict(errors_item_data)
 
             errors.append(errors_item)
 
         pagination = Pagination.from_dict(d.pop("pagination"))
 
         tables = []
         _tables = d.pop("tables")
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/collections_tables_preview_table_data_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/collections_tables_preview_table_data_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_dictionary.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_dictionary.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_concept.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_concept.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_definition.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_definition.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference_external_reference.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_external_reference_external_reference.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_number_range.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_number_range.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_number_range_number_range.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_number_range_number_range.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_text_range.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_text_range.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_text_range_text_range.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_text_range_text_range.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_value_set.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_value_set.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_permissible_values_value_set_value_set_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_permissible_values_value_set_value_set_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/data_element_reference.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/data_element_reference.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/datastore.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/datastore.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options_options.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options_options.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/dictionary_search_options_options_additional_property.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/dictionary_search_options_options_additional_property.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/error.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/error.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_activity.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_activity.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_address_or_object_type_2.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_address_or_object_type_2.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_collection.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_collection.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_collection_page.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_collection_page.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/federation_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/federation_user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/group.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/group.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/group_create_group_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/group_create_group_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/group_get_groups_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/group_get_groups_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/identity.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/identity.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_column.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_column.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from typing import Dict
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 from attrs import define as _attrs_define
 
-from ..models.item_column_type import ItemColumnType
+from ..models.column_schema_type import ColumnSchemaType
+from ..models.item_column_enum_map import ItemColumnEnumMap
 from ..types import UNSET
 from ..types import Unset
 
 
 T = TypeVar("T", bound="ItemColumn")
 
 
@@ -20,31 +21,38 @@
     """ItemColumn model
 
     Attributes:
         name (str):
         data_element_ref (Union[Unset, str]): A URL referencing a specific data element (and optional
             version) within a PDD, CDE set, or other data element
             source.
+        enum_map (Union[Unset, ItemColumnEnumMap]): When provided, defines the mapping between the values
+            present in the column and the permissible values defined
+            in the referenced data element.
         represents_pv (Union[Unset, int, str]): When provided, this indicates that this column
             represents one of the permissible values from the
             referenced data element. The desired permissible value
             must be placed in this field, and the column type must
             be either 'Categorical' or 'Boolean'.
-        type (Union[Unset, ItemColumnType]):
+        type (Union[Unset, ColumnSchemaType]):
     """
 
     name: str
     data_element_ref: Union[Unset, str] = UNSET
+    enum_map: Union[Unset, "ItemColumnEnumMap"] = UNSET
     represents_pv: Union[Unset, int, str] = UNSET
-    type: Union[Unset, ItemColumnType] = UNSET
+    type: Union[Unset, ColumnSchemaType] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
         name = self.name
         data_element_ref = self.data_element_ref
+        enum_map: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.enum_map, Unset):
+            enum_map = self.enum_map.to_dict()
         represents_pv: Union[Unset, int, str]
         if isinstance(self.represents_pv, Unset):
             represents_pv = UNSET
         else:
             represents_pv = self.represents_pv
         type: Union[Unset, str] = UNSET
         if not isinstance(self.type, Unset):
@@ -54,14 +62,16 @@
         field_dict.update(
             {
                 "name": name,
             }
         )
         if data_element_ref is not UNSET:
             field_dict["data_element_ref"] = data_element_ref
+        if enum_map is not UNSET:
+            field_dict["enum_map"] = enum_map
         if represents_pv is not UNSET:
             field_dict["represents_pv"] = represents_pv
         if type is not UNSET:
             field_dict["type"] = type
 
         return field_dict
 
@@ -69,29 +79,37 @@
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         """Create an instance of :py:class:`ItemColumn` from a dict"""
         d = src_dict.copy()
         name = d.pop("name")
 
         data_element_ref = d.pop("data_element_ref", UNSET)
 
+        _enum_map = d.pop("enum_map", UNSET)
+        enum_map: Union[Unset, ItemColumnEnumMap]
+        if isinstance(_enum_map, Unset):
+            enum_map = UNSET
+        else:
+            enum_map = ItemColumnEnumMap.from_dict(_enum_map)
+
         def _parse_represents_pv(data: object) -> Union[Unset, int, str]:
             if isinstance(data, Unset):
                 return data
             return cast(Union[Unset, int, str], data)
 
         represents_pv = _parse_represents_pv(d.pop("represents_pv", UNSET))
 
         _type = d.pop("type", UNSET)
-        type: Union[Unset, ItemColumnType]
+        type: Union[Unset, ColumnSchemaType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
-            type = ItemColumnType(_type)
+            type = ColumnSchemaType(_type)
 
         item_column = cls(
             name=name,
             data_element_ref=data_element_ref,
+            enum_map=enum_map,
             represents_pv=represents_pv,
             type=type,
         )
 
         return item_column
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_metadata.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_metadata.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_parser.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_parser.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_parser_options.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_parser_options.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status_detail.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status_detail.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_status_details.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_status_details.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_storage.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_storage.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/item_storage_checksum.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/item_storage_checksum.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection_metadata.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection_version.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection_version.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/new_collection_version_metadata.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/new_collection_version_metadata.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/new_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/new_user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/oauth_provider.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/pagination.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/pagination.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/parser.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/parser.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/parser_options.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/parser_options.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/parser_options_additional_property.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/parser_options_additional_property.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/root_get_datastores_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/root_get_datastores_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_collections_response.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_collections_response.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_collections_response_hits_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_collections_response_hits_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_collections_response_hits_item_items_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_collections_response_hits_item_items_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 from attrs import define as _attrs_define
 
-from ..models.item_column_type import ItemColumnType
+from ..models.column_schema_type import ColumnSchemaType
 from ..models.search_dictionaries_by_item_column_hits_search_dictionaries_hit import (
     SearchDictionariesByItemColumnHitsSearchDictionariesHit,
 )
 
 
 T = TypeVar("T", bound="SearchDictionariesByItemColumnHits")
 
@@ -18,20 +18,20 @@
 @_attrs_define
 class SearchDictionariesByItemColumnHits:
     """SearchDictionariesByItemColumnHits model
 
     Attributes:
         hits (List['SearchDictionariesByItemColumnHitsSearchDictionariesHit']):
         name (str):
-        type_as_parsed (ItemColumnType):
+        type_as_parsed (ColumnSchemaType):
     """
 
     hits: List["SearchDictionariesByItemColumnHitsSearchDictionariesHit"]
     name: str
-    type_as_parsed: ItemColumnType
+    type_as_parsed: ColumnSchemaType
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
         hits = []
         for hits_item_data in self.hits:
             hits_item = hits_item_data.to_dict()
             hits.append(hits_item)
@@ -63,15 +63,15 @@
                 )
             )
 
             hits.append(hits_item)
 
         name = d.pop("name")
 
-        type_as_parsed = ItemColumnType(d.pop("type_as_parsed"))
+        type_as_parsed = ColumnSchemaType(d.pop("type_as_parsed"))
 
         search_dictionaries_by_item_column_hits = cls(
             hits=hits,
             name=name,
             type_as_parsed=type_as_parsed,
         )
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits_search_dictionaries_hit.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits_search_dictionaries_hit.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_inverse_response.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_inverse_response.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_by_item_response.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_by_item_response.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_inverse_result.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_inverse_result.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_inverse_result_queries_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_inverse_result_queries_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_dictionaries_response.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_dictionaries_response.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_get_collection_terms_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_get_collection_terms_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_get_dictionary_search_options_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_get_dictionary_search_options_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_collections_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_collections_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_collections_body_facets.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_collections_body_facets.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_body_options.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_body_options.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_inverse_body.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/search_search_dictionaries_by_item_inverse_body.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/server_error.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/server_error.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/session_token.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/session_token.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/session_user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/session_user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_0.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_1.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_2.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_authentication_additional_property_type_2.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_cache.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_cache.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_0.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_1.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_datastores_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/system_configuration_workers.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/system_configuration_workers.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/table.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 from attrs import define as _attrs_define
 
+from ..models.error import Error
 from ..models.table_data_model import TableDataModel
-from ..models.table_error import TableError
 from ..types import UNSET
 from ..types import Unset
 
 
 T = TypeVar("T", bound="Table")
 
 
 @_attrs_define
 class Table:
     """Dataview summary
 
     Attributes:
         description (str):
-        errors (List['TableError']):
+        errors (List['Error']):
         name (str):
         data_model (Union[Unset, TableDataModel]):
     """
 
     description: str
-    errors: List["TableError"]
+    errors: List["Error"]
     name: str
     data_model: Union[Unset, "TableDataModel"] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
         description = self.description
         errors = []
@@ -63,15 +63,15 @@
         """Create an instance of :py:class:`Table` from a dict"""
         d = src_dict.copy()
         description = d.pop("description")
 
         errors = []
         _errors = d.pop("errors")
         for errors_item_data in _errors:
-            errors_item = TableError.from_dict(errors_item_data)
+            errors_item = Error.from_dict(errors_item_data)
 
             errors.append(errors_item)
 
         name = d.pop("name")
 
         _data_model = d.pop("data_model", UNSET)
         data_model: Union[Unset, TableDataModel]
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 from attrs import define as _attrs_define
 
+from ..models.error import Error
 from ..models.pagination import Pagination
 from ..models.table_data_data_item import TableDataDataItem
 from ..models.table_data_data_model import TableDataDataModel
-from ..models.table_error import TableError
 
 
 T = TypeVar("T", bound="TableData")
 
 
 @_attrs_define
 class TableData:
     """Dataview contents
 
     Attributes:
         data (List['TableDataDataItem']):
         data_model (TableDataDataModel):
-        errors (List['TableError']):
+        errors (List['Error']):
         pagination (Pagination):
     """
 
     data: List["TableDataDataItem"]
     data_model: "TableDataDataModel"
-    errors: List["TableError"]
+    errors: List["Error"]
     pagination: "Pagination"
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
         data = []
         for data_item_data in self.data:
             data_item = data_item_data.to_dict()
@@ -70,15 +70,15 @@
             data.append(data_item)
 
         data_model = TableDataDataModel.from_dict(d.pop("data_model"))
 
         errors = []
         _errors = d.pop("errors")
         for errors_item_data in _errors:
-            errors_item = TableError.from_dict(errors_item_data)
+            errors_item = Error.from_dict(errors_item_data)
 
             errors.append(errors_item)
 
         pagination = Pagination.from_dict(d.pop("pagination"))
 
         table_data = cls(
             data=data,
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data_data_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data_data_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data_data_model.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data_data_model.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/table_data_model.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/table_data_model.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/table_error.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/bundle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 from typing import Any
+from typing import cast
 from typing import Dict
+from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 from attrs import define as _attrs_define
 
 from ..types import UNSET
 from ..types import Unset
 
 
-T = TypeVar("T", bound="TableError")
+T = TypeVar("T", bound="Bundle")
 
 
 @_attrs_define
-class TableError:
-    """TableError model
+class Bundle:
+    """Bundle model
 
     Attributes:
-        detail (str):
-        title (str):
-        source (Union[Unset, str]):
+        elements (List[str]):
+        id (str):
+        name (str):
+        version (Union[Unset, str]):
     """
 
-    detail: str
-    title: str
-    source: Union[Unset, str] = UNSET
+    elements: List[str]
+    id: str
+    name: str
+    version: Union[Unset, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert to a dict"""
-        detail = self.detail
-        title = self.title
-        source = self.source
+        elements = self.elements
+
+        id = self.id
+        name = self.name
+        version = self.version
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(
             {
-                "detail": detail,
-                "title": title,
+                "elements": elements,
+                "id": id,
+                "name": name,
             }
         )
-        if source is not UNSET:
-            field_dict["source"] = source
+        if version is not UNSET:
+            field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        """Create an instance of :py:class:`TableError` from a dict"""
+        """Create an instance of :py:class:`Bundle` from a dict"""
         d = src_dict.copy()
-        detail = d.pop("detail")
+        elements = cast(List[str], d.pop("elements"))
+
+        id = d.pop("id")
 
-        title = d.pop("title")
+        name = d.pop("name")
 
-        source = d.pop("source", UNSET)
+        version = d.pop("version", UNSET)
 
-        table_error = cls(
-            detail=detail,
-            title=title,
-            source=source,
+        bundle = cls(
+            elements=elements,
+            id=id,
+            name=name,
+            version=version,
         )
 
-        return table_error
+        return bundle
```

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/termset.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/termset.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/termset_additional_property_item.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/termset_additional_property_item.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/update_collection.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/update_collection.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/update_collection_metadata.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/update_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/user.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/user.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/models/user_get_users_response_200.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/models/user_get_users_response_200.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/paginator.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/paginator.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon/pigeon_core/types.py` & `pypigeon-0.2.8/pypigeon/pigeon_core/types.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/pypigeon.egg-info/PKG-INFO` & `pypigeon-0.2.8/pypigeon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pypigeon
-Version: 0.2.6
+Version: 0.2.8
 Summary: an easy-to-use Python client for Pigeon
 Author-email: BioTeam <contact@bioteam.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: httpx<0.26.0,>=0.20.0
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: python-dateutil
 Requires-Dist: pyarrow
 Requires-Dist: pandas
 Requires-Dist: tqdm
+Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-httpx<0.26.0,>=0.20.0; extra == "dev"
 Requires-Dist: openapi-python-client==0.17.2; extra == "dev"
 Requires-Dist: reorder-python-imports; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: black==23.12.1; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: types-tqdm; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
+Requires-Dist: types-tabulate; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 
 # PyPigeon
```

### Comparing `pypigeon-0.2.6/pypigeon.egg-info/SOURCES.txt` & `pypigeon-0.2.8/pypigeon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,33 @@
 pypigeon/pcmd/__init__.py
 pypigeon/pcmd/__main__.py
 pypigeon/pcmd/cli.py
 pypigeon/pcmd/commands/__init__.py
 pypigeon/pcmd/commands/auth.py
 pypigeon/pcmd/commands/base_commands.py
 pypigeon/pcmd/commands/cde.py
+pypigeon/pcmd/commands/config.py
 pypigeon/pcmd/commands/pdd.py
+pypigeon/pcmd/commands/users.py
 pypigeon/pigeon_core/.opcignore
 pypigeon/pigeon_core/__init__.py
 pypigeon/pigeon_core/client.py
 pypigeon/pigeon_core/errors.py
 pypigeon/pigeon_core/login.py
 pypigeon/pigeon_core/paginator.py
 pypigeon/pigeon_core/types.py
 pypigeon/pigeon_core/api/__init__.py
 pypigeon/pigeon_core/api/account/__init__.py
 pypigeon/pigeon_core/api/account/account_create_account.py
 pypigeon/pigeon_core/api/account/account_delete_account.py
 pypigeon/pigeon_core/api/account/account_get_account.py
 pypigeon/pigeon_core/api/admin/__init__.py
 pypigeon/pigeon_core/api/admin/admin_get_config.py
+pypigeon/pigeon_core/api/admin/admin_grant_admin.py
+pypigeon/pigeon_core/api/admin/admin_list_admins.py
 pypigeon/pigeon_core/api/admin/admin_put_config.py
 pypigeon/pigeon_core/api/auth/__init__.py
 pypigeon/pigeon_core/api/auth/auth_activate_session.py
 pypigeon/pigeon_core/api/auth/auth_authenticate_user.py
 pypigeon/pigeon_core/api/auth/auth_get_csrf.py
 pypigeon/pigeon_core/api/auth/auth_get_session.py
 pypigeon/pigeon_core/api/auth/auth_new_session.py
@@ -65,52 +69,63 @@
 pypigeon/pigeon_core/api/auth/auth_provider_login.py
 pypigeon/pigeon_core/api/auth/auth_provider_signin_provider.py
 pypigeon/pigeon_core/api/auth/auth_providers_req.py
 pypigeon/pigeon_core/api/auth/auth_signin.py
 pypigeon/pigeon_core/api/auth/auth_signout.py
 pypigeon/pigeon_core/api/cde/__init__.py
 pypigeon/pigeon_core/api/cde/cdes_delete_cdeset.py
-pypigeon/pigeon_core/api/cde/cdes_get_cdeset.py
+pypigeon/pigeon_core/api/cde/cdes_get_data_element_latest.py
+pypigeon/pigeon_core/api/cde/cdes_get_data_element_version.py
+pypigeon/pigeon_core/api/cde/cdes_get_ordered_cdeset.py
 pypigeon/pigeon_core/api/cde/cdes_list_cdesets.py
 pypigeon/pigeon_core/api/cde/cdes_list_data_elements.py
 pypigeon/pigeon_core/api/cde/cdes_new_cdeset.py
 pypigeon/pigeon_core/api/collections/__init__.py
 pypigeon/pigeon_core/api/collections/collections_create_collection.py
 pypigeon/pigeon_core/api/collections/collections_create_collection_version.py
 pypigeon/pigeon_core/api/collections/collections_delete_collection_version.py
 pypigeon/pigeon_core/api/collections/collections_get_cde_stats.py
 pypigeon/pigeon_core/api/collections/collections_get_collection_version.py
 pypigeon/pigeon_core/api/collections/collections_get_collections.py
 pypigeon/pigeon_core/api/collections/collections_get_stats.py
 pypigeon/pigeon_core/api/collections/collections_update_collection_meta.py
 pypigeon/pigeon_core/api/collections/collections_update_collection_metapatch.py
 pypigeon/pigeon_core/api/data_dictionaries/__init__.py
-pypigeon/pigeon_core/api/data_dictionaries/cdes_get_data_element_latest.py
-pypigeon/pigeon_core/api/data_dictionaries/cdes_get_data_element_version.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_copy_to_cdeset.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_a_new_data_element_ref.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_ref_version.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_create_new_data_element_version.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_bundle.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_delete_data_element.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_bundle.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_latest.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_latest.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_ref_version.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_data_element_version.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_order.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_get_ordered_dictionary.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_bundles.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_element_refs.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_data_elements.py
 pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_list_dictionaries.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_new_bundle.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_set_order.py
+pypigeon/pigeon_core/api/data_dictionaries/collections_dictionaries_update_bundle.py
 pypigeon/pigeon_core/api/federation/__init__.py
 pypigeon/pigeon_core/api/federation/collections_get_collection_apc_inbox.py
 pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members.py
 pypigeon/pigeon_core/api/federation/collections_get_collection_apc_members_pending.py
 pypigeon/pigeon_core/api/federation/collections_get_collection_apc_outbox.py
 pypigeon/pigeon_core/api/federation/collections_process_inbox_message.py
 pypigeon/pigeon_core/api/general/__init__.py
+pypigeon/pigeon_core/api/general/parsers_get_parsers.py
+pypigeon/pigeon_core/api/general/parsers_resolve_prql_modules.py
 pypigeon/pigeon_core/api/general/root_get_datastores.py
+pypigeon/pigeon_core/api/general/root_resolve_data_element_ref.py
 pypigeon/pigeon_core/api/group/__init__.py
 pypigeon/pigeon_core/api/group/group_create_group.py
 pypigeon/pigeon_core/api/group/group_delete_group.py
 pypigeon/pigeon_core/api/group/group_get_group.py
 pypigeon/pigeon_core/api/group/group_get_groups.py
 pypigeon/pigeon_core/api/items/__init__.py
 pypigeon/pigeon_core/api/items/collections_items_copy_item.py
@@ -118,14 +133,17 @@
 pypigeon/pigeon_core/api/items/collections_items_delete_item.py
 pypigeon/pigeon_core/api/items/collections_items_get_item.py
 pypigeon/pigeon_core/api/items/collections_items_get_item_data.py
 pypigeon/pigeon_core/api/items/collections_items_get_item_status.py
 pypigeon/pigeon_core/api/items/collections_items_list_items.py
 pypigeon/pigeon_core/api/items/collections_items_put_item.py
 pypigeon/pigeon_core/api/items/collections_items_put_item_data.py
+pypigeon/pigeon_core/api/metadata/__init__.py
+pypigeon/pigeon_core/api/metadata/metadata_get_fields.py
+pypigeon/pigeon_core/api/metadata/metadata_set_fields.py
 pypigeon/pigeon_core/api/search/__init__.py
 pypigeon/pigeon_core/api/search/search_get_collection_terms.py
 pypigeon/pigeon_core/api/search/search_get_dictionary_search_options.py
 pypigeon/pigeon_core/api/search/search_search_collections.py
 pypigeon/pigeon_core/api/search/search_search_dictionaries.py
 pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item.py
 pypigeon/pigeon_core/api/search/search_search_dictionaries_by_item_inverse.py
@@ -145,41 +163,45 @@
 pypigeon/pigeon_core/api/user/user_get_user_apc_outbox.py
 pypigeon/pigeon_core/api/user/user_get_users.py
 pypigeon/pigeon_core/api/user/user_receive_in_user_inbox.py
 pypigeon/pigeon_core/api/user/user_send_to_user_outbox.py
 pypigeon/pigeon_core/models/__init__.py
 pypigeon/pigeon_core/models/account.py
 pypigeon/pigeon_core/models/account_create_account_body.py
+pypigeon/pigeon_core/models/admin_grant_admin_admin_list_request.py
+pypigeon/pigeon_core/models/admin_grants.py
+pypigeon/pigeon_core/models/admin_list.py
+pypigeon/pigeon_core/models/admin_operations_item.py
 pypigeon/pigeon_core/models/auth_activate_session_body.py
 pypigeon/pigeon_core/models/auth_authenticate_user_authentication_request.py
 pypigeon/pigeon_core/models/auth_authenticate_user_response_200.py
 pypigeon/pigeon_core/models/auth_get_csrf_response_200.py
 pypigeon/pigeon_core/models/auth_get_session_response_200.py
 pypigeon/pigeon_core/models/auth_provider_authorized_provider.py
 pypigeon/pigeon_core/models/auth_provider_login_provider.py
 pypigeon/pigeon_core/models/auth_provider_signin_provider_provider.py
 pypigeon/pigeon_core/models/auth_provider_signin_provider_response_200.py
 pypigeon/pigeon_core/models/auth_providers_req_response_200.py
+pypigeon/pigeon_core/models/auth_signout_no_data.py
+pypigeon/pigeon_core/models/bundle.py
+pypigeon/pigeon_core/models/bundle_definition.py
 pypigeon/pigeon_core/models/cdes_list_data_elements_response_200.py
 pypigeon/pigeon_core/models/cdes_new_cdeset_body.py
 pypigeon/pigeon_core/models/cdeset.py
 pypigeon/pigeon_core/models/cdeset_list.py
 pypigeon/pigeon_core/models/collection.py
 pypigeon/pigeon_core/models/collection_cde_stats.py
 pypigeon/pigeon_core/models/collection_cde_stats_item_distrib_item.py
 pypigeon/pigeon_core/models/collection_cde_stats_per_cde.py
 pypigeon/pigeon_core/models/collection_metadata.py
 pypigeon/pigeon_core/models/collection_stats.py
 pypigeon/pigeon_core/models/collection_stats_item_stats.py
 pypigeon/pigeon_core/models/collection_stats_item_stats_additional_property.py
 pypigeon/pigeon_core/models/collections_dictionaries_copy_to_cdeset_body.py
-pypigeon/pigeon_core/models/collections_dictionaries_create_a_new_data_element_data_element.py
-pypigeon/pigeon_core/models/collections_dictionaries_create_a_new_data_element_data_element_data_type.py
-pypigeon/pigeon_core/models/collections_dictionaries_create_new_data_element_version_data_element.py
-pypigeon/pigeon_core/models/collections_dictionaries_create_new_data_element_version_data_element_data_type.py
+pypigeon/pigeon_core/models/collections_dictionaries_list_bundles_response_200.py
 pypigeon/pigeon_core/models/collections_dictionaries_list_data_element_refs_response_200.py
 pypigeon/pigeon_core/models/collections_dictionaries_list_data_elements_response_200.py
 pypigeon/pigeon_core/models/collections_dictionaries_list_dictionaries_response_200.py
 pypigeon/pigeon_core/models/collections_get_collection_apc_members_filter.py
 pypigeon/pigeon_core/models/collections_get_collections_collection_list.py
 pypigeon/pigeon_core/models/collections_items_copy_item_body.py
 pypigeon/pigeon_core/models/collections_items_create_item_files_form_style_upload.py
@@ -192,17 +214,19 @@
 pypigeon/pigeon_core/models/collections_items_put_item_body_content.py
 pypigeon/pigeon_core/models/collections_items_put_item_body_content_checksum.py
 pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200.py
 pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_element_map.py
 pypigeon/pigeon_core/models/collections_tables_get_table_data_elements_response_200_error_map.py
 pypigeon/pigeon_core/models/collections_tables_list_tables_response_200.py
 pypigeon/pigeon_core/models/collections_tables_preview_table_data_body.py
+pypigeon/pigeon_core/models/column_schema_type.py
 pypigeon/pigeon_core/models/data_dictionary.py
 pypigeon/pigeon_core/models/data_dictionary_source_item.py
 pypigeon/pigeon_core/models/data_element.py
+pypigeon/pigeon_core/models/data_element_bundle.py
 pypigeon/pigeon_core/models/data_element_concept.py
 pypigeon/pigeon_core/models/data_element_concept_applies_to.py
 pypigeon/pigeon_core/models/data_element_data_type.py
 pypigeon/pigeon_core/models/data_element_definition.py
 pypigeon/pigeon_core/models/data_element_definition_definition_type.py
 pypigeon/pigeon_core/models/data_element_permissible_values_external_reference.py
 pypigeon/pigeon_core/models/data_element_permissible_values_external_reference_external_reference.py
@@ -231,37 +255,46 @@
 pypigeon/pigeon_core/models/group.py
 pypigeon/pigeon_core/models/group_create_group_body.py
 pypigeon/pigeon_core/models/group_get_groups_response_200.py
 pypigeon/pigeon_core/models/group_role.py
 pypigeon/pigeon_core/models/identity.py
 pypigeon/pigeon_core/models/item.py
 pypigeon/pigeon_core/models/item_column.py
-pypigeon/pigeon_core/models/item_column_type.py
+pypigeon/pigeon_core/models/item_column_enum_map.py
 pypigeon/pigeon_core/models/item_metadata.py
 pypigeon/pigeon_core/models/item_parser.py
 pypigeon/pigeon_core/models/item_parser_options.py
 pypigeon/pigeon_core/models/item_status.py
 pypigeon/pigeon_core/models/item_status_additional_property.py
 pypigeon/pigeon_core/models/item_status_detail.py
 pypigeon/pigeon_core/models/item_status_detail_status.py
 pypigeon/pigeon_core/models/item_status_details.py
 pypigeon/pigeon_core/models/item_storage.py
 pypigeon/pigeon_core/models/item_storage_checksum.py
 pypigeon/pigeon_core/models/item_type.py
+pypigeon/pigeon_core/models/metadata_fields.py
+pypigeon/pigeon_core/models/metadata_fields_data_elements.py
 pypigeon/pigeon_core/models/new_collection.py
 pypigeon/pigeon_core/models/new_collection_metadata.py
 pypigeon/pigeon_core/models/new_collection_version.py
 pypigeon/pigeon_core/models/new_collection_version_metadata.py
+pypigeon/pigeon_core/models/new_data_element.py
+pypigeon/pigeon_core/models/new_data_element_data_type.py
 pypigeon/pigeon_core/models/new_user.py
 pypigeon/pigeon_core/models/oauth_provider.py
+pypigeon/pigeon_core/models/ordered_dictionary.py
 pypigeon/pigeon_core/models/pagination.py
 pypigeon/pigeon_core/models/parser.py
 pypigeon/pigeon_core/models/parser_options.py
 pypigeon/pigeon_core/models/parser_options_additional_property.py
 pypigeon/pigeon_core/models/parser_options_additional_property_type.py
+pypigeon/pigeon_core/models/parsers_get_parsers_response_200.py
+pypigeon/pigeon_core/models/parsers_resolve_prql_modules_response_200.py
+pypigeon/pigeon_core/models/preferred_order.py
+pypigeon/pigeon_core/models/prql_module.py
 pypigeon/pigeon_core/models/root_get_datastores_response_200.py
 pypigeon/pigeon_core/models/search_collections_response.py
 pypigeon/pigeon_core/models/search_collections_response_hits_item.py
 pypigeon/pigeon_core/models/search_collections_response_hits_item_items_item.py
 pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits.py
 pypigeon/pigeon_core/models/search_dictionaries_by_item_column_hits_search_dictionaries_hit.py
 pypigeon/pigeon_core/models/search_dictionaries_by_item_inverse_response.py
@@ -300,21 +333,19 @@
 pypigeon/pigeon_core/models/system_configuration_workers.py
 pypigeon/pigeon_core/models/system_configuration_workers_backend_type.py
 pypigeon/pigeon_core/models/table.py
 pypigeon/pigeon_core/models/table_data.py
 pypigeon/pigeon_core/models/table_data_data_item.py
 pypigeon/pigeon_core/models/table_data_data_model.py
 pypigeon/pigeon_core/models/table_data_model.py
-pypigeon/pigeon_core/models/table_error.py
 pypigeon/pigeon_core/models/termset.py
 pypigeon/pigeon_core/models/termset_additional_property_item.py
 pypigeon/pigeon_core/models/update_collection.py
 pypigeon/pigeon_core/models/update_collection_metadata.py
 pypigeon/pigeon_core/models/user.py
 pypigeon/pigeon_core/models/user_get_users_response_200.py
 pypigeon/pigeon_core/models/user_membership.py
-pypigeon/pigeon_core/models/user_membership_role_type_1.py
 tests/client_test.py
 tests/collections_test.py
 tests/conftest.py
 tests/pigeon_core/login_test.py
 tests/pigeon_core/paginator_test.py
```

### Comparing `pypigeon-0.2.6/pyproject.toml` & `pypigeon-0.2.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 dependencies = [
     "httpx>=0.20.0,<0.26.0",
     "attrs>=21.3.0",
     "python-dateutil",
     "pyarrow",
     "pandas",
     "tqdm",
+    "tabulate",
 ]
 
 [project.optional-dependencies]
 dev = [
     "sphinx",
     "pytest",
     "pytest-httpx>=0.20.0,<0.26.0",
@@ -34,14 +35,15 @@
     "ruff",
     "black==23.12.1",
     "mypy",
     "types-python-dateutil",
     "pandas-stubs",
     "types-tqdm",
     "types-PyYAML",
+    "types-tabulate",
     "build",
     "twine",
 ]
 doc = [
     "sphinx",
 ]
```

### Comparing `pypigeon-0.2.6/tests/client_test.py` & `pypigeon-0.2.8/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/tests/collections_test.py` & `pypigeon-0.2.8/tests/collections_test.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/tests/pigeon_core/login_test.py` & `pypigeon-0.2.8/tests/pigeon_core/login_test.py`

 * *Files identical despite different names*

### Comparing `pypigeon-0.2.6/tests/pigeon_core/paginator_test.py` & `pypigeon-0.2.8/tests/pigeon_core/paginator_test.py`

 * *Files identical despite different names*

