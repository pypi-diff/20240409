# Comparing `tmp/tyro-0.8.2.tar.gz` & `tmp/tyro-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.8.2.tar", last modified: Sat Apr  6 00:00:15 2024, max compression
+gzip compressed data, was "tyro-0.8.3.tar", last modified: Tue Apr  9 19:25:26 2024, max compression
```

## Comparing `tyro-0.8.2.tar` & `tyro-0.8.3.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.126873 tyro-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 23:58:18.000000 tyro-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-06 00:00:15.126873 tyro-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-06 00:00:13.000000 tyro-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-05 23:58:18.000000 tyro-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:00:15.126873 tyro-0.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.114873 tyro-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.118873 tyro-0.8.2/src/tyro/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54289 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_argparse_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22872 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    18589 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    42889 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    24359 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_instantiators.py
--rw-r--r--   0 runner    (1001) docker     (127)    25673 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_subcommand_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/_unsafe_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.118873 tyro-0.8.2/src/tyro/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/conf/_confstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/conf/_markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.118873 tyro-0.8.2/src/tyro/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/extras/_base_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/extras/_choices_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/extras/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/extras/_subcommand_cli_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:58:18.000000 tyro-0.8.2/src/tyro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.126873 tyro-0.8.2/src/tyro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-06 00:00:15.000000 tyro-0.8.2/src/tyro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-06 00:00:15.000000 tyro-0.8.2/src/tyro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:00:15.000000 tyro-0.8.2/src/tyro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-06 00:00:15.000000 tyro-0.8.2/src/tyro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 00:00:15.000000 tyro-0.8.2/src/tyro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:00:15.126873 tyro-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_base_configs_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_boolean_optional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    40475 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_dcargs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_dict_namedtuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_dynamic_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_flax_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_generics_and_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_helptext.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_initvar_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_is_nested_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_missing_optional_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_mixed_unions.py
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_nested_in_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_new_style_annotations_min_py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_new_style_annotations_min_py312.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_new_style_annotations_min_py39.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_positional_min_py38.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_pydantic_with_newtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_self_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_tuple_with_subcommands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_union_from_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_unsafe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-05 23:58:18.000000 tyro-0.8.2/tests/test_unsupported_but_should_work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.033469 tyro-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 19:24:55.000000 tyro-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-09 19:25:26.033469 tyro-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-09 19:25:23.000000 tyro-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-09 19:24:55.000000 tyro-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:25:26.033469 tyro-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.017469 tyro-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.021469 tyro-0.8.3/src/tyro/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101735 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54903 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_argparse_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22874 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42889 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24359 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_subcommand_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/_unsafe_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.021469 tyro-0.8.3/src/tyro/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/conf/_confstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/conf/_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.021469 tyro-0.8.3/src/tyro/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_choices_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/extras/_subcommand_cli_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:24:55.000000 tyro-0.8.3/src/tyro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.029469 tyro-0.8.3/src/tyro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 19:25:26.000000 tyro-0.8.3/src/tyro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:25:26.029469 tyro-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_base_configs_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_boolean_optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40475 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_dcargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_dict_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_dynamic_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_flax_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12768 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_generics_and_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_helptext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_initvar_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_is_nested_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_missing_optional_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_mixed_unions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_nested_in_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_new_style_annotations_min_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_new_style_annotations_min_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_new_style_annotations_min_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_positional_min_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_pydantic_with_newtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_self_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_tuple_with_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_union_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_unsafe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-09 19:24:55.000000 tyro-0.8.3/tests/test_unsupported_but_should_work.py
```

### Comparing `tyro-0.8.2/LICENSE` & `tyro-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/PKG-INFO` & `tyro-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.8.2
+Version: 0.8.3
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tyro Version: 0.8.2 Summary: Strongly typed, zero-
+Metadata-Version: 2.1 Name: tyro Version: 0.8.3 Summary: Strongly typed, zero-
 effort CLI interfaces Author-email: brentyi
 berkeley.edu> License: MIT Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
```

### Comparing `tyro-0.8.2/README.md` & `tyro-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/pyproject.toml` & `tyro-0.8.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tyro"
 authors = [
     {name = "brentyi", email = "brentyi@berkeley.edu"},
 ]
-version = "0.8.2"  # TODO: currently needs to be synchronized manually with __init__.py.
+version = "0.8.3"  # TODO: currently needs to be synchronized manually with __init__.py.
 description = "Strongly typed, zero-effort CLI interfaces"
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
@@ -63,15 +63,18 @@
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 python_version = "3.12"
 ignore_missing_imports = true
 warn_unused_configs = true
-exclude = "^tests/test_py311_generated/.*"
+exclude = ["^tests/test_py311_generated/.*", "_argparse\\.py"]
+
+[tool.coverage.run]
+omit = ["**/_argparse.py"]
 
 [tool.coverage.report]
 exclude_lines = [
     # Have to re-enable the standard pragma
     "pragma: no cover",
 
     # Don't compute coverage for abstract methods, properties
@@ -123,7 +126,12 @@
     "PLC1901",  # Use falsey strings.
     "PLR5501",  # Use `elif` instead of `else if`.
     "PLR0911",  # Too many return statements.
     "PLR0912",  # Too many branches.
     "PLW0603",  # Global statement updates are discouraged.
     "PLW2901"  # For loop variable overwritten.
 ]
+extend-exclude = ["**/_argparse.py"]
+
+[tool.pyright]
+pythonVersion = "3.12"
+ignore = ["**/_argparse.py"]
```

### Comparing `tyro-0.8.2/src/tyro/_argparse_formatter.py` & `tyro-0.8.3/src/tyro/_argparse_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Utilities and functions for helptext formatting. We replace argparse's simple help
 messages with ones that:
     - Are more nicely formatted!
     - Support multiple columns when many fields are defined.
     - Use `rich` for formatting.
     - Can be themed with an accent color.
 
-This is largely built by fussing around in argparse implementation details, and is
-extremely chaotic as a result.
-
-TODO: the current implementation should be robust given our test coverage, but unideal
-long-term. We should just maintain our own fork of argparse.
+This is largely built by fussing around in argparse implementation details. It's
+chaotic as a result; for stability we mirror argparse at _argparse.py.
 """
 
 from __future__ import annotations
 
-import argparse
+import argparse as argparse_sys
 import contextlib
 import dataclasses
 import difflib
 import itertools
 import re as _re
 import shlex
 import shutil
@@ -33,14 +30,15 @@
 from rich.rule import Rule
 from rich.style import Style
 from rich.table import Table
 from rich.text import Text
 from rich.theme import Theme
 from typing_extensions import override
 
+from . import _argparse as argparse
 from . import _arguments, _strings, conf
 from ._parsers import ParserSpecification
 
 
 @dataclasses.dataclass
 class TyroTheme:
     border: Style = Style()
@@ -265,15 +263,17 @@
 # arguments.
 #
 # Our current solution is to manually track unrecognized arguments in _parse_known_args,
 # and in error() override other errors when unrecognized arguments are present.
 global_unrecognized_args: List[str] = []
 
 
-class TyroArgumentParser(argparse.ArgumentParser):
+# We inherit from both our local mirror of argparse and the upstream one.
+# Including the latter is purely for `isinstance()`-style checks.
+class TyroArgumentParser(argparse.ArgumentParser, argparse_sys.ArgumentParser):  # type: ignore
     _parser_specification: ParserSpecification
     _parsing_known_args: bool
     _args: List[str]
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
@@ -355,30 +355,29 @@
             if argument_values is not argparse.SUPPRESS:
                 action(self, namespace, argument_values, option_string)
 
         # function to convert arg_strings into an optional action
         def consume_optional(start_index):
             # get the optional identified at this index
             option_tuple = option_string_indices[start_index]
-            action, option_string, explicit_arg = option_tuple
+            action, option_string, sep, explicit_arg = option_tuple
 
             # identify additional optionals in the same arg string
             # (e.g. -xyz is the same as -x -y -z if no args are required)
             match_argument = self._match_argument
             action_tuples = []
             while True:
                 # if we found no optional action, skip it
                 if action is None:
                     # <new>
                     # Manually track unused arguments to assist with error messages
                     # later.
                     if not self._parsing_known_args:
                         global_unrecognized_args.append(option_string)
                     # </new>
-
                     extras.append(arg_strings[start_index])
                     return start_index + 1
 
                 # if there is an explicit argument, try to match the
                 # optional's string arguments to only this
                 if explicit_arg is not None:
                     arg_count = match_argument(action, "A")
@@ -388,26 +387,35 @@
                     # of the tail of the option string
                     chars = self.prefix_chars
                     if (
                         arg_count == 0
                         and option_string[1] not in chars
                         and explicit_arg != ""
                     ):
+                        if sep or explicit_arg[0] in chars:
+                            msg = _("ignored explicit argument %r")
+                            raise argparse.ArgumentError(action, msg % explicit_arg)
                         action_tuples.append((action, [], option_string))
                         char = option_string[0]
                         option_string = char + explicit_arg[0]
-                        new_explicit_arg = explicit_arg[1:] or None
                         optionals_map = self._option_string_actions
                         if option_string in optionals_map:
                             action = optionals_map[option_string]
-                            explicit_arg = new_explicit_arg
+                            explicit_arg = explicit_arg[1:]
+                            if not explicit_arg:
+                                sep = explicit_arg = None
+                            elif explicit_arg[0] == "=":
+                                sep = "="
+                                explicit_arg = explicit_arg[1:]
+                            else:
+                                sep = ""
                         else:
-                            msg = _("ignored explicit argument %r")
-                            raise argparse.ArgumentError(action, msg % explicit_arg)
-
+                            extras.append(char + explicit_arg)
+                            stop = start_index + 1
+                            break
                     # if the action expect exactly one argument, we've
                     # successfully matched the option; exit the loop
                     elif arg_count == 1:
                         stop = start_index + 1
                         args = [explicit_arg]
                         action_tuples.append((action, args, option_string))
                         break
```

### Comparing `tyro-0.8.2/src/tyro/_arguments.py` & `tyro-0.8.3/src/tyro/_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Rules for taking high-level field definitions and lowering them into inputs for
 argparse's `add_argument()`."""
 
 from __future__ import annotations
 
-import argparse
 import dataclasses
 import enum
 import functools
 import itertools
 import json
 import shlex
 from typing import (
@@ -26,14 +25,15 @@
     Union,
     cast,
 )
 
 import rich.markup
 import shtab
 
+from . import _argparse as argparse
 from . import _fields, _instantiators, _resolver, _strings
 from ._typing import TypeForm
 from .conf import _markers
 
 if TYPE_CHECKING:
     cached_property = property
 else:
@@ -44,15 +44,14 @@
         # Python 3.7.
         from backports.cached_property import cached_property  # type: ignore
 
 
 _T = TypeVar("_T")
 
 
-# TODO: refactor!
 class BooleanOptionalAction(argparse.Action):
     """Adapted from https://github.com/python/cpython/pull/27672"""
 
     def __init__(
         self,
         option_strings: Sequence[str],
         dest: str,
```

### Comparing `tyro-0.8.2/src/tyro/_calling.py` & `tyro-0.8.3/src/tyro/_calling.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_cli.py` & `tyro-0.8.3/src/tyro/_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Core public API."""
 
-import argparse
 import dataclasses
 import pathlib
 import sys
 import warnings
 from typing import (
     Callable,
     Dict,
@@ -17,14 +16,15 @@
     cast,
     overload,
 )
 
 import shtab
 from typing_extensions import Literal
 
+from . import _argparse as argparse
 from . import (
     _argparse_formatter,
     _arguments,
     _calling,
     _fields,
     _parsers,
     _strings,
```

### Comparing `tyro-0.8.2/src/tyro/_docstrings.py` & `tyro-0.8.3/src/tyro/_docstrings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_fields.py` & `tyro-0.8.3/src/tyro/_fields.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_instantiators.py` & `tyro-0.8.3/src/tyro/_instantiators.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_parsers.py` & `tyro-0.8.3/src/tyro/_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Interface for generating `argparse.ArgumentParser()` definitions from callables."""
 
 from __future__ import annotations
 
-import argparse
 import dataclasses
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
@@ -16,14 +15,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 from typing_extensions import Annotated, get_args, get_origin
 
+from . import _argparse as argparse
 from . import (
     _argparse_formatter,
     _arguments,
     _docstrings,
     _fields,
     _instantiators,
     _resolver,
```

### Comparing `tyro-0.8.2/src/tyro/_resolver.py` & `tyro-0.8.3/src/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_strings.py` & `tyro-0.8.3/src/tyro/_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_subcommand_matching.py` & `tyro-0.8.3/src/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_typing.py` & `tyro-0.8.3/src/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/_unsafe_cache.py` & `tyro-0.8.3/src/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/conf/__init__.py` & `tyro-0.8.3/src/tyro/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/conf/_confstruct.py` & `tyro-0.8.3/src/tyro/conf/_confstruct.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/conf/_markers.py` & `tyro-0.8.3/src/tyro/conf/_markers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/extras/__init__.py` & `tyro-0.8.3/src/tyro/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/extras/_base_configs.py` & `tyro-0.8.3/src/tyro/extras/_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/extras/_choices_type.py` & `tyro-0.8.3/src/tyro/extras/_choices_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/extras/_serialization.py` & `tyro-0.8.3/src/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro/extras/_subcommand_cli_from_dict.py` & `tyro-0.8.3/src/tyro/extras/_subcommand_cli_from_dict.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/src/tyro.egg-info/PKG-INFO` & `tyro-0.8.3/src/tyro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.8.2
+Version: 0.8.3
 Summary: Strongly typed, zero-effort CLI interfaces
 Author-email: brentyi <brentyi@berkeley.edu>
 License: MIT
 Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tyro Version: 0.8.2 Summary: Strongly typed, zero-
+Metadata-Version: 2.1 Name: tyro Version: 0.8.3 Summary: Strongly typed, zero-
 effort CLI interfaces Author-email: brentyi
 berkeley.edu> License: MIT Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
```

### Comparing `tyro-0.8.2/src/tyro.egg-info/SOURCES.txt` & `tyro-0.8.3/src/tyro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 src/tyro/__init__.py
+src/tyro/_argparse.py
 src/tyro/_argparse_formatter.py
 src/tyro/_arguments.py
 src/tyro/_calling.py
 src/tyro/_cli.py
 src/tyro/_deprecated.py
 src/tyro/_docstrings.py
 src/tyro/_fields.py
```

### Comparing `tyro-0.8.2/src/tyro.egg-info/requires.txt` & `tyro-0.8.3/src/tyro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_attrs.py` & `tyro-0.8.3/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_base_configs_nested.py` & `tyro-0.8.3/tests/test_base_configs_nested.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_boolean_optional.py` & `tyro-0.8.3/tests/test_boolean_optional.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_collections.py` & `tyro-0.8.3/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_completion.py` & `tyro-0.8.3/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_conf.py` & `tyro-0.8.3/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_dcargs.py` & `tyro-0.8.3/tests/test_dcargs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_dict_namedtuple.py` & `tyro-0.8.3/tests/test_dict_namedtuple.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_errors.py` & `tyro-0.8.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_flax_min_py38.py` & `tyro-0.8.3/tests/test_flax_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_forward_ref.py` & `tyro-0.8.3/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_functools.py` & `tyro-0.8.3/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_generics_and_serialization.py` & `tyro-0.8.3/tests/test_generics_and_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_helptext.py` & `tyro-0.8.3/tests/test_helptext.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_initvar_min_py38.py` & `tyro-0.8.3/tests/test_initvar_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_is_nested_type.py` & `tyro-0.8.3/tests/test_is_nested_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_missing.py` & `tyro-0.8.3/tests/test_missing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_missing_optional_packages.py` & `tyro-0.8.3/tests/test_missing_optional_packages.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_mixed_unions.py` & `tyro-0.8.3/tests/test_mixed_unions.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_nested.py` & `tyro-0.8.3/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_nested_in_containers.py` & `tyro-0.8.3/tests/test_nested_in_containers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_new_style_annotations_min_py310.py` & `tyro-0.8.3/tests/test_new_style_annotations_min_py310.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_new_style_annotations_min_py312.py` & `tyro-0.8.3/tests/test_new_style_annotations_min_py312.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_new_style_annotations_min_py39.py` & `tyro-0.8.3/tests/test_new_style_annotations_min_py39.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_partial.py` & `tyro-0.8.3/tests/test_partial.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_positional_min_py38.py` & `tyro-0.8.3/tests/test_positional_min_py38.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_pydantic.py` & `tyro-0.8.3/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_pydantic_with_newtype.py` & `tyro-0.8.3/tests/test_pydantic_with_newtype.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_self_type.py` & `tyro-0.8.3/tests/test_self_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_strings.py` & `tyro-0.8.3/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_tuple_with_subcommands.py` & `tyro-0.8.3/tests/test_tuple_with_subcommands.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_union_from_mapping.py` & `tyro-0.8.3/tests/test_union_from_mapping.py`

 * *Files identical despite different names*

### Comparing `tyro-0.8.2/tests/test_unsupported_but_should_work.py` & `tyro-0.8.3/tests/test_unsupported_but_should_work.py`

 * *Files identical despite different names*

