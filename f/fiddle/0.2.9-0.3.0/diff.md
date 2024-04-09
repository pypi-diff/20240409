# Comparing `tmp/fiddle-0.2.9.tar.gz` & `tmp/fiddle-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddle-0.2.9.tar", last modified: Fri Jul 21 19:08:24 2023, max compression
+gzip compressed data, was "fiddle-0.3.0.tar", last modified: Tue Apr  9 00:15:23 2024, max compression
```

## Comparing `fiddle-0.2.9.tar` & `fiddle-0.3.0.tar`

### file list

```diff
@@ -1,217 +1,238 @@
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.9/LICENSE
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-21 19:08:24.555863 fiddle-0.2.9/PKG-INFO
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-07-21 19:08:10.000000 fiddle-0.2.9/README.md
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.539863 fiddle-0.2.9/fiddle/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.543863 fiddle-0.2.9/fiddle/_src/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.543863 fiddle-0.2.9/fiddle/_src/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/absl_flags/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1047 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/flags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15534 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/legacy_flags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/sample_module_for_flags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7150 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/absl_flags/utils.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/arg_factory_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5939 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/building.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/building_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.543863 fiddle-0.2.9/fiddle/_src/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.547863 fiddle-0.2.9/fiddle/_src/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7956 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2506 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5371 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8540 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11095 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5265 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3942 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7921 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6294 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8328 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7507 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6640 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8476 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2765 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4027 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17405 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/sub_fixture.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11681 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/sub_fixture_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5759 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/auto_config/test_fixtures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17419 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/formatting_utilities.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/import_manager.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/import_manager_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9134 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/mini_ast.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/codegen/namespace.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/namespace_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5207 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/new_codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3653 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/new_codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4537 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6544 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15928 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6189 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/special_value_codegen.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.547863 fiddle-0.2.9/fiddle/_src/codegen/test_submodule/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/test_submodule/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/test_submodule/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/codegen/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    42592 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    53885 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    27540 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish_extensions.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish_extensions_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    20247 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/daglish_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/diffing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45929 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/diffing_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43693 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5668 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/auto_config_policy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    44111 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/auto_config_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3167 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2917 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/dataclasses_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/dict_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7286 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/lazy_imports.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9119 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/lazy_imports_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      909 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/lazy_imports_test_example.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/namespace_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30877 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/transform_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11539 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/with_tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/with_tags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2804 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4422 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/flax_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/seqio_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/extensions/tf_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36979 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/graphviz_custom_object.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9437 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/history_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/materialize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/materialize_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3459 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/module_reflection.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/module_reflection_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/module_reflection_test_module.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/mutate_buildable.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/mutate_buildable_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14648 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/printing_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/reraised_exception.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/reraised_exception_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10408 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11289 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/selectors_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4274 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/signatures_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/signatures_test_helper.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7368 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/tagging.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    13570 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/tagging_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/tagging_test_module.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/autotest.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/_src/testing/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2463 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/demo_configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2533 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/fake_encoder_decoder.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/example/person_friend_toy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/nested_values.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/nested_values_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/_src/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/_src/testing/test_util_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.551863 fiddle-0.2.9/fiddle/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      967 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/absl_flags/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/business_logic.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/absl_flags/example/configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/example.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/absl_flags/example/tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/building.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1076 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2119 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/diffing.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/examples/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/examples/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/examples/colabs/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/examples/colabs/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1719 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/experimental/auto_config_policy.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      854 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/lazy_imports.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/experimental/yaml_serialization.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/tagging.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.555863 fiddle-0.2.9/fiddle/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-07-21 19:08:10.000000 fiddle-0.2.9/fiddle/testing/autotest.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-07-21 19:08:11.000000 fiddle-0.2.9/fiddle/version.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-21 19:08:24.539863 fiddle-0.2.9/fiddle.egg-info/
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/PKG-INFO
--rw-r-----   0 dhr      (201437) primarygroup (89939)     7166 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/SOURCES.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/dependency_links.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/requires.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-07-21 19:08:24.000000 fiddle-0.2.9/fiddle.egg-info/top_level.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-07-21 19:08:24.555863 fiddle-0.2.9/setup.cfg
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-07-21 19:08:11.000000 fiddle-0.2.9/setup.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.603339 fiddle-0.3.0/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.3.0/LICENSE
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1705 2024-04-09 00:15:23.603339 fiddle-0.3.0/PKG-INFO
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2024-04-09 00:14:26.000000 fiddle-0.3.0/README.md
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.575339 fiddle-0.3.0/fiddle/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1683 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.583339 fiddle-0.3.0/fiddle/_src/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.583339 fiddle-0.3.0/fiddle/_src/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/absl_flags/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11799 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/absl_flags/flags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15264 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/absl_flags/legacy_flags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/absl_flags/sample_module_for_flags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1577 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/absl_flags/sample_test_binary.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10385 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/absl_flags/utils.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/arg_factory_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6317 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/building.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/building_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2327 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/casting.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.587339 fiddle-0.3.0/fiddle/_src/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.591339 fiddle-0.3.0/fiddle/_src/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4332 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/add_type_signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3525 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/add_type_signatures_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8393 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/code_ir.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2553 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/code_ir_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5334 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/complex_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8644 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11384 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/get_history_comments.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/get_history_comments_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2009 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/import_manager_wrapper.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/init_task.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/init_task_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5730 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_printer.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4155 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_printer_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9623 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_to_cst.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7074 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7902 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/make_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7507 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6640 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/naming.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8590 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/naming_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/parents_first_traversal.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2765 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4027 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/shared_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2299 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/split_arg_factories.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2449 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17434 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/sub_fixture.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11681 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/sub_fixture_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5759 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/auto_config/test_fixtures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    19117 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/formatting_utilities.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9073 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/import_manager.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/import_manager_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11285 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/legacy_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9248 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/legacy_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/mini_ast.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/namespace.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/namespace_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5696 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/new_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3701 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/new_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4188 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/newcg_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6544 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/newcg_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15956 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6190 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/py_val_to_cst_converter_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/special_value_codegen.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.591339 fiddle-0.3.0/fiddle/_src/codegen/test_submodule/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/test_submodule/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/test_submodule/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/codegen/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    34073 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41213 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1802 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/copying.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2246 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/copying_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30618 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/daglish_extensions.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/daglish_extensions_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    24373 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/daglish_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41581 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/diffing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    47564 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/diffing_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.595339 fiddle-0.3.0/fiddle/_src/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43951 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5701 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/auto_config_policy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45491 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/auto_config_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.595339 fiddle-0.3.0/fiddle/_src/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/autobuilders/autobuilders.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/autobuilders/autobuilders_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/daglish_legacy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/daglish_legacy_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3167 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2917 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/dataclasses_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/dict_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8179 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/lazy_imports.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/lazy_imports_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      918 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/lazy_imports_test_example.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/namespace_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    31040 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3267 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5085 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/transform_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11563 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/with_tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/with_tags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2833 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/yaml_serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4422 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/experimental/yaml_serialization_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.595339 fiddle-0.3.0/fiddle/_src/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/flax_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3679 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/numpy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5069 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/numpy_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/seqio_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/extensions/tf_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    37044 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/graphviz_custom_object.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9711 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5853 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/history_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2411 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/materialize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/materialize_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3459 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/module_reflection.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/module_reflection_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/module_reflection_test_module.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5208 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/mutate_buildable.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5117 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/mutate_buildable_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10061 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/partial.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14727 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/partial_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    13513 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    19500 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/printing_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/reraised_exception.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/reraised_exception_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10401 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11289 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/selectors_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12943 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11299 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/signatures_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/signatures_test_helper.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4310 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/special_overrides.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11001 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/tagging.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    21423 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/tagging_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/tagging_test_module.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/_src/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/autotest.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/_src/testing/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2463 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/example/demo_configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2553 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/example/fake_encoder_decoder.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/example/person_friend_toy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5626 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/nested_values.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/nested_values_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/testing/test_util_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/_src/validation/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5169 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/baseline_style.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/baseline_style_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3611 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/check_types.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8461 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/check_types_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/fake_experiment.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3627 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/no_custom_objects.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5864 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/_src/validation/no_custom_objects_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1143 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/absl_flags/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/absl_flags/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/absl_flags/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/absl_flags/example/business_logic.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/absl_flags/example/configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/absl_flags/example/example.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/absl_flags/example/tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/building.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1352 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/codegen/codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1056 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2165 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/diffing.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/examples/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/examples/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.599339 fiddle-0.3.0/fiddle/examples/colabs/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/examples/colabs/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.603339 fiddle-0.3.0/fiddle/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1719 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/auto_config_policy.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.603339 fiddle-0.3.0/fiddle/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      854 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/lazy_imports.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/experimental/yaml_serialization.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.603339 fiddle-0.3.0/fiddle/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      823 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/extensions/numpy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      863 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/tagging.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.603339 fiddle-0.3.0/fiddle/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/testing/autotest.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      935 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/validation.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2024-04-09 00:14:27.000000 fiddle-0.3.0/fiddle/version.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2024-04-09 00:15:23.575339 fiddle-0.3.0/fiddle.egg-info/
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1705 2024-04-09 00:15:23.000000 fiddle-0.3.0/fiddle.egg-info/PKG-INFO
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     7920 2024-04-09 00:15:23.000000 fiddle-0.3.0/fiddle.egg-info/SOURCES.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2024-04-09 00:15:23.000000 fiddle-0.3.0/fiddle.egg-info/dependency_links.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)      179 2024-04-09 00:15:23.000000 fiddle-0.3.0/fiddle.egg-info/requires.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2024-04-09 00:15:23.000000 fiddle-0.3.0/fiddle.egg-info/top_level.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2024-04-09 00:15:23.603339 fiddle-0.3.0/setup.cfg
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3805 2024-04-09 00:14:27.000000 fiddle-0.3.0/setup.py
```

### Comparing `fiddle-0.2.9/LICENSE` & `fiddle-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/PKG-INFO` & `fiddle-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.9
+Version: 0.3.0
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
@@ -14,20 +14,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: flags
 Provides-Extra: testing
 License-File: LICENSE
 
 
 # Fiddle
```

### Comparing `fiddle-0.2.9/README.md` & `fiddle-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/__init__.py` & `fiddle-0.3.0/fiddle/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,29 +12,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Init file for the `fiddle` package."""
 
 from fiddle._src.building import build
-from fiddle._src.config import add_tag
-from fiddle._src.config import ArgFactory
-from fiddle._src.config import assign
+from fiddle._src.casting import cast
 from fiddle._src.config import Buildable
-from fiddle._src.config import cast
-from fiddle._src.config import clear_tags
 from fiddle._src.config import Config
-from fiddle._src.config import copy_with
-from fiddle._src.config import deepcopy_with
 from fiddle._src.config import get_callable
-from fiddle._src.config import get_tags
 from fiddle._src.config import NO_VALUE
 from fiddle._src.config import ordered_arguments
-from fiddle._src.config import Partial
-from fiddle._src.config import remove_tag
-from fiddle._src.config import set_tags
-from fiddle._src.config import update_callable
+from fiddle._src.copying import copy_with
+from fiddle._src.copying import deepcopy_with
 from fiddle._src.materialize import materialize_defaults
+from fiddle._src.mutate_buildable import assign
+from fiddle._src.mutate_buildable import update_callable
+from fiddle._src.partial import ArgFactory
+from fiddle._src.partial import Partial
+from fiddle._src.signatures import VARARGS
+from fiddle._src.tagging import add_tag
+from fiddle._src.tagging import clear_tags
+from fiddle._src.tagging import get_tags
+from fiddle._src.tagging import remove_tag
 from fiddle._src.tagging import set_tagged
+from fiddle._src.tagging import set_tags
 from fiddle._src.tagging import Tag
 from fiddle._src.tagging import TaggedValue
 from fiddle.version import __version__
```

### Comparing `fiddle-0.2.9/fiddle/_src/__init__.py` & `fiddle-0.3.0/fiddle/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/absl_flags/__init__.py` & `fiddle-0.3.0/fiddle/_src/absl_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/absl_flags/flags.py` & `fiddle-0.3.0/fiddle/codegen/codegen_diff.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,18 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""API to use command line flags with Fiddle Buildables."""
+"""Library for converting generating fiddlers from diffs."""
 
-from fiddle._src.absl_flags import legacy_flags
-
-# Legacy API
-apply_fiddlers_to = legacy_flags.apply_fiddlers_to
-apply_overrides_to = legacy_flags.apply_overrides_to
-create_buildable_from_flags = legacy_flags.create_buildable_from_flags
-flags_parser = legacy_flags.flags_parser
-rewrite_fdl_args = legacy_flags.rewrite_fdl_args
-fdl_flags_supplied = legacy_flags.fdl_flags_supplied
+# pylint: disable=unused-import
+from fiddle._src.codegen.codegen_diff import fiddler_from_diff
```

### Comparing `fiddle-0.2.9/fiddle/_src/absl_flags/legacy_flags.py` & `fiddle-0.3.0/fiddle/_src/absl_flags/legacy_flags.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Legacy API to use command line flags with Fiddle Buildables.
 
+NOTE: Deprecation: These are legacy APIs. Please refer to the new API usage in
+flags.py and find the documentation in flags_code_lab.md.
+
 While it's generally better to check in the full configuration into a source-
 control system, there are some instances (e.g. hyperparameter sweeps) where it's
 most effective to set initialization parameters (hyperparameters) from command
 line flags. This library exposes functions you can call within your program.
 
 NOTE: The flags aren't applied in the order they are passed in on the command
   line. The order followed is:
@@ -114,26 +117,23 @@
 [T5X](https://github.com/google-research/t5x), among others. Thank you!
 """
 
 import inspect
 import re
 import sys
 import textwrap
-import typing
 from typing import Any, List, Optional, Sequence
 
 from absl import app
 from absl import flags
 from absl import logging
 from etils import epath
 from fiddle import printing
 from fiddle import selectors
 from fiddle._src import config
-from fiddle._src import daglish
-from fiddle._src import module_reflection
 from fiddle._src import tagging
 from fiddle._src.absl_flags import utils
 from fiddle._src.experimental import auto_config
 from fiddle._src.experimental import serialization
 
 
 _FDL_CONFIG = flags.DEFINE_string(
@@ -170,35 +170,24 @@
 
 
 def _print_stderr(*args, **kwargs):
   print(*args, **kwargs, file=sys.stderr)
 
 
 def apply_overrides_to(cfg: config.Buildable):
-  """Applies all command line flags to `cfg`."""
+  """[DEPRECATED] Applies all command line flags to `cfg`.
+
+  Deprecation: This is a legacy API. Please refer to the new API usage in
+  flags.py and find the documentation in flags_code_lab.md.
+
+  Args:
+    cfg: The configuration to apply overrides to.
+  """
   for flag in _FDL_SET.value:
-    path, value = flag.split('=', maxsplit=1)
-    *parents, last = utils.parse_path(path)
-    walk = typing.cast(Any, cfg)
-    try:
-      for parent in parents:
-        walk = parent.follow(walk)
-    except Exception as e:
-      raise ValueError(f'Invalid path "{path}".') from e
-
-    literal_value = utils.parse_value(value=value, path=path)
-    try:
-      if isinstance(last, daglish.Attr):
-        setattr(walk, last.name, literal_value)
-      elif isinstance(last, daglish.Key):
-        walk[last.key] = literal_value
-      else:
-        raise ValueError(f'Unexpected path element {last}.')
-    except Exception as e:
-      raise ValueError(f'Could not set "{path}" to "{value}".') from e
+    utils.set_value(cfg, flag)
 
 
 def rewrite_fdl_args(args: Sequence[str]) -> List[str]:
   """Rewrites short-form Fiddle flags.
 
   There are two main rewrites:
 
@@ -245,15 +234,26 @@
   Returns:
     Whatever `absl.app.parse_flags_with_usage` returns. Sorry!
   """
   return app.parse_flags_with_usage(rewrite_fdl_args(args))
 
 
 def set_tags(cfg: config.Buildable):
-  """Sets tags based on their name, from CLI flags."""
+  """[DEPRECATED] Sets tags based on their name, from CLI flags.
+
+  Deprecation: This is a legacy API. Please refer to the new API usage in
+  flags.py and find the documentation in flags_code_lab.md.
+
+  Args:
+    cfg: The configuration to set tags on.
+
+  Raises:
+    ValueError: If no tags with the given name are found.
+    EnvironmentError: If multiple tags with the given name are found.
+  """
   all_tags = tagging.list_tags(cfg, add_superclasses=True)
   for flag in _FDL_TAGS_SET.value:
     name, value = flag.split('=', maxsplit=1)
     matching_tags = [tag for tag in all_tags if tag.name == name]
     if not matching_tags:
       # TODO(b/219988937): Improve and unify these errors.
       loose_matches = [
@@ -273,33 +273,35 @@
         value=utils.parse_value(value=value, path=str(matching_tags[0]))
     )
 
 
 def apply_fiddlers_to(cfg: config.Buildable,
                       source_module: Any,
                       allow_imports=False):
-  """Applies fiddlers to `cfg`."""
+  """[DEPRECATED] Applies fiddlers to `cfg`.
+
+  Deprecation: This is a legacy API. Please refer to the new API usage in
+  flags.py and find the documentation in flags_code_lab.md.
+
+  Args:
+    cfg: The configuration to apply fiddlers to.
+    source_module: source py module where fiddlers are defined.
+    allow_imports: If true, then fully qualified dotted names may be used to
+      specify configs or fiddlers that should be automatically imported.
+  """
   for fiddler_value in _FIDDLER.value:
     call_expr = utils.CallExpression.parse(fiddler_value)
     fiddler_name = call_expr.func_name
-    if hasattr(source_module, fiddler_name):
-      fiddler = getattr(source_module, fiddler_name)
-    elif allow_imports:
-      try:
-        fiddler = utils.import_dotted_name(
-            fiddler_name, mode=utils.ImportDottedNameDebugContext.FIDDLER
-        )
-      except ModuleNotFoundError as e:
-        raise ValueError(f'Could not load fiddler {fiddler_name!r}: {e}') from e
-    else:
-      available_fiddlers = ', '.join(
-          module_reflection.find_fiddler_like_things(source_module))
-      raise ValueError(
-          f'No fiddler named {fiddler_name!r} found; available fiddlers: '
-          f'{available_fiddlers}.')
+    fiddler = utils.resolve_function_reference(
+        fiddler_name,
+        utils.ImportDottedNameDebugContext.FIDDLER,
+        source_module,
+        allow_imports,
+        'Could not load fiddler',
+    )
     fiddler(cfg, *call_expr.args, **call_expr.kwargs)
 
 
 def _print_help(module, allow_imports):
   """Prints flag help, including available symbols in `module`."""
   flags_help_text = flags.FLAGS.module_help(sys.modules[__name__])
   flags_help_text = '\n'.join(flags_help_text.splitlines()[2:])
@@ -340,15 +342,18 @@
 
 
 def create_buildable_from_flags(
     module: Optional[Any],
     allow_imports=False,
     pyref_policy: Optional[serialization.PyrefPolicy] = None,
 ) -> config.Buildable:
-  """Returns a fdl.Buildable based on standardized flags.
+  """[DEPRECATED] Returns a fdl.Buildable based on standardized flags.
+
+  Deprecation: This is a legacy API. Please refer to the new API usage in
+  flags.py and find the documentation in flags_code_lab.md.
 
   NOTE: the flags aren't applied in the order they are passed in on the command
   line. The order followed is:
   - all fiddlers are applied first, followed by
   - all tags, followed by
   - all overrides.
 
@@ -357,14 +362,17 @@
       fiddlers. May be `None`; if `None`, only fully qualified Fiddler imports
       will be used (or alternatively a base configuration can be specified using
       the `--fdl_config_file` flag.)
     allow_imports: If true, then fully qualified dotted names may be used to
       specify configs or fiddlers that should be automatically imported.
     pyref_policy: An optional `serialization.PyrefPolicy` to use if parsing a
       serialized Fiddle config (passed via `--fdl_config_file`).
+
+  Returns:
+    A `fdl.Buildable` based on standardized flags.
   """
   missing_base_config = not _FDL_CONFIG.value and not _FDL_CONFIG_FILE.value
   if not _FDL_HELP.value and missing_base_config:
     raise app.UsageError(
         'At least one of --fdl_config or --fdl_config_file is required.')
   elif _FDL_CONFIG.value and _FDL_CONFIG_FILE.value:
     raise app.UsageError(
@@ -384,29 +392,22 @@
       raise ValueError(err_msg.format(flag='--fdl_config'))
     if _FIDDLER.value:
       raise ValueError(err_msg.format(flag='--fiddler'))
 
   if _FDL_CONFIG.value:
     call_expr = utils.CallExpression.parse(_FDL_CONFIG.value)
     base_name = call_expr.func_name
-    if hasattr(module, base_name):
-      base_fn = getattr(module, base_name)
-    elif allow_imports:
-      try:
-        base_fn = utils.import_dotted_name(
-            base_name,
-            mode=utils.ImportDottedNameDebugContext.BASE_CONFIG,
-        )
-      except ModuleNotFoundError as e:
-        raise ValueError(
-            f'Could not init a buildable from {base_name!r}: {e}') from e
-    else:
-      available_names = module_reflection.find_base_config_like_things(module)
-      raise ValueError(f'Could not init a buildable from {base_name!r}; '
-                       f'available names: {", ".join(available_names)}.')
+
+    base_fn = utils.resolve_function_reference(
+        base_name,
+        utils.ImportDottedNameDebugContext.BASE_CONFIG,
+        module,
+        allow_imports,
+        'Could not init a buildable from',
+    )
 
     if auto_config.is_auto_config(base_fn):
       buildable = base_fn.as_buildable(*call_expr.args, **call_expr.kwargs)
     else:
       buildable = base_fn(*call_expr.args, **call_expr.kwargs)
   elif _FDL_CONFIG_FILE.value:
     with _FDL_CONFIG_FILE.value.open() as f:
```

### Comparing `fiddle-0.2.9/fiddle/_src/absl_flags/sample_module_for_flags_test.py` & `fiddle-0.3.0/fiddle/_src/absl_flags/sample_module_for_flags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/absl_flags/utils.py` & `fiddle-0.3.0/fiddle/_src/absl_flags/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utilities to use command line flags with Fiddle Buildables."""
 
 import ast
+import base64
 import dataclasses
 import enum
 import importlib
 import re
+import types
+import typing
 from typing import Any, Dict, Optional, Tuple
+import zlib
 
+from fiddle._src import config
 from fiddle._src import daglish
 from fiddle._src import daglish_extensions
+from fiddle._src import module_reflection
+from fiddle._src.experimental import serialization
 
 
 class ImportDottedNameDebugContext(enum.Enum):
   """Context of importing a sumbol, for error messages."""
 
   BASE_CONFIG = 1
   FIDDLER = 2
@@ -195,7 +202,102 @@
   except Exception as e:
     raise ValueError(
         f'Could not parse literal value "{value}" while trying to set '
         f'"{path}". Does a string need to be quoted? For example, you might '
         f"want to pass --fdl_set={path}='{value}' instead of "
         f'--fdl_set={path}={value}.'
     ) from e
+
+
+def resolve_function_reference(
+    function_name: str,
+    mode: ImportDottedNameDebugContext,
+    module: Optional[types.ModuleType],
+    allow_imports: bool,
+    failure_msg_prefix: str,
+):
+  """Returns function that produces `fdl.Buildable` from its name.
+
+  Args:
+    function_name: The name of the function.
+    mode: Whether we're looking for a base config function or a fiddler.
+    module: A common namespace to use as the basis for finding configs and
+      fiddlers. May be `None`; if `None`, only fully qualified Fiddler imports
+      will be used (or alternatively a base configuration can be specified using
+      the `--fdl_config_file` flag.)
+    allow_imports: If true, then fully qualified dotted names may be used to
+      specify configs or fiddlers that should be automatically imported.
+    failure_msg_prefix: Prefix string to prefix log messages in case of
+      failures.
+
+  Returns:
+    The named value.
+  """
+  if hasattr(module, function_name):
+    return getattr(module, function_name)
+  elif allow_imports:
+    try:
+      return import_dotted_name(
+          function_name,
+          mode=mode,
+      )
+    except ModuleNotFoundError as e:
+      raise ValueError(f'{failure_msg_prefix} {function_name!r}: {e}') from e
+  else:
+    available_names = module_reflection.find_base_config_like_things(module)
+    raise ValueError(
+        f'{failure_msg_prefix} {function_name!r}; '
+        f'available names: {", ".join(available_names)}.'
+    )
+
+
+def set_value(cfg: config.Buildable, assignment: str) -> None:
+  """Set an attribute's value.
+
+  Args:
+    cfg: A `fdl.Buildable` whose attribute is to be overridden.
+    assignment: String representing attribute's override expression. Of the form
+      `attribute=value`.
+  """
+  path, value = assignment.split('=', maxsplit=1)
+  *parents, last = parse_path(path)
+
+  walk = typing.cast(Any, cfg)
+  try:
+    for parent in parents:
+      walk = parent.follow(walk)
+  except Exception as e:
+    raise ValueError(f'Invalid path "{path}".') from e
+
+  literal_value = parse_value(value=value, path=path)
+  try:
+    if isinstance(last, daglish.Attr):
+      setattr(walk, last.name, literal_value)
+    elif isinstance(last, daglish.Key):
+      walk[last.key] = literal_value
+    else:
+      raise ValueError(f'Unexpected path element {last}.')
+  except Exception as e:
+    raise ValueError(f'Could not set "{path}" to "{value}".') from e
+
+
+class ZlibJSONSerializer:
+  """Serializer that uses JSON, zlib, and base64 encoding."""
+
+  def serialize(
+      self,
+      cfg: config.Buildable,
+      pyref_policy: Optional[serialization.PyrefPolicy] = None,
+  ) -> str:
+    return base64.urlsafe_b64encode(
+        zlib.compress(serialization.dump_json(cfg, pyref_policy).encode())
+    ).decode('ascii')
+
+  def deserialize(
+      self,
+      serialized: str,
+      pyref_policy: Optional[serialization.PyrefPolicy] = None,
+  ) -> config.Buildable:
+    return serialization.load_json(
+        zlib.decompress(base64.urlsafe_b64decode(serialized)).decode(),
+        pyref_policy=pyref_policy,
+    )
```

### Comparing `fiddle-0.2.9/fiddle/_src/arg_factory.py` & `fiddle-0.3.0/fiddle/_src/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/arg_factory_test.py` & `fiddle-0.3.0/fiddle/_src/arg_factory_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/building.py` & `fiddle-0.3.0/fiddle/_src/building.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 """Implements Fiddle's build() function."""
 
 import contextlib
 import functools
 import logging
 import threading
-from typing import Any, Callable, Dict, TypeVar, overload
+from typing import Any, Callable, Dict, Sequence, TypeVar, Union, overload
 
 from fiddle._src import config as config_lib
 from fiddle._src import daglish
+from fiddle._src import partial
 from fiddle._src import reraised_exception
 
 T = TypeVar('T')
 
 
 class _BuildGuardState(threading.local):
 
@@ -55,63 +56,77 @@
   """Returns repr(arg), returning a constant string if repr() fails."""
   try:
     return repr(arg)
   except Exception:  # pylint: disable=broad-except
     return f'<ERROR FORMATTING {type(arg)} ARGUMENT>'
 
 
-def _make_message(current_path: daglish.Path, buildable: config_lib.Buildable,
-                  arguments: Dict[str, Any]) -> str:
+def _make_message(
+    current_path: daglish.Path,
+    buildable: config_lib.Buildable,
+    args: Sequence[Any],
+    kwargs: Dict[str, Any],
+) -> str:
   """Returns Fiddle-related debugging information for an exception."""
   path_str = '<root>' + daglish.path_str(current_path)
   fn_or_cls = config_lib.get_callable(buildable)
   try:
     fn_or_cls_name = fn_or_cls.__qualname__
   except AttributeError:
     fn_or_cls_name = str(fn_or_cls)  # callable instances, etc.
+  args_str = ', '.join(f'{_format_arg(value)}' for value in args)
   kwargs_str = ', '.join(
-      f'{name}={_format_arg(value)}' for name, value in arguments.items())
+      f'{name}={_format_arg(value)}' for name, value in kwargs.items()
+  )
 
   tag_information = ''
-  bound_args = buildable.__signature__.bind_partial(**arguments)
+  bound_args = buildable.__signature_info__.signature.bind_partial(
+      *args, **kwargs
+  )
   bound_args.apply_defaults()
   unset_arg_tags = []
-  for param in buildable.__signature__.parameters:
+  for param in buildable.__signature_info__.parameters:
     if param in bound_args.arguments:
       continue  # User supplied it, all good.
     tags = buildable.__argument_tags__.get(param, None)
     if tags:
       tag_str = ' '.join(sorted(str(tag) for tag in tags))
       unset_arg_tags.append(f' - {param}: {tag_str}')
   if unset_arg_tags:
     tag_details = '\n'.join(unset_arg_tags)
     tag_information = f'\nTags for unset arguments:\n{tag_details}'
 
   return (
       '\n\nFiddle context: failed to construct or call '
       f'{fn_or_cls_name} at {path_str} '
-      f'with arguments ({kwargs_str}){tag_information}'
+      f'with positional arguments: ({args_str}), '
+      f'keyword arguments: ({kwargs_str}){tag_information}.'
   )
 
 
 def call_buildable(
     buildable: config_lib.Buildable,
-    arguments: Dict[str, Any],
+    arguments: Dict[Union[str, int], Any],
     *,
     current_path: daglish.Path,
 ) -> Any:
-  make_message = functools.partial(_make_message, current_path, buildable,
-                                   arguments)
+  """Prepare positional arguments and actually build the buildable."""
+  args, kwargs = buildable.__signature_info__.transform_to_args_kwargs(
+      arguments
+  )
+  make_message = functools.partial(
+      _make_message, current_path, buildable, args, kwargs
+  )
   with reraised_exception.try_with_lazy_message(make_message):
-    return buildable.__build__(**arguments)
+    return buildable.__build__(*args, **kwargs)
 
 
 # Define typing overload for `build(Partial[T])`
 @overload
-def build(buildable: config_lib.Partial[T]) -> Callable[..., T]:
+def build(buildable: partial.Partial[T]) -> Callable[..., T]:
   ...
 
 
 # Define typing overload for `build(Config[T])`
 @overload
 def build(buildable: config_lib.Config[T]) -> T:
   ...
```

### Comparing `fiddle-0.2.9/fiddle/_src/building_test.py` & `fiddle-0.3.0/fiddle/_src/building_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/__init__.py` & `fiddle-0.3.0/fiddle/_src/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/__init__.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/code_ir.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,19 @@
 
 @dataclasses.dataclass
 class ModuleReference(BaseNameReference):
   """Reference to an imported module."""
 
 
 @dataclasses.dataclass
+class BuiltinReference(BaseNameReference):
+  """Reference to an imported module."""
+
+
+@dataclasses.dataclass
 class FixtureReference(BaseNameReference):
   """Reference to another fixture."""
 
 
 @dataclasses.dataclass
 class AttributeExpression(CodegenNode):
   """Reference to an attribute of another expression."""
@@ -126,14 +131,22 @@
     # having AttributeExpression's as dict keys, as those keys are rewritten to
     # expressions. This function allows for that, but one shouldn't generally
     # assume equality as object identity here.
     return id(self)
 
 
 @dataclasses.dataclass
+class ParameterizedTypeExpression(CodegenNode):
+  """Reference to a parameterized type like list[int]."""
+
+  base_expression: Any  # Expression like BuiltinReference(Name("list"))
+  param_expressions: List[Any]  # List of (positional) argument expressions
+
+
+@dataclasses.dataclass
 class ArgFactoryExpr(CodegenNode):
   """Represents a factory that should be interpreted as an argument factory.
 
   Inside Fiddle configs, we represent arg factories with fdl.ArgFactory, e.g.
 
   attention=fdl.ArgFactory(
     initializer=fdl.ArgFactory(nn.initializers.zeros, dtype='float16')
@@ -208,14 +221,15 @@
   in a `return` statement.
   """
 
   name: Name
   parameters: List[Parameter]
   variables: List[VariableDeclaration]
   output_value: Any  # Value that can involve VariableReference's
+  return_type_annotation: Optional[Any] = None
 
   def __hash__(self):
     return id(self)
 
   def replace_with(self, other: FixtureFunction) -> None:
     self.name = other.name
     self.parameters = other.parameters
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/code_ir_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/code_ir_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         [
             ("", fn),
             (".name", fn.name),
             (".parameters", []),
             (".variables", []),
             (".output_value", fn.output_value),
             (".output_value.x", 2),
+            (".return_type_annotation", None),
         ],
     )
 
   @parameterized.named_parameters(test_fixtures.parameters_for_testcases())
   def test_smoke_traverse_fixtures(self, task: code_ir.CodegenTask):
     functions = task.top_level_call.all_fixture_functions()
     self.assertNotEmpty(functions)
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/complex_to_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
       # Names don't count towards node complexity. Usually they are sub-fields
       # of another node (like code_ir.VariableReference), where the container
       # has already incremented the complexity.
       return 0
     elif not state.is_traversable(value):
       return 1
     else:
-      sub_values = state.flattened_map_children(value)
-      return 1 + sum(sub_values.values)
+      return 1 + sum(state.yield_map_child_values(value))
 
   return lambda x: daglish.MemoizedTraversal.run(traverse, x) > level
 
 
 def move_complex_nodes_to_variables(
     task: code_ir.CodegenTask,
     *,
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/complex_to_variables_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/complex_to_variables_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/experimental_top_level_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,18 @@
   )
 
 
 @dataclasses.dataclass(frozen=True)
 class IrToCst(CodegenPass):
   """Converts a codegen IR task to a LibCST module."""
 
+  def print_debug(self, value: Any) -> None:
+    # This pass doesn't print debug information.
+    pass
+
   def __call__(self, value: Any) -> Any:
     return ir_to_cst.code_for_task(value)
 
 
 @auto_config.auto_config(experimental_allow_control_flow=True)
 def code_generator(
     top_level_fixture_name: str = "config_fixture",
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import dataclasses
 import importlib
 import os
 import random
 import re
 import sys
 import types
+from unittest import mock
 import uuid
 
 from absl import flags
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import daglish
@@ -115,14 +116,18 @@
           "testcase_name": "all_variables",
           "kwargs": {"max_expression_complexity": 1},
       },
       {
           "testcase_name": "with_history",
           "kwargs": {"include_history": True},
       },
+      {
+          "testcase_name": "debug_print",
+          "kwargs": {"debug_print": True},
+      },
   ])
   def test_fuzz(self, kwargs):
     # TODO(b/272826193): Test on more RNG seeds.
     for i in range(10):
       config = tagging.materialize_tags(
           nested_values.generate_nested_value(random.Random(i))
       )
@@ -130,17 +135,22 @@
       has_buildables = any(
           isinstance(value, fdl.Buildable)
           for value, _ in daglish.iterate(config)
       )
       if has_buildables:
         with self.subTest(f"rng_{i}"):
           sub_fixtures = create_random_sub_fixture(config, random.Random(i))
-          code = experimental_top_level_api.auto_config_codegen(
-              config, sub_fixtures=sub_fixtures, **kwargs
-          )
+          with mock.patch.object(
+              experimental_top_level_api,
+              "print",
+              mock.create_autospec(print),
+          ):
+            code = experimental_top_level_api.auto_config_codegen(
+                config, sub_fixtures=sub_fixtures, **kwargs
+            )
           module = self._load_code_as_module(code)
           generated_config = module.config_fixture.as_buildable()
           self.assertDagEqual(config, generated_config)
 
   def test_config_contains_tags_wo_default(self):
     @dataclasses.dataclass
     class Foo:
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/get_history_comments.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/get_history_comments_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/get_history_comments_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/init_task.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/init_task_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/init_task_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_printer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Values from the `typing` module. This probably pulls in too much stuff, but
 # we don't have to be 100% precise in this module, it's just for debug printing.
 typing_consts = [getattr(typing, name) for name in dir(typing)]
 
 
 def format_py_reference(value: Any) -> str:
   module_name = inspect.getmodule(value).__name__
-  if module_name == "fiddle._src.config":
+  if module_name in ("fiddle._src.config", "fiddle._src.partial"):
     module_name = "fdl"
   cls_name = value.__qualname__
   return f"{module_name}.{cls_name}"
 
 
 def format_expr(expr: Any):
   """Formats an expression, which may contain other IR nodes.
@@ -86,16 +86,17 @@
     elif isinstance(value, code_ir.AttributeExpression):
       base_obj = state.call(value.base, daglish.Attr("base"))
       return f"{base_obj}.{value.attribute}"
     elif isinstance(value, code_ir.ArgFactoryExpr):
       sub_value = state.map_children(value).expression
       return f"ArgFactoryExpr[{sub_value}]"
     elif isinstance(value, code_ir.WithTagsCall):
-      sub_value = state.map_children(value).expression
-      return f"WithTagsCall[{sub_value}]"
+      tags_str = ", ".join(value.tag_symbol_expressions)
+      sub_value = state.map_children(value.item_to_tag)
+      return f"WithTagsCall[{tags_str}]({sub_value})"
     elif isinstance(value, code_ir.SymbolOrFixtureCall):
       symbol_expression = state.call(
           value.symbol_expression, daglish.Attr("symbol_expression")
       )
       positional_arg_expressions = state.call(
           value.positional_arg_expressions,
           daglish.Attr("positional_arg_expressions"),
@@ -104,17 +105,25 @@
           value.arg_expressions, daglish.Attr("arg_expressions")
       )
       return (
           f"call:<{symbol_expression}"
           f"(*[{positional_arg_expressions}],"
           f" **{arg_expressions})>"
       )
+    elif isinstance(value, code_ir.ParameterizedTypeExpression):
+      base_expression = state.call(
+          value.base_expression, daglish.Attr("base_expression")
+      )
+      param_expressions = state.call(
+          value.param_expressions, daglish.Attr("param_expressions")
+      )
+      return f"{base_expression}{param_expressions}"
     elif isinstance(value, code_ir.Name):
       return value.value
-    elif isinstance(value, type):
+    elif isinstance(value, type) and value is not typing.Any:
       return value.__name__
     elif value in typing_consts or type(value) in typing_consts:
       return str(value)
     else:
       return f"<<<custom:{repr(value)}>>>"
 
   return daglish.MemoizedTraversal.run(traverse, expr)
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_printer_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_printer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,20 @@
 
     self_var = code_ir.VariableReference(
         code_ir.Name("self", is_generated=True)
     )
     attr = code_ir.AttributeExpression(self_var, "foo")
     self.assertEqual(ir_printer.format_expr(attr), "self.foo")
 
+  def test_format_with_tags(self):
+    with_tags = code_ir.WithTagsCall(["module.Tag"], item_to_tag=123.4)
+    self.assertEqual(
+        ir_printer.format_expr(with_tags), "WithTagsCall[module.Tag](123.4)"
+    )
+
   def test_format_calls(self):
     call = code_ir.SymbolOrFixtureCall(
         symbol_expression=code_ir.Name("foo"),
         positional_arg_expressions=[code_ir.Name("bar")],
         arg_expressions={"baz": code_ir.Name("qux")},
     )
     self.assertEqual(
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_to_cst.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Converts from the auto_config codegen representation to LibCST nodes.
 
 Note: We do not generally do a lot of formatting, instead relying on existing
 source code formatters (pyformat, yapf, etc.).
 """
 
-from typing import Any, List, Optional
+from typing import Any, List, Optional, Union
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen import py_val_to_cst_converter
 from fiddle._src.codegen.auto_config import code_ir
 import libcst as cst
 
@@ -37,74 +37,109 @@
   Returns:
     CST node for expression.
   """
 
   def traverse(value, state: daglish.State) -> cst.CSTNode:
 
     def _prepare_args_helper(
-        names: List[str],
+        names: List[Union[str, int]],
         values: List[Any],
         attr: daglish.Attr,
         *,
         history: Optional[code_ir.HistoryComments] = None,
     ) -> List[cst.Arg]:
       """Prepare code_ir.Arg node based on names and values."""
-      args = []
+      cst_args = {}
+      cst_kwargs = []
       for arg_name, arg_value in zip(names, values):
-        assert isinstance(arg_name, str)
+        if not isinstance(arg_name, (int, str)):
+          raise TypeError(
+              f"Unsupported arg name type: {type(arg_name)} (value: {arg_name})"
+          )
         arg_value = state.call(arg_value, attr, daglish.Key(arg_name))
         kwargs = {}
         if history and arg_name in history.per_field:
           kwargs["comma"] = cst.Comma(
               whitespace_after=cst.ParenthesizedWhitespace(
                   first_line=cst.TrailingWhitespace(
                       whitespace=cst.SimpleWhitespace("  "),
                       comment=cst.Comment(f"# {history.per_field[arg_name]}"),
                       newline=cst.Newline(),
                   ),
                   last_line=cst.SimpleWhitespace(" " * 6),
               )
           )
-        args.append(
-            cst.Arg(
-                arg_value,
-                keyword=cst.Name(arg_name),
-                equal=cst.AssignEqual(
-                    whitespace_before=cst.SimpleWhitespace(""),
-                    whitespace_after=cst.SimpleWhitespace(""),
-                ),
-                **kwargs,
-            )
+        if isinstance(arg_name, str):
+          cst_kwargs.append(
+              cst.Arg(
+                  arg_value,
+                  keyword=cst.Name(arg_name),
+                  equal=cst.AssignEqual(
+                      whitespace_before=cst.SimpleWhitespace(""),
+                      whitespace_after=cst.SimpleWhitespace(""),
+                  ),
+                  **kwargs,
+              )
+          )
+        elif isinstance(arg_name, int):
+          if arg_name in cst_args:
+            raise ValueError(f"Duplicate positional arg: {arg_name}")
+          cst_args[arg_name] = cst.Arg(arg_value, **kwargs)
+
+      positional_arg_keys = set(cst_args.keys())
+      if positional_arg_keys != set(range(len(positional_arg_keys))):
+        raise ValueError(
+            "Positional args supplied were not contiguous! "
+            f"Got {positional_arg_keys}"
         )
-      return args
+      return [value for _, value in sorted(cst_args.items())] + cst_kwargs
 
     if isinstance(value, config_lib.Buildable):
       raise ValueError(
           "Internal Fiddle error: you must run the make_symbolic_references "
           "passes before CST generation."
       )
     elif isinstance(value, (list, tuple)):
+      original = value
       value = state.map_children(value)
       if isinstance(value, list):
         cst_cls = cst.List
       else:
         cst_cls = cst.Tuple
-      return cst_cls([cst.Element(elt) for elt in value])
+      elements = []
+      for sub_value in value:
+        if not isinstance(sub_value, cst.CSTNode):
+          raise TypeError(
+              f"Failed to map children of {original!r}, this might be because "
+              f"{type(original)} subclasses list or tuple. If this is the case,"
+              " please replace these objects in your input config, likely "
+              "with fdl.Config nodes."
+          )
+        elements.append(cst.Element(sub_value))
+      return cst_cls(elements)
     elif isinstance(value, dict):
       elements = []
       for key, sub_value in value.items():
         key_node = state.call(key, daglish.Key(f"__key_{key}"))
         sub_value_node = state.call(sub_value, daglish.Attr(key))
         elements.append(cst.DictElement(key_node, sub_value_node))
       return cst.Dict(elements)
     elif isinstance(value, code_ir.BaseNameReference):
       return cst.Name(value.name.value)
     elif isinstance(value, code_ir.AttributeExpression):
       base = state.call(value.base, daglish.Attr("base"))
       return cst.Attribute(value=base, attr=cst.Name(value.attribute))
+    elif isinstance(value, code_ir.ParameterizedTypeExpression):
+      return cst.Subscript(
+          value=code_for_expr(value.base_expression),
+          slice=[
+              cst.SubscriptElement(cst.Index(code_for_expr(param)))
+              for param in value.param_expressions
+          ],
+      )
     elif isinstance(value, code_ir.SymbolOrFixtureCall):
       attr = daglish.Attr("arg_expressions")
       args = []
       for i, arg_value in enumerate(value.positional_arg_expressions):
         arg_value = state.call(arg_value, attr, daglish.Key(i))
         args.append(cst.Arg(arg_value))
 
@@ -195,26 +230,33 @@
       body=[
           *variable_lines,
           cst.SimpleStatementLine(
               body=[cst.Return(code_for_expr(fn.output_value))]
           ),
       ]
   )
+  if fn.return_type_annotation:
+    returns = cst.Annotation(
+        annotation=code_for_expr(fn.return_type_annotation)
+    )
+  else:
+    returns = None
   if fn.parameters and len(fn.parameters) > 1:
     whitespace_before_params = cst.ParenthesizedWhitespace(
         cst.TrailingWhitespace(),
         indent=True,
         last_line=cst.SimpleWhitespace("  "),
     )
   else:
     whitespace_before_params = cst.SimpleWhitespace("")
   return cst.FunctionDef(
       cst.Name(fn.name.value),
       params,
       body,
+      returns=returns,
       decorators=[cst.Decorator(auto_config_expr)] if auto_config_expr else [],
       whitespace_before_params=whitespace_before_params,
       leading_lines=[cst.EmptyLine(), cst.EmptyLine()],
   )
 
 
 def code_for_task(
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/ir_to_cst_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/ir_to_cst_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import get_history_comments
 from fiddle._src.codegen.auto_config import init_task
 from fiddle._src.codegen.auto_config import ir_to_cst
 from fiddle._src.codegen.auto_config import make_symbolic_references
 from fiddle._src.codegen.auto_config import shared_to_variables
 from fiddle._src.codegen.auto_config import test_fixtures
+import jax.sharding
 import libcst as cst
 
 
 def _code_for_expr(node: cst.CSTNode) -> str:
   """Returns Python code for a CST node.
 
   This assumes two spaces of indentation. It is helpful because we CST nodes
@@ -58,14 +59,36 @@
     call = code_ir.SymbolOrFixtureCall(
         attr, [], {"bar": code_ir.AttributeExpression(self_var, "bar")}
     )
     self.assertEqual(
         _code_for_expr(ir_to_cst.code_for_expr(call)), "self.foo(bar=self.bar)"
     )
 
+  def test_code_for_positional_arg_call(self):
+    self_var = code_ir.VariableReference(
+        code_ir.Name("self", is_generated=True)
+    )
+    attr = code_ir.AttributeExpression(self_var, "foo")
+    call = code_ir.SymbolOrFixtureCall(
+        attr, [123.4], {"bar": code_ir.AttributeExpression(self_var, "bar")}
+    )
+    self.assertEqual(
+        _code_for_expr(ir_to_cst.code_for_expr(call)),
+        "self.foo(123.4, bar=self.bar)",
+    )
+
+  def test_code_for_expr_jax_partition_spec(self):
+    """This is a very weird overridden tuple."""
+    value = jax.sharding.PartitionSpec("data")
+    with self.assertRaisesRegex(
+        TypeError,
+        r"Failed to map.*PartitionSpec.*subclasses list or tuple.*",
+    ):
+      ir_to_cst.code_for_expr(value)
+
   def test_basic_ir(self):
     task = test_fixtures.simple_ir()
     make_symbolic_references.import_symbols(task)
     make_symbolic_references.replace_callables_and_configs_with_symbols(task)
     code = ir_to_cst.code_for_task(task).code
     expected = """
     from fiddle._src.codegen.auto_config import test_fixtures
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/make_symbolic_references.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 # limitations under the License.
 
 """Changes callables to symbol references."""
 
 import enum
 import functools
 import inspect
-import typing
 from typing import Any, Callable
 
 from fiddle import arg_factory
 from fiddle import daglish
 from fiddle._src import config as config_lib
+from fiddle._src import partial
 from fiddle._src.codegen.auto_config import code_ir
+from fiddle._src.codegen.auto_config import import_manager_wrapper
 
 
 def is_plain_symbol_or_enum_value(value: Any) -> bool:
   """Returns whether the value is a plain symbol."""
   if isinstance(value, config_lib.Buildable):
     return False
   elif isinstance(value, type):
@@ -63,24 +64,14 @@
       task.import_manager.add(value)
 
 
 def noop_history_comments(unused_buildable):
   return code_ir.HistoryComments()
 
 
-def _name_to_attribute_expression(name: str) -> code_ir.AttributeExpression:
-  if "." not in name:
-    raise ValueError(f"Could not parse symbol import {name}")
-  base, *parts = name.split(".")
-  value = code_ir.ModuleReference(code_ir.Name(base))
-  for part in parts:
-    value = code_ir.AttributeExpression(value, part)
-  return typing.cast(code_ir.AttributeExpression, value)
-
-
 def replace_callables_and_configs_with_symbols(
     task: code_ir.CodegenTask,
     *,
     format_history: Callable[
         ..., code_ir.HistoryComments
     ] = noop_history_comments,
 ) -> None:
@@ -92,17 +83,17 @@
       get_history_comments.format_history_for_buildable (or a functools.partial
       variant) to populate histories.
   """
 
   fn_name = None
 
   def _handle_partial(
-      value: config_lib.Partial,
+      value: partial.Partial,
       state: daglish.State,
-      ir_for_symbol: code_ir.AttributeExpression,
+      ir_for_symbol: code_ir.CodegenNode,
   ):
     """Split-out helper method to handle Partial() nodes."""
     arguments = config_lib.ordered_arguments(value)
     all_tags = value.__argument_tags__
 
     # Arguments which were config_lib.ArgFactory arguments; these need to be
     # turned into regular calls.
@@ -127,56 +118,50 @@
           dict_of_args[arg] = code_ir.WithTagsCall(
               tag_symbol_expressions=tags_expr,
               item_to_tag=dict_of_args[arg],
           )
 
     def _arg_factory_partial():
       return code_ir.SymbolOrFixtureCall(
-          _name_to_attribute_expression(
-              task.import_manager.add(arg_factory.partial)
-          ),
+          import_manager_wrapper.add(arg_factory.partial, task.import_manager),
           positional_arg_expressions=[ir_for_symbol],
           arg_expressions=arg_factory_args,
           history_comments=format_history(value),
       )
 
     if not arg_factory_args:
       # The common case: there are no arg_factory's, so just emit a functools
       # partial. We currently emit a functools partial even if there are no
       # arguments, because this will mean there's a fdl.Partial when we call
       # the auto_config fixture's as_buildable() method. If we got rid of the
       # functools.partial, then we couldn't configure any attributes.
       return code_ir.SymbolOrFixtureCall(
-          _name_to_attribute_expression(
-              task.import_manager.add(functools.partial)
-          ),
+          import_manager_wrapper.add(functools.partial, task.import_manager),
           positional_arg_expressions=[ir_for_symbol],
           arg_expressions=regular_args,
           history_comments=format_history(value),
       )
     elif not regular_args:
       # There are only arg_factory args, so we can emit an arg_factory.partial.
       return _arg_factory_partial()
     else:
       # We have both functools.partial and arg_factory args. It doesn't matter
       # which order, but we need to emit both decorators. Go with functools
       # on the outer level.
       return code_ir.SymbolOrFixtureCall(
-          _name_to_attribute_expression(
-              task.import_manager.add(functools.partial)
-          ),
+          import_manager_wrapper.add(functools.partial, task.import_manager),
           positional_arg_expressions=[_arg_factory_partial()],
           arg_expressions=regular_args,
           history_comments=format_history(value),
       )
 
   def traverse(value, state: daglish.State):
     if isinstance(value, config_lib.Buildable):
-      ir_for_symbol = _name_to_attribute_expression(
-          task.import_manager.add(config_lib.get_callable(value))
+      ir_for_symbol = import_manager_wrapper.add(
+          config_lib.get_callable(value), task.import_manager
       )
       if isinstance(value, config_lib.Config):
         all_tags = value.__argument_tags__
         value = state.map_children(value)
         for arg, arg_tags in all_tags.items():
           tag_expr = [task.import_manager.add(tag) for tag in arg_tags]
           if arg not in value.__arguments__:
@@ -193,31 +178,31 @@
           )
         return code_ir.SymbolOrFixtureCall(
             symbol_expression=ir_for_symbol,
             positional_arg_expressions=[],
             arg_expressions=config_lib.ordered_arguments(value),
             history_comments=format_history(value),
         )
-      elif isinstance(value, config_lib.Partial):
+      elif isinstance(value, partial.Partial):
         return _handle_partial(value, state, ir_for_symbol)
-      elif isinstance(value, config_lib.ArgFactory):
+      elif isinstance(value, partial.ArgFactory):
         paths = " , ".join(
             daglish.path_str(path) for path in state.get_all_paths()
         )
         raise TypeError(
             "fdl.ArgFactory instances should be inside fdl.Partial's, and "
             "appropriately lowered with the split_arg_factories pass. Either "
             "your config is malformed, or a previous codegen pass introduced "
             f"an error. Path to misformed object in codegen DAG: {paths}.\n\n("
             f"in function definition {fn_name}; `.output_value` "
             "indicates the value in the `return` statement.)"
         )
       else:
         raise TypeError(f"Unsupported Buildable {type(value)}")
     elif is_plain_symbol_or_enum_value(value):
-      return _name_to_attribute_expression(task.import_manager.add(value))
+      return import_manager_wrapper.add(value, task.import_manager)
     else:
       return state.map_children(value)
 
   for fn in task.top_level_call.all_fixture_functions():
     fn_name = fn.name.value
     fn.replace_with(daglish.MemoizedTraversal.run(traverse, fn))
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/naming.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/naming_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/naming_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     num_values = 0
     for value, path in daglish.iterate(config):
       name_set.add(namer.name_for(value, [path]))
       num_values += 1
     self.assertLen(name_set, num_values)
 
   def test_names_as_documented_example_1(self):
-    config = fdl.Config(Foo, bar={"qux": fdl.Config(Qux)})
+    config = fdl.Config(Foo, bar={"qux": fdl.Config(Qux)})  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
     namer = new_path_first_namer()
     names = {
         daglish.path_str(path): namer.name_for(value, [path])
         for value, path in daglish.iterate(config)
     }
     self.assertDictEqual(names, {
         "": "foo",
@@ -206,15 +206,15 @@
     num_values = 0
     for value, path in daglish.iterate(config):
       name_set.add(namer.name_for(value, [path]))
       num_values += 1
     self.assertLen(name_set, num_values)
 
   def test_names_as_documented_example_1(self):
-    config = fdl.Config(Foo, bar={"qux": fdl.Config(Qux)})
+    config = fdl.Config(Foo, bar={"qux": fdl.Config(Qux)})  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
     namer = new_type_first_namer()
     names = {
         daglish.path_str(path): namer.name_for(value, [path])
         for value, path in daglish.iterate(config)
     }
     # N.B. Change from path-first namer: .bar['qux'] is 'qux' not 'bar_qux'.
     self.assertDictEqual(
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/parents_first_traversal.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/shared_to_variables.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/shared_to_variables_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/shared_to_variables_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/split_arg_factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,37 +22,43 @@
 
 For example, when lowering the ArgFactory's into
 """
 
 import copy
 
 from fiddle import daglish
+from fiddle._src import casting
 from fiddle._src import config as config_lib
+from fiddle._src import partial
 from fiddle._src.codegen.auto_config import code_ir
 
 
 def lower_arg_factories(task: code_ir.CodegenTask) -> None:
   """Replaces fdl.ArgFactory(X) with ArgFactoryExpr(fdl.Partial(X))."""
 
   def traverse(value, state: daglish.State):
     def _convert_arg(arg_value):
-      if isinstance(arg_value, config_lib.ArgFactory):
-        return code_ir.ArgFactoryExpr(
-            config_lib.cast(config_lib.Partial, arg_value)
-        )
+      if isinstance(arg_value, partial.ArgFactory):
+        return code_ir.ArgFactoryExpr(casting.cast(partial.Partial, arg_value))
       else:
         return arg_value
 
-    if isinstance(value, config_lib.Partial):
+    if isinstance(value, partial.Partial):
       arguments = config_lib.ordered_arguments(value)
       arguments = {
-          name: state.call(_convert_arg(arg), daglish.Attr(name))
+          name: state.call(_convert_arg(arg), daglish.attr_or_index(name))
           for name, arg in arguments.items()
       }
       value = copy.copy(value)
-      config_lib.assign(value, **arguments)
+      for key, arg_value in arguments.items():
+        if isinstance(key, str):
+          setattr(value, key, arg_value)
+        elif isinstance(key, int):
+          value[key] = arg_value
+        else:
+          raise TypeError(f'Unknown key type: {key}')
       return value
     else:
       return state.map_children(value)
 
   for fn in task.top_level_call.all_fixture_functions():
     fn.replace_with(daglish.MemoizedTraversal.run(traverse, fn))
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/split_arg_factories_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/split_arg_factories_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 from fiddle._src.codegen.auto_config import split_arg_factories
 from fiddle._src.codegen.auto_config import test_fixtures
 
 
 class SplitArgFactoriesTest(absltest.TestCase):
 
   def test_lower_arg_factories(self):
-    config = fdl.Partial(
+    config = fdl.Partial(  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
         test_fixtures.Attention,
         kernel_init=fdl.ArgFactory(
             test_fixtures.initializer, name='const', dtype='float32'
         ),
     )
     task = init_task.init_task(config=config)
     split_arg_factories.lower_arg_factories(task=task)
     code = ir_printer.format_task(task=task)
     self.assertIn('kernel_init=ArgFactoryExpr[fdl.Partial', code)
 
   def test_lower_nested_arg_factories(self):
-    config = fdl.Partial(
+    config = fdl.Partial(  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
         test_fixtures.EncoderLayer,
         attention=fdl.ArgFactory(
             test_fixtures.Attention,
             kernel_init=fdl.ArgFactory(
                 test_fixtures.initializer, name='const', dtype='float32'
             ),
         ),
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/sub_fixture.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/sub_fixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 """Transform sub-fixtures into separate functions."""
 from typing import Any, Callable, Dict, List, Set, Tuple
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
+from fiddle._src import partial
 from fiddle._src.codegen import namespace as namespace_lib
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import naming
 from fiddle._src.codegen.auto_config import parents_first_traversal
 
 
 def _get_node_to_parents_mapping(
@@ -448,15 +449,15 @@
       msg = (
           f"'{name}' already exists in the top level fixture. Please use "
           "another name for the sub-fixture"
       )
       raise ValueError(msg)
 
   for fixture in sub_fixtures.values():
-    if isinstance(fixture, config_lib.ArgFactory):
+    if isinstance(fixture, partial.ArgFactory):
       raise ValueError(
           "fdl.ArgFactory is not supported in auto-config codegen sub-fixture"
           " transformation."
       )
 
   namer = make_namer(namespace_lib.Namespace(existing_names))
   _transform_sub_fixtures(task, sub_fixtures, namer)
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/sub_fixture_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/sub_fixture_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/auto_config/test_fixtures.py` & `fiddle-0.3.0/fiddle/_src/codegen/auto_config/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/codegen_diff.py` & `fiddle-0.3.0/fiddle/_src/codegen/codegen_diff.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,35 +12,78 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Library for converting generating fiddlers from diffs."""
 
 import collections
+import dataclasses
 import functools
 import re
 import types
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple
+from typing import Any, Callable, Dict, List, Literal, Optional, Set, Tuple
 
 from fiddle import daglish
 from fiddle import diffing
 from fiddle._src import config as config_lib
+from fiddle._src import mutate_buildable
+from fiddle._src import tagging
 from fiddle._src.codegen import import_manager as import_manager_lib
 from fiddle._src.codegen import namespace as namespace_lib
 from fiddle._src.codegen import py_val_to_cst_converter
 from fiddle._src.experimental import daglish_legacy
 import libcst as cst
 
 
+@dataclasses.dataclass(frozen=True)
+class ObjectToName:
+  prefix: str
+  path: daglish.Path
+
+  def __hash__(self):
+    return id(self)
+
+
+def assign_explicit_names(
+    all_to_name: List[ObjectToName], param_name: str
+) -> List[str]:
+  """Returns suggested names for a list of objects."""
+  return [
+      to_name.prefix + param_name + '_' + _path_to_name(to_name.path)
+      for to_name in all_to_name
+  ]
+
+
+def assign_short_names(all_to_name: List[ObjectToName]) -> List[str]:
+  """Returns suggested names for a list of objects."""
+  name_to_paths = {}
+  for to_name in all_to_name:
+    sub_path = to_name.path[-1:]
+    name_to_paths.setdefault(
+        to_name.prefix + _path_to_name(sub_path), []
+    ).append(to_name)
+
+  result_as_dict = {}
+  for name, group in name_to_paths.items():
+    if len(group) == 1:
+      result_as_dict[group[0]] = name
+    else:
+      for to_name in group:
+        sub_path = to_name.path[-2:]
+        result_as_dict[to_name] = to_name.prefix + _path_to_name(sub_path)
+  return [result_as_dict[to_name] for to_name in all_to_name]
+
+
 def fiddler_from_diff(
     diff: diffing.Diff,
     old: Any = None,
     func_name: str = 'fiddler',
     param_name: str = 'cfg',
     import_manager: Optional[import_manager_lib.ImportManager] = None,
+    variable_naming: Literal['explicit', 'short'] = 'explicit',
 ):
   """Returns the CST for a fiddler function that applies the changes in `diff`.
 
   The returned `cst.Module` consists of a set of `import` statements for any
   necessary imports, followed by a function definition for a function whose
   name is `func_name`, which takes a single parameter named `param_name`
   containing a `fdl.Config` (or other `Buildable` or structure), and mutates
@@ -68,14 +111,16 @@
       specified, then pessimistically assume that aliases must be created for
       all referenced paths.
     func_name: The name for the fiddler function.
     param_name: The name for the parameter to the fiddler function.
     import_manager: Existing import manager. Usually set to None, but if you are
       integrating this with other code generation tasks, it can be nice to
       share.
+    variable_naming: Whether to create intermediate variables with long,
+      explicit names, or just capture the last elements of a path.
 
   Returns:
     An `cst.Module` object.  You can convert this to a string using
     `result.code`.
   """
   if import_manager is None:
     # Create a namespace to keep track of variables that we add.  Reserve the
@@ -93,26 +138,34 @@
   # Get a list of paths that are referenced by the diff.
   used_paths = _find_used_paths(diff)
 
   # Add variables for any used paths where the value (or any of the value's
   # ancestors) will be replaced by a change in the diff.  If we don't have an
   # `old` structure, then we pessimistically assume that we need to create
   # variables for all used paths.
-  moved_value_names = {}
+  moved_values_to_name = []
   if old is not None:
     modified_paths = set([change.target for change in diff.changes])
     _add_path_aliases(modified_paths, old)
     for path in sorted(used_paths, key=daglish.path_str):
       if any(path[:i] in modified_paths for i in range(len(path) + 1)):
-        moved_value_names[path] = namespace.get_new_name(
-            _path_to_name(path), f'moved_{param_name}_')
+        moved_values_to_name.append(ObjectToName('moved_', path))
   else:
     for path in sorted(used_paths, key=daglish.path_str):
-      moved_value_names[path] = namespace.get_new_name(
-          _path_to_name(path), f'original_{param_name}_')
+      moved_values_to_name.append(ObjectToName('original_', path))
+
+  if variable_naming == 'explicit':
+    initial_names = assign_explicit_names(moved_values_to_name, param_name)
+  else:
+    initial_names = assign_short_names(moved_values_to_name)
+
+  moved_value_names = {
+      to_name.path: namespace.get_new_name(name, prefix='')
+      for to_name, name in zip(moved_values_to_name, initial_names)
+  }
 
   # Add variables for new shared values added by the diff.
   new_shared_value_names = [
       namespace.get_new_name(_name_for_value(value), 'shared_')
       for value in diff.new_shared_values
   ]
 
@@ -311,50 +364,57 @@
 
       if isinstance(child_path_elt, daglish.BuildableFnOrCls):
         assert isinstance(change, diffing.ModifyValue)
         assert update_callable is None
         new_value_cst = pyval_to_cst(change.new_value)
         update_callable = cst.Expr(
             cst.Call(
-                func=pyval_to_cst(config_lib.update_callable),
-                args=[cst.Arg(parent_cst),
-                      cst.Arg(new_value_cst)]))
+                func=pyval_to_cst(mutate_buildable.update_callable),
+                args=[cst.Arg(parent_cst), cst.Arg(new_value_cst)],
+            )
+        )
 
       elif isinstance(change, diffing.DeleteValue):
         deletes.append(cst.Del(target=child_cst))
 
       elif isinstance(change, diffing.RemoveTag):
         arg_name = change.target[-1].name
         deletes.append(
             cst.Expr(
                 cst.Call(
-                    func=pyval_to_cst(config_lib.remove_tag),
+                    func=pyval_to_cst(tagging.remove_tag),
                     args=[
                         cst.Arg(parent_cst),
                         cst.Arg(pyval_to_cst(arg_name)),
-                        cst.Arg(pyval_to_cst(change.tag))
-                    ])))
+                        cst.Arg(pyval_to_cst(change.tag)),
+                    ],
+                )
+            )
+        )
 
       elif isinstance(change, (diffing.SetValue, diffing.ModifyValue)):
         new_value_cst = pyval_to_cst(change.new_value)
         assigns.append(
             cst.Assign(
                 targets=[cst.AssignTarget(child_cst)], value=new_value_cst))
 
       elif isinstance(change, diffing.AddTag):
         arg_name = change.target[-1].name
         assigns.append(
             cst.Expr(
                 value=cst.Call(
-                    func=pyval_to_cst(config_lib.add_tag),
+                    func=pyval_to_cst(tagging.add_tag),
                     args=[
                         cst.Arg(parent_cst),
                         cst.Arg(pyval_to_cst(arg_name)),
-                        cst.Arg(pyval_to_cst(change.tag))
-                    ])))
+                        cst.Arg(pyval_to_cst(change.tag)),
+                    ],
+                )
+            )
+        )
 
       else:
         raise ValueError(f'Unsupported DiffOperation {type(change)}')
 
     body.extend(deletes)
     if update_callable is not None:
       body.append(update_callable)
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/formatting_utilities.py` & `fiddle-0.3.0/fiddle/_src/codegen/formatting_utilities.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/import_manager.py` & `fiddle-0.3.0/fiddle/_src/codegen/import_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import dataclasses
 import enum
 import functools
 import inspect
 from typing import Any, Dict, Union
 
 from absl import logging
+from fiddle._src import special_overrides
 from fiddle._src.codegen import namespace
 import libcst as cst
 
 AnyImport = Union[cst.Import, cst.ImportFrom]
 _dummy_module_for_formatting = cst.Module([])
 
 
@@ -96,43 +97,44 @@
   if isinstance(node, cst.ImportFrom):
     module_str = _dummy_module_for_formatting.code_for_node(node.module)
     return f"{module_str}.{name_str}"
   else:
     return name_str
 
 
-# Project-specific import aliases.
-_SPECIAL_IMPORT_ALIASES = {
-    "fiddle.config": parse_import("import fiddle as fdl"),
-    "fiddle": parse_import("import fiddle as fdl"),
-    "fiddle._src.config": parse_import("import fiddle as fdl"),
-    "fiddle._src.experimental.auto_config": parse_import(
-        "from fiddle.experimental import auto_config"
-    ),
-    "fiddle._src.arg_factory": parse_import("from fiddle import arg_factory"),
-    "fiddle._src.codegen": parse_import("from fiddle import codegen"),
-    "fiddle._src.codegen.py_val_to_cst_converter": parse_import(
-        "from fiddle.codgen import py_val_to_cst_converter"
-    ),
-    "fiddle._src.daglish": parse_import("from fiddle import daglish"),
-}
-
-
 def register_import_alias(name: str, import_stmt: str) -> None:
   """Registers an import alias.
 
+  This function can be used to customize codegen, by changing references to a
+  source module to a public module. For example, let's say you have a public API
+  `foo/bar.py` which has a `from foo._src.bar import Baz` statement. When your
+  Python code references `foo.bar.Baz`, the `inspect` module will see
+  `foo._src.bar.Baz`, and so codegen will emit this name/import. To replace the
+  private (in this example, _src) import with the public API, please use
+
+  ```
+  register_import_alias("foo._src.bar", "from foo import bar")
+  ```
+
+  This will make codegen to emit `from foo import bar` at the top, and use
+  `bar.Baz` in generated fixtures. (You can also change the second argument to
+  "import foo.bar" if you want it to use `foo.bar.Baz` in fixtures.)
+
   Typically this is called by extensions in `fiddle.extensions`.
 
   Args:
     name: Full module name to alias. Often, this is what can be found in
       `type(py_value).__module__.__name__`.
     import_stmt: Import statement for this module, which will be parsed by
       LibCST.
   """
-  _SPECIAL_IMPORT_ALIASES[name] = parse_import(import_stmt)
+  import_override = special_overrides.SpecialOverrides(
+      module_name=name, module_import_alias=import_stmt
+  )
+  special_overrides.register_special_override(name, import_override)
 
 
 def _make_import(full_module_name: str) -> AnyImport:
   """Makes an import statement from a string module name."""
   if "." in full_module_name:
     parent_name, name = full_module_name.rsplit(".", 1)
     return parse_import(f"from {parent_name} import {name}")
@@ -186,17 +188,19 @@
 
     Returns:
       Name for the imported module. This is usually the last name, possibly
       followed by a numeric suffix if necessary to disambiguate from other
       imports or variables. In a few cases where special import aliases are
       applied, then a name with a "." may be emitted.
     """
-    result = _SPECIAL_IMPORT_ALIASES.get(full_module_name)
+    result = special_overrides.SPECIAL_OVERRIDES_MAP.get(full_module_name)
     if result is None:
       result = _make_import(full_module_name)
+    else:
+      result = parse_import(result.module_import_alias)
 
     # Since multiple things could be aliased to the same import, rewrite
     # the module name to the alias' module name.
     full_module_name = get_full_module_name(result)
 
     if full_module_name in self.imports_by_full_name:
       return get_import_name(self.imports_by_full_name[full_module_name])
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/import_manager_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/import_manager_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen.py` & `fiddle-0.3.0/fiddle/_src/codegen/legacy_codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
   children_by_id = {}
 
   def traverse(value, state: daglish.State):
     # N.B. don't memoize or we'll never count the duplicates!
     if isinstance(value, config_lib.Buildable):
       to_count[id(value)] += 1
       children_by_id[id(value)] = value
-    if state.is_traversable(value):
-      state.flattened_map_children(value)
+    for _ in state.yield_map_child_values(value, ignore_leaves=True):
+      pass  # Run lazy iterator.
 
   daglish.BasicTraversal.run(traverse, buildable)
   return [
       children_by_id[child_hash]
       for child_hash, count in to_count.items()
       if count > 1
   ]
@@ -190,18 +190,18 @@
       compatible with daglish. Its dependencies can form a DAG, and any leaf
       nodes will be added first.
     shared_manager: Shared object manager.
     import_manager: Import manager.
     variable_name_prefix: Prefix for any variables introduced.
   """
 
-  def traverse(child, state):
+  def traverse(child, state: daglish.State):
     """Generates code for a shared instance."""
-    if state.is_traversable(child):
-      state.flattened_map_children(child)
+    for _ in state.yield_map_child_values(child, ignore_leaves=True):
+      pass  # Run lazy iterator.
     if isinstance(child, config_lib.Buildable):
       # Name this better..
       name = shared_manager.namespace.get_new_name(
           config_lib.get_callable(child).__name__, prefix=variable_name_prefix)
       relname = import_manager.add(config_lib.get_callable(child))
       buildable_subclass_str = import_manager.add(child.__class__)
       nodes = [
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/legacy_codegen_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/legacy_codegen_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 def identity(x):
   return x
 
 
 def simple_tree() -> fdl.Config[Foo]:
-  return fdl.Config(
+  return fdl.Config(  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
       Foo, a=1, leaves=[
           fdl.Config(Foo, a=2),
           fdl.Config(Foo, a=3),
       ])
 
 
 def shared_config() -> fdl.Config[Baz]:
@@ -168,15 +168,15 @@
 
   return root
     """
     code = "\n".join(result.lines())
     self.assertSequenceEqual(tokens(code), tokens(expected), code)
 
   def test_codegen_import_and_exec(self):
-    cfg = fdl.Config(
+    cfg = fdl.Config(  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
         test_util.Foo, a=1, leaves=[fdl.Config(test_util.Foo, a=2)])
     result = legacy_codegen.codegen_dot_syntax(cfg)
     expected = """
 import fiddle as fdl
 from fiddle._src.codegen import test_util
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/mini_ast.py` & `fiddle-0.3.0/fiddle/_src/codegen/mini_ast.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/namespace.py` & `fiddle-0.3.0/fiddle/_src/codegen/namespace.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/namespace_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/namespace_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/new_codegen.py` & `fiddle-0.3.0/fiddle/_src/codegen/new_codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """
 
 import dataclasses
 from typing import Any, Callable, Dict, Optional, Type
 
 import fiddle as fdl
 from fiddle._src.codegen import newcg_symbolic_references
+from fiddle._src.codegen.auto_config import add_type_signatures
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import experimental_top_level_api
 from fiddle._src.codegen.auto_config import make_symbolic_references as old_symbolic_references
 from fiddle._src.experimental import auto_config
 
 
 @dataclasses.dataclass(frozen=True)
@@ -57,14 +58,21 @@
       newcg_symbolic_references.replace_callables_and_configs_with_symbols
   )
   format_history: Callable[..., Any] = (
       old_symbolic_references.noop_history_comments
   )
 
 
+@dataclasses.dataclass(frozen=True)
+class AddTypeSignatures(experimental_top_level_api.MutationCodegenPass):
+  """Adds return type signatures to fixtures."""
+
+  fn: Callable[..., Any] = add_type_signatures.add_return_types
+
+
 def _get_pass_idx(
     codegen_config: fdl.Config[experimental_top_level_api.Codegen],
     cls: Type[experimental_top_level_api.CodegenPass],
 ) -> int:
   for i, codegen_pass in enumerate(codegen_config.passes):
     if issubclass(fdl.get_callable(codegen_pass), cls):
       return i
@@ -96,14 +104,19 @@
   # Replace ImportSymbols
   idx = _get_pass_idx(config, experimental_top_level_api.ImportSymbols)
   fdl.update_callable(config.passes[idx], ImportSymbols)
 
   # Replace MakeSymbolicReferences
   idx = _get_pass_idx(config, experimental_top_level_api.MakeSymbolicReferences)
   fdl.update_callable(config.passes[idx], MakeSymbolicReferences)
+
+  # Insert type annotations before MakeSymbolicReferences. These type
+  # annotations currently make more sense for non-auto_config cases.
+  config.passes.insert(idx, fdl.Config(AddTypeSignatures))
+
   return config
 
 
 def new_codegen(
     config,
     *,
     top_level_fixture_name: str = "config_fixture",
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/new_codegen_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/new_codegen_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         max_expression_complexity=4,
     )
     expected = """
     import fiddle as fdl
     from fiddle._src.testing.example import fake_encoder_decoder
 
 
-    def config_fixture():
+    def config_fixture() -> fdl.Config[fake_encoder_decoder.FakeEncoder]:
         mlp = fdl.Config(fake_encoder_decoder.Mlp, dtype='float32',
           use_bias=False, sharding_axes=['embed', 'num_heads', 'head_dim'])
         return fdl.Config(fake_encoder_decoder.FakeEncoder, embedders={'tokens':
           fdl.Config(fake_encoder_decoder.TokenEmbedder, dtype='float32'),
           'position': None},
           attention=fdl.Config(fake_encoder_decoder.Attention, dtype='float32',
           kernel_init='uniform()', bias_init='zeros()'), mlp=mlp)
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references.py` & `fiddle-0.3.0/fiddle/_src/codegen/newcg_symbolic_references.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # limitations under the License.
 
 """Changes callables to symbol references for non-auto_config codegen.
 
 N.B. Please see codegen/auto_config for the auto_config version!!
 """
 
-import typing
 from typing import Callable
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen.auto_config import code_ir
+from fiddle._src.codegen.auto_config import import_manager_wrapper
 from fiddle._src.codegen.auto_config import make_symbolic_references as ac_make_symbolic_references
 
 is_plain_symbol_or_enum_value = (
     ac_make_symbolic_references.is_plain_symbol_or_enum_value
 )
 noop_history_comments = ac_make_symbolic_references.noop_history_comments
 
@@ -52,24 +52,14 @@
       for arg_tags in value.__argument_tags__.values():
         for tag in arg_tags:
           task.import_manager.add(tag)
     elif is_plain_symbol_or_enum_value(value):
       task.import_manager.add(value)
 
 
-def _name_to_attribute_expression(name: str) -> code_ir.AttributeExpression:
-  if "." not in name:
-    raise ValueError(f"Could not parse symbol import {name}")
-  base, *parts = name.split(".")
-  value = code_ir.ModuleReference(code_ir.Name(base))
-  for part in parts:
-    value = code_ir.AttributeExpression(value, part)
-  return typing.cast(code_ir.AttributeExpression, value)
-
-
 def replace_callables_and_configs_with_symbols(
     task: code_ir.CodegenTask,
     *,
     format_history: Callable[
         ..., code_ir.HistoryComments
     ] = noop_history_comments,
 ) -> None:
@@ -80,19 +70,19 @@
     format_history: Function used to format history for a buildable. Set to
       get_history_comments.format_history_for_buildable (or a functools.partial
       variant) to populate histories.
   """
 
   def traverse(value, state: daglish.State):
     if isinstance(value, config_lib.Buildable):
-      ir_for_buildable_type = _name_to_attribute_expression(
-          task.import_manager.add(type(value))
+      ir_for_buildable_type = import_manager_wrapper.add(
+          type(value), task.import_manager
       )
-      ir_for_symbol = _name_to_attribute_expression(
-          task.import_manager.add(config_lib.get_callable(value))
+      ir_for_symbol = import_manager_wrapper.add(
+          config_lib.get_callable(value), task.import_manager
       )
       all_tags = value.__argument_tags__
       value = state.map_children(value)
       for arg, arg_tags in all_tags.items():
         tag_expr = [task.import_manager.add(tag) for tag in arg_tags]
         if arg not in value.__arguments__:
           raise ValueError(
@@ -109,13 +99,13 @@
       return code_ir.SymbolOrFixtureCall(
           symbol_expression=ir_for_buildable_type,
           positional_arg_expressions=[ir_for_symbol],
           arg_expressions=config_lib.ordered_arguments(value),
           history_comments=format_history(value),
       )
     elif is_plain_symbol_or_enum_value(value):
-      return _name_to_attribute_expression(task.import_manager.add(value))
+      return import_manager_wrapper.add(value, task.import_manager)
     else:
       return state.map_children(value)
 
   for fn in task.top_level_call.all_fixture_functions():
     fn.replace_with(daglish.MemoizedTraversal.run(traverse, fn))
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/newcg_symbolic_references_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/newcg_symbolic_references_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter.py` & `fiddle-0.3.0/fiddle/_src/codegen/py_val_to_cst_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 """Library for converting Python values to `cst` expressions."""
 
 import builtins
 import enum
 import functools
 import inspect
 import types
-from typing import Any, Callable, Union, Type, List, Optional, NamedTuple, Sequence
+from typing import Any, Callable, List, NamedTuple, Optional, Sequence, Type, Union
 
 from fiddle._src import config as config_lib
+from fiddle._src import partial
 from fiddle._src import tagging
 from fiddle._src.experimental import daglish_legacy
-
 import libcst as cst
 
 # A function that takes any python value, and returns a cst node.
 PyValToCstFunc = Callable[[Any], cst.CSTNode]
 
 # A ValueConverterFunc is a function that takes a value and a PyValToCstFunc,
 # and returns a CST node for the value.  The PyValToCstFunc should be used
@@ -318,15 +318,15 @@
       func=conversion_fn(type(value)),
       args=[
           kwarg_to_cst(arg_name, conversion_fn(arg_val))
           for (arg_name, arg_val) in value._asdict().items()
       ])
 
 
-@register_py_val_to_cst_converter([config_lib.Config, config_lib.Partial])
+@register_py_val_to_cst_converter([config_lib.Config, partial.Partial])
 def _convert_buildable(value: Any,
                        conversion_fn: PyValToCstFunc) -> cst.CSTNode:
   """Converts a fdl.Config or fdl.Partial to CST."""
   args = [cst.Arg(conversion_fn(config_lib.get_callable(value)))]
   for (arg_name, arg_val) in value.__arguments__.items():
     if arg_name in value.__argument_tags__:
       for tag in value.__argument_tags__[arg_name]:
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/py_val_to_cst_converter_test.py` & `fiddle-0.3.0/fiddle/_src/codegen/py_val_to_cst_converter_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
       # Fiddle types:
       (
           fdl.Config(SampleNamedTuple, 3),
           'fiddle._src.config.Config(SampleNamedTuple, x=3)',
       ),
       (
           fdl.Partial(SampleNamedTuple, [4]),
-          'fiddle._src.config.Partial(SampleNamedTuple, x=[4])',
+          'fiddle._src.partial.Partial(SampleNamedTuple, x=[4])',
       ),
       (
           fdl.Config(re.match, 'a|b'),
           "fiddle._src.config.Config(re.match, pattern='a|b')",
       ),
       (SampleTag.new(123), 'SampleTag.new(123)'),
       # NamedTuples:
```

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/special_value_codegen.py` & `fiddle-0.3.0/fiddle/_src/codegen/special_value_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/test_submodule/__init__.py` & `fiddle-0.3.0/fiddle/_src/codegen/test_submodule/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/test_submodule/test_util.py` & `fiddle-0.3.0/fiddle/_src/codegen/test_submodule/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/codegen/test_util.py` & `fiddle-0.3.0/fiddle/_src/codegen/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/config.py` & `fiddle-0.3.0/fiddle/_src/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,60 +18,51 @@
 from __future__ import annotations
 
 import abc
 import collections
 import copy
 import dataclasses
 import functools
-import inspect
-import itertools
-import logging
 import types
 from typing import Any, Callable, Collection, Dict, FrozenSet, Generic, Iterable, Mapping, NamedTuple, Optional, Set, Tuple, Type, TypeVar, Union
 
-from fiddle._src import arg_factory
 from fiddle._src import daglish
 from fiddle._src import history
 from fiddle._src import signatures
 from fiddle._src import tag_type
 
 
 T = TypeVar('T')
 TypeOrCallableProducingT = Union[Callable[..., T], Type[T]]
 
-
-class NoValue:
-  """Sentinel class for arguments with no value."""
-
-  def __repr__(self):
-    return 'fdl.NO_VALUE'
-
-  def __deepcopy__(self, memo):
-    """Override for deepcopy that does not copy this sentinel object."""
-    del memo
-    return self
-
-  def __copy__(self):
-    """Override for `copy.copy()` that does not copy this sentinel object."""
-    return self
-
-
-NO_VALUE = NoValue()
+NoValue = signatures.NoValue
+# A sentinel object that represents no value is set for the argument.
+NO_VALUE = signatures.NO_VALUE
 
 # Unique object instance that should never be used by end-users, and can thus
 # be used to differentiate between unset values and user-set values that are
 # None or other commonly-used sentinel.
 _UNSET_SENTINEL = object()
 
 
 _defaults_aware_traverser_registry = daglish.NodeTraverserRegistry(
     use_fallback=True
 )
 
 
+class _Placeholder(object):
+  """A Placeholder class to represent config arguments."""
+
+  def __init__(self, index):
+    self.index = index
+
+  def __eq__(self, other):
+    return self.index == other.index
+
+
 def _buildable_flatten(
     buildable: Buildable, include_defaults: bool = False
 ) -> Tuple[Tuple[Any, ...], BuildableTraverserMetadata]:
   """Implement Buildable.__flatten__ method."""
   arguments = ordered_arguments(buildable, include_defaults=include_defaults)
   keys = tuple(arguments.keys())
   values = tuple(arguments.values())
@@ -91,18 +82,18 @@
       argument_history=argument_history,
   )
   return values, metadata
 
 
 def _buildable_path_elements(
     buildable: Buildable, include_defaults: bool = False
-) -> Tuple[daglish.Attr]:
+) -> Tuple[daglish.PathElement]:
   """Implement Buildable.__path_elements__ method."""
   return tuple(
-      daglish.Attr(name)
+      daglish.Attr(name) if isinstance(name, str) else daglish.Index(name)
       for name in ordered_arguments(
           buildable, include_defaults=include_defaults
       ).keys()
   )
 
 
 def _register_buildable_defaults_aware_traversers(cls: Type[Buildable]):
@@ -120,23 +111,33 @@
 def _compare_buildable(x: Buildable, y: Buildable, check_dag: bool = False):
   """Compare if two Buildables are equal, including DAG structure."""
   assert isinstance(x, Buildable)
   if type(x) is not type(y):
     return False
   if x.__fn_or_cls__ != y.__fn_or_cls__:
     return False
-  assert x._has_var_keyword == y._has_var_keyword, (  # pylint: disable=protected-access
+  assert (
+      x.__signature_info__.has_var_keyword
+      == y.__signature_info__.has_var_keyword
+  ), (  # pylint: disable=protected-access
       'Internal invariant violated: has_var_keyword should be the same if '
       "__fn_or_cls__'s are the same."
   )
 
   missing = object()
+
+  def get_value_or_default(key: Union[str, int], buildable: Buildable) -> Any:
+    value = buildable.__arguments__.get(key, missing)
+    if value is missing:
+      value = buildable.__signature_info__.get_default(key, missing)
+    return value
+
   for key in set(x.__arguments__) | set(y.__arguments__):
-    v1 = getattr(x, key, missing)
-    v2 = getattr(y, key, missing)
+    v1 = get_value_or_default(key, x)
+    v2 = get_value_or_default(key, y)
     assert not (v1 is missing and v2 is missing)
     if v1 is missing or v2 is missing:
       return False
     if isinstance(v1, Buildable) and isinstance(v2, Buildable):
       if not _compare_buildable(v1, v2, check_dag=False):
         return False
     if v1 != v2:
@@ -180,15 +181,15 @@
 class BuildableTraverserMetadata(NamedTuple):
   """Metadata for a Buildable.
 
   This separate class is used for DAG traversals.
   """
 
   fn_or_cls: Callable[..., Any]
-  argument_names: Tuple[str, ...]
+  argument_names: Tuple[Union[str, int], ...]
   argument_tags: Dict[str, FrozenSet[tag_type.TagType]]
   argument_history: Mapping[str, Tuple[history.HistoryEntry, ...]] = (
       types.MappingProxyType({})
   )
 
   def without_history(self) -> BuildableTraverserMetadata:
     return self._replace(argument_history={})
@@ -210,24 +211,29 @@
 
 class Buildable(Generic[T], metaclass=abc.ABCMeta):
   """Base class for buildable types (``Config`` and ``Partial``).
 
   Buildable types implement a ``__build__`` method that is called during
   ``fdl.build()`` with arguments set on the ``Buildable`` to get output for the
   corresponding instance.
+
+  Arguments are stored in the `__arguments__` dict with the following
+  "canonical storage format":
+  Positional-only and variadic-positional arguments use the position index of
+  the argument as a key (of type int); all other arguments use the name of the
+  argument as a key (of type str).
   """
 
   # "Dunder"-style names were chosen here to reduce the possibility of naming
   # conflicts while still making the fields accessible.
   __fn_or_cls__: TypeOrCallableProducingT[T]
-  __signature__: inspect.Signature
-  __arguments__: Dict[str, Any]
+  __arguments__: Dict[Union[str, int], Any]
   __argument_history__: history.History
-  __argument_tags__: Dict[str, Set[tag_type.TagType]]
-  _has_var_keyword: bool
+  __argument_tags__: Dict[Union[str, int], Set[tag_type.TagType]]
+  __signature_info__: signatures.SignatureInfo
 
   def __init__(
       self,
       fn_or_cls: Union['Buildable[T]', TypeOrCallableProducingT[T]],
       *args,
       **kwargs,
   ):
@@ -235,45 +241,41 @@
 
     Args:
       fn_or_cls: A callable to configure. The signature of this callable will
         determine the parameters this ``Buidlable`` can be used to configure.
       *args: Any positional arguments to configure for ``fn_or_cls``.
       **kwargs: Any keyword arguments to configure for ``fn_or_cls``.
     """
-    signature = self.__init_callable__(fn_or_cls)
+    self.__init_callable__(fn_or_cls)
     arg_history = history.History()
     arg_history.add_new_value('__fn_or_cls__', fn_or_cls)
     super().__setattr__('__argument_history__', arg_history)
     super().__setattr__('__argument_tags__', collections.defaultdict(set))
+    arguments = signatures.SignatureInfo.signature_binding(
+        fn_or_cls, *args, **kwargs
+    )
 
-    arguments = signature.bind_partial(*args, **kwargs).arguments
-    for name in list(arguments.keys()):  # Make a copy in case we mutate.
-      param = signature.parameters[name]
-      if param.kind == param.VAR_POSITIONAL:
-        # TODO(b/197367863): Add *args support.
-        err_msg = (
-            'Variable positional arguments (aka `*args`) not supported. '
-            f'Found param `{name}` in `{fn_or_cls}`.'
+    for key, value in arguments.items():
+      if isinstance(key, (str, int)):
+        self._arguments_set_value(key, value)
+      else:
+        raise ValueError(
+            f'Unexpected type received for the argument name: {key!r}'
         )
-        raise NotImplementedError(err_msg)
-      elif param.kind == param.VAR_KEYWORD:
-        arguments.update(arguments.pop(param.name))
-
-    for name, value in arguments.items():
-      setattr(self, name, value)
 
     for name, tags in tag_type.find_tags_from_annotations(fn_or_cls).items():
       self.__argument_tags__[name].update(tags)
       self.__argument_history__.add_updated_tags(
           name, self.__argument_tags__[name]
       )
 
   def __init_callable__(
       self, fn_or_cls: Union['Buildable[T]', TypeOrCallableProducingT[T]]
-  ) -> inspect.Signature:
+  ) -> None:
+    """Save information on `fn_or_cls` to the `Buildable`."""
     if isinstance(fn_or_cls, Buildable):
       raise ValueError(
           'Using the Buildable constructor to convert a buildable to a new '
           'type or to override arguments is forbidden; please use either '
           '`fdl.cast(new_type, buildable)` (for casting) or '
           '`fdl.copy_with(buildable, **kwargs)` (for overriding arguments).'
       )
@@ -281,21 +283,20 @@
     # Using `super().__setattr__` here because assigning directly would trigger
     # our `__setattr__` override. Using `super().__setattr__` instead of special
     # casing these attribute names in `__setattr__` also has the effect of
     # making them easily gettable but not as easily settable by user code.
     super().__setattr__('__fn_or_cls__', fn_or_cls)
     super().__setattr__('__arguments__', {})
     signature = signatures.get_signature(fn_or_cls)
-    super().__setattr__('__signature__', signature)
-    has_var_keyword = any(
-        param.kind == param.VAR_KEYWORD
-        for param in signature.parameters.values()
+    # Several attributes are computed automatically by SignatureInfo during
+    # `__post_init__`.
+    super().__setattr__(
+        '__signature_info__',
+        signatures.SignatureInfo(signature=signature),
     )
-    super().__setattr__('_has_var_keyword', has_var_keyword)
-    return signature
 
   def __init_subclass__(cls):
     daglish.register_node_traverser(
         cls,
         flatten_fn=lambda x: x.__flatten__(),
         unflatten_fn=cls.__unflatten__,
         path_elements_fn=lambda x: x.__path_elements__(),
@@ -317,32 +318,40 @@
     rebuilt = cls.__new__(cls)
     rebuilt.__init_callable__(metadata.fn_or_cls)
     object.__setattr__(rebuilt, '__argument_tags__', metadata.tags())
     object.__setattr__(rebuilt, '__argument_history__', metadata.history())
     object.__setattr__(rebuilt, '__arguments__', metadata.arguments(values))
     return rebuilt
 
-  def __path_elements__(self) -> Tuple[daglish.Attr]:
+  def __path_elements__(self) -> Tuple[daglish.PathElement]:
     return _buildable_path_elements(self, include_defaults=False)
 
   def __getattr__(self, name: str):
     """Get parameter with given ``name``."""
     value = self.__arguments__.get(name, _UNSET_SENTINEL)
+    # Check that positional-only arguments cannot be accessed by keywords.
+    param = self.__signature_info__.parameters.get(name)
+    if param is not None and (
+        param.kind in (param.POSITIONAL_ONLY, param.VAR_POSITIONAL)
+    ):
+      raise AttributeError(
+          'Cannot access positional-only or variadic positional arguments '
+          f'{name} on {self!r} using attributes.'
+      )
 
     if value is not _UNSET_SENTINEL:
       return value
     if dataclasses.is_dataclass(
         self.__fn_or_cls__
     ) and _field_uses_default_factory(self.__fn_or_cls__, name):
       raise ValueError(
           "Can't get default value for dataclass field "
           + f'{self.__fn_or_cls__.__qualname__}.{name} '
           + 'since it uses a default_factory.'
       )
-    param = self.__signature__.parameters.get(name)
     if param is not None and param.default is not param.empty:
       return param.default
     msg = f"No parameter '{name}' has been set on {self!r}."
     # TODO(b/219988937): Implement an edit distance function and display valid
     # attributes that are close to `name`.
     if hasattr(self.__fn_or_cls__, name):
       msg += (
@@ -351,116 +360,222 @@
           'this name, so this could be caused by using a '
           f'fdl.{self.__class__.__qualname__} in '
           'place of the actual function or class being configured. Did you '
           'forget to call `fdl.build(...)`?'
       )
     raise AttributeError(msg)
 
-  def __validate_param_name__(self, name) -> None:
-    """Raises an error if ``name`` is not a valid parameter name."""
-    param = self.__signature__.parameters.get(name)
-
-    if param is not None:
-      if param.kind == param.POSITIONAL_ONLY:
-        # TODO(b/197367863): Add positional-only arg support.
-        raise NotImplementedError(
-            'Positional only arguments not supported. '
-            f'Tried to set {name!r} on {self.__fn_or_cls__}'
-        )
-      elif param.kind in (param.VAR_POSITIONAL, param.VAR_KEYWORD):
-        # Just pretend it doesn't correspond to a valid parameter name... below
-        # a TypeError will be thrown unless there is a **kwargs parameter.
-        param = None
-
-    if param is None and not self._has_var_keyword:
-      if name in self.__signature__.parameters:
-        err_msg = f'Variadic arguments (e.g. *{name}) are not supported.'
-      else:
-        valid_parameter_names = (
-            name
-            for name, param in self.__signature__.parameters.items()
-            if param.kind not in (param.POSITIONAL_ONLY, param.VAR_POSITIONAL)
-        )
-        err_msg = (
-            f"No parameter named '{name}' exists for "
-            f'{self.__fn_or_cls__}; valid parameter names: '
-            f"{', '.join(valid_parameter_names)}."
-        )
-      raise TypeError(err_msg)
-
-  def __setattr__(self, name: str, value: Any):
-    """Sets parameter ``name`` to ``value``."""
-
-    self.__validate_param_name__(name)
-
+  def _arguments_set_value(self, key: Union[int, str], value: Any):
+    """Set `self.__arguments__` values directly."""
     if isinstance(value, TaggedValueCls):
       tags = value.__argument_tags__.get('value', ())
       if tags:
-        self.__argument_tags__[name].update(tags)
+        self.__argument_tags__[key].update(tags)
         self.__argument_history__.add_updated_tags(
-            name, self.__argument_tags__[name]
+            key, self.__argument_tags__[key]
         )
       if 'value' in value.__arguments__:
         value = value.__arguments__['value']
       else:
         return
 
-    self.__arguments__[name] = value
-    self.__argument_history__.add_new_value(name, value)
+    self.__arguments__[key] = value
+    self.__argument_history__.add_new_value(key, value)
+
+  def _arguments_del_value(self, key: Union[int, str]):
+    """Delete `self.__arguments__` values directly."""
+    del self.__arguments__[key]
+    self.__argument_history__.add_deleted_value(key)
+
+  def __setattr__(self, name: str, value: Any):
+    """Sets parameter ``name`` to ``value``."""
+    self.__signature_info__.validate_param_name(name, self.__fn_or_cls__)
+    self._arguments_set_value(name, value)
 
   def __delattr__(self, name):
     """Unsets parameter ``name``."""
     try:
-      del self.__arguments__[name]
-      self.__argument_history__.add_deleted_value(name)
+      self._arguments_del_value(name)
     except KeyError:
       err = AttributeError(f"No parameter '{name}' has been set on {self!r}")
       raise err from None
 
+  def __getitem__(self, key: Any):
+    """Get positional arguments by index."""
+    key = self.__signature_info__.replace_varargs_handle(key)
+    all_positional_args, _ = self.__signature_info__.transform_to_args_kwargs(
+        self.__arguments__,
+        include_pos_or_kw_in_args=True,
+        include_no_value=True,
+    )
+    params = list(self.__signature_info__.parameters.values())
+    for index, value in enumerate(all_positional_args):
+      if value is NO_VALUE and index < len(params):
+        param = params[index]
+        if param.default is not param.empty:
+          all_positional_args[index] = param.default
+    return all_positional_args[key]
+
+  def __delitem__(self, key: Any):
+    """Delete positional arguments by index."""
+    key = self.__signature_info__.replace_varargs_handle(key)
+    all_positional_args, _ = self.__signature_info__.transform_to_args_kwargs(
+        self.__arguments__,
+        include_pos_or_kw_in_args=True,
+        include_no_value=True,
+    )
+    var_positional_start = self.__signature_info__.var_positional_start
+    if isinstance(key, slice):
+      key = key.indices(len(all_positional_args))
+      indices = list(range(*key))
+    else:
+      if key < 0:
+        key += len(all_positional_args)
+      indices = [key]
+
+    old_placeholders = [
+        _Placeholder(index) for index in range(len(all_positional_args))
+    ]
+    new_placeholders = old_placeholders.copy()
+    # Traverse from largest index to maintain order of undeleted indices.
+    for index in indices[::-1]:
+      if index < var_positional_start:
+        k = self.__signature_info__.index_to_key(index, self.__arguments__)
+        if k in self.__arguments__:
+          self._arguments_del_value(k)
+      else:
+        del new_placeholders[index]
+
+    # Delete var-positional args and compact the *args list.
+    for index in range(var_positional_start, len(old_placeholders)):
+      if index < len(new_placeholders):
+        if new_placeholders[index] != old_placeholders[index]:
+          new_value = self.__arguments__[new_placeholders[index].index]
+          self._arguments_set_value(index, new_value)
+      else:
+        self._arguments_del_value(index)
+
+  def _set_item_by_index(self, key: int, value: Any):
+    """Set positional arguments by index."""
+    key = self.__signature_info__.index_to_key(key, self.__arguments__)
+    positional_num = self.__signature_info__.var_positional_start
+    if positional_num is None:
+      # *args does not exist
+      positional_num = len(self.__signature_info__.parameters)
+      if self.__signature_info__.var_keyword_name:
+        # Exclude **kwargs
+        positional_num -= 1
+
+    # Cannot set item when index is beyond current positional args list length.
+    # Only index that points to *args can be out of range.
+    if (
+        isinstance(key, int)
+        and key >= positional_num
+        and key not in self.__arguments__
+    ):
+      raise IndexError(
+          f'Cannot set positional argument with index {key}'
+          ' (index out of range).'
+      )
+    self._arguments_set_value(key, value)
+
+  def _set_item_by_slice(self, slice_key: slice, value: Any):
+    """Set positional arguments by slice."""
+    all_positional_args, _ = self.__signature_info__.transform_to_args_kwargs(
+        self.__arguments__,
+        include_pos_or_kw_in_args=True,
+        include_no_value=True,
+    )
+    var_positional_start = self.__signature_info__.var_positional_start
+    index_range = slice_key.indices(len(all_positional_args))
+    if var_positional_start is None or index_range[0] < var_positional_start:
+      # The slice key spans on non-variadic positional arguments, this set item
+      # operation cannot modify the total length of full positiona args list.
+      indices = range(*index_range)
+      if len(indices) != len(value):
+        raise ValueError(
+            'Cannot modify the total length of full positional arguments list'
+            ' with __setitem__ when the slice key spans over non-variadic'
+            ' positional arguments. To remove values, use `del config[key]`.'
+            ' To append values to variadic positional arguments, you can use '
+            ' config[fdl.VARARGS:] = value.'
+        )
+      for index, v in zip(indices, value):
+        self._set_item_by_index(index, v)
+    else:
+      # The slice key only spans on variadic positional arguments
+      old_placeholders = [
+          _Placeholder(index) for index in range(len(all_positional_args))
+      ]
+      new_placeholders = old_placeholders.copy()
+      new_placeholders[slice_key] = value
+      for index in range(var_positional_start, len(old_placeholders)):
+        if index < len(new_placeholders):
+          new_value = new_placeholders[index]
+          if isinstance(new_value, _Placeholder):
+            if new_value == old_placeholders[index]:
+              continue
+            else:
+              new_value = self.__arguments__[new_value.index]
+          self._arguments_set_value(index, new_value)
+        else:
+          self._arguments_del_value(index)
+      len_old = len(old_placeholders)
+      len_new = len(new_placeholders)
+      for index in range(len_old, len_new):
+        new_value = new_placeholders[index]
+        if isinstance(new_value, _Placeholder):
+          new_value = self.__arguments__[new_value.index]
+        self._arguments_set_value(index, new_value)
+
+  def __setitem__(self, key: Any, value: Any):
+    """Set positional arguments by index."""
+    key = self.__signature_info__.replace_varargs_handle(key)
+    if isinstance(key, int):
+      self._set_item_by_index(key, value)
+    elif isinstance(key, slice):
+      self._set_item_by_slice(key, value)
+
   def __dir__(self) -> Collection[str]:
     """Provide a useful list of attribute names, optimized for Jupyter/Colab.
 
     ``__dir__`` is often implicitly called by tooling such as Jupyter/Colab to
     provide autocomplete suggestions. This implementation of ``__dir__`` makes
     it easy to see what are valid attributes to get, set, or delete.
 
     Returns:
       A list of useful attribute names corresponding to set or unset parameters.
     """
-    valid_param_names = {
-        name
-        for name, param in self.__signature__.parameters.items()
-        if param.kind in (param.POSITIONAL_OR_KEYWORD, param.KEYWORD_ONLY)
-    }
     set_argument_names = self.__arguments__.keys()
+    valid_param_names = set(self.__signature_info__.valid_param_names)
     all_names = valid_param_names.union(set_argument_names)
     return all_names
 
   def __repr__(self):
     if hasattr(self.__fn_or_cls__, '__qualname__'):
       formatted_fn_or_cls = self.__fn_or_cls__.__qualname__
     else:
       formatted_fn_or_cls = str(self.__fn_or_cls__)
     formatted_params = []
     # Show parameters from signature first (in signature order) followed by
     # **varkwarg parameters (in the order they were set).
-    param_names = list(self.__signature__.parameters) + [
+    param_names = list(self.__signature_info__.parameters) + [
         name
         for name in self.__arguments__
-        if name not in self.__signature__.parameters
+        if name not in self.__signature_info__.parameters
     ]
 
     for name in param_names:
       tags = self.__argument_tags__.get(name, ())
-      value = self.__arguments__.get(name, _UNSET_SENTINEL)
-      if tags or (value is not _UNSET_SENTINEL):
-        param_str = name
+      value = self.__arguments__.get(name, NO_VALUE)
+      if tags or (value is not NO_VALUE):
+        param_str = str(name)
         if tags:
           param_str += f"[{', '.join(sorted(str(tag) for tag in tags))}]"
-        if value is not _UNSET_SENTINEL:
+        if value is not NO_VALUE:
           param_str += f'={value!r}'
         formatted_params.append(param_str)
 
     name = type(self).__name__
 
     formatted_params_no_linebreak = ', '.join(formatted_params)
     # An arbitrary threshold to determine whether to add linebreaks to args.
@@ -491,18 +606,20 @@
     Returns:
       A shallow copy of this ``Buildable``.
     """
     # TODO(b/231368256): Preserve argument history...
     return self.__unflatten__(*self.__flatten__())
 
   def __deepcopy__(self, memo: Dict[int, Any]):
-    """Deepcopies this ``Buildable``, skipping copying of ``__signature__``."""
+    """Deepcopies this Buildable, skipping copying of ``__signature_info__``."""
     # Skipping copying inspect.Signature objects, which are generally immutable,
     # is about 2x faster on artificial benchmarks.
-    memo[id(self.__signature__)] = self.__signature__
+    memo[id(self.__signature_info__.signature)] = (
+        self.__signature_info__.signature
+    )
     result = object.__new__(type(self))
     result.__dict__.update(copy.deepcopy(self.__dict__, memo))
     return result
 
   def __eq__(self, other):
     """Returns true iff self and other contain the same argument values.
 
@@ -525,38 +642,41 @@
       ``True`` if ``self`` equals ``other``, ``False`` if not.
     """
     return _compare_buildable(self, other, check_dag=True)
 
   def __getstate__(self):
     """Gets pickle serialization state, removing some fields.
 
-    For now, we discard the ``__signature__`` (which can be recalculated) and
-    ``__argument_history__``, because these tend to contain values which cannot
-    be serialized.
+    For now, we discard the ``__signature_info__.signature`` (which can be
+    recalculated), because these tend to contain values which cannot be
+    serialized.
 
     Returns:
       Dict of serialized state.
     """
     result = dict(self.__dict__)
-    result.pop('__signature__', None)
+    # During serialization, set `__signature_info__` as None to avoid signature
+    # serialization issues.
+    result['__signature_info__'] = None
     return result
 
   def __setstate__(self, state) -> None:
     """Loads pickle serialization state.
 
-    This re-derives the signature if not present, and adds an empty
-    ``__argument_history__``, if it was removed.
+    This re-derives the signature if not present.
 
     Args:
       state: State dictionary, from ``__getstate__``.
     """
     self.__dict__.update(state)  # Support unpickle.
-    if '__signature__' not in self.__dict__:
-      object.__setattr__(
-          self, '__signature__', signatures.get_signature(self.__fn_or_cls__)
+    if self.__signature_info__ is None:
+      signature = signatures.get_signature(self.__fn_or_cls__)
+      super().__setattr__(
+          '__signature_info__',
+          signatures.SignatureInfo(signature=signature),
       )
 
 
 class Config(Generic[T], Buildable[T]):
   """A mutable representation of a function or class's parameters.
 
   This class represents the configuration for a given function or class,
@@ -584,36 +704,72 @@
 
       def test_function(arg, kwarg=None):
         return arg, kwarg
 
       fn_config = Config(test_function, 1)
       fn_config.kwarg = 'kwarg'
 
+  If the class/function has positional arguments, they can be accessed through
+  the `[]` syntax::
+
+      def test_function(a, b, /, c, *args):
+        return locals()
+
+      fn_config = Config(test_function, 1, 2, 3, 4, 5)
+
+      # Read
+      assert fn_config[0] == 1
+      assert fn_config[:] == [1, 2, 3, 4, 5]
+
+      # Modify
+      fn_config[0] = 'a'
+      fn_config.c = 'c'
+
+      # `fdl.VARARGS` represents the start of variadic positional args (*args)
+      fn_config[fdl.VARARGS:] = ['x', 'y']
+      assert fn_config[:] == [1, 2, 3, 'x', 'y']
+
+      # Delete
+      del fn_config[0]
+      del fn_config[fdl.VARARGS:]
+      assert fn_config[:] == [fdl.NO_VALUE, 2, 3]
+
+  NOTE: Directly calling `list` methods like `append` and `extend` is not
+  supported, and will not mutate the config. Like with Python lists, slice
+  operations on Configs effectively create a copy of the underlying sequence.
+
+  NOTE: If using `slice` as key for modifying the config, and the `slice` spans
+  over positional-only or positional-or-keyword arguments, the provided value
+  must have the same length as that of the slice range.
+
+  fn_config[2:4] = ['a', 'b'] # OK
+  fn_config[2:4] = ['m']      # Not OK. Will raise an error!
+
   A ``Config`` instance may be transformed into instances and function outputs
   by passing it to the ``build`` function. The ``build`` function invokes each
   function or class in the configuration tree (appropriately propagating the
   built outputs from nested ``Config``'s). For example, using the
   ``SampleClass`` config from above::
 
       instance = build(class_config)
       assert instance.arg == 1
       assert instance.kwarg == 'kwarg'
 
   If the same ``Config`` instance is used in multiple places within the
   configuration tree, its function or class is invoked only once during
-  ``build``, and the result shared across all occurences of the ``Config``
+  ``build``, and the result shared across all occurrences of the ``Config``
   instance. (See ``build`` documentation for further details.) To create a new
   instance of a ``Config`` with the same parameter settings that will yield a
   separate instance during ``build``, ``copy.copy()`` or ``copy.deepcopy()``
   may be used.
   """
 
   # NOTE(b/201159339): We currently need to repeat these annotations for pytype.
   __fn_or_cls__: TypeOrCallableProducingT[T]
-  __signature__: inspect.Signature
+  __signature_info__: signatures.SignatureInfo
 
   def __build__(self, *args, **kwargs):
     """Builds this ``Config`` for the given ``args`` and ``kwargs``.
 
     This method is called during `build` to get the output for this `Config`.
 
     Args:
@@ -658,532 +814,117 @@
   of a Fiddle Buildable, will be expanded into that argument's values and tags.
   However, they may survive as stand-alone objects within tuples, lists, and
   dictionaries.
   """
 
   # NOTE(b/201159339): We currently need to repeat these annotations for pytype.
   __fn_or_cls__: TypeOrCallableProducingT[T]
-  __signature__: inspect.Signature
+  __signature_info__: signatures.SignatureInfo
 
   @property
   def tags(self):
     return self.__argument_tags__['value']
 
   def __build__(self, *args: Any, **kwargs: Any) -> T:
     if self.__fn_or_cls__ is not tagged_value_fn:
       raise RuntimeError(
           'Unexpected __fn_or_cls__ in TaggedValueCls; found:'
           f'{self.__fn_or_cls__}'
       )
     return self.__fn_or_cls__(tags=self.tags, *args, **kwargs)
 
 
-@dataclasses.dataclass(frozen=True)
-class _BuiltArgFactory:
-  """The result of building an ``ArgFactory``.
-
-  This wrapper is returned by ``ArgFactory.__build__``, and then consumed by the
-  ``__build__`` method of the containing ``Partial`` or ``ArgFactory`` object.
-  """
-
-  factory: Callable[..., Any]
-
-
-def _contains_arg_factory(value: Any) -> bool:
-  """Returns true if ``value`` contains any ``_BuiltArgFactory`` instances."""
-
-  def visit(node, state):
-    if isinstance(node, _BuiltArgFactory):
-      return True
-    elif state.is_traversable(node):
-      return any(state.flattened_map_children(node).values)
-    else:
-      return False
-
-  return daglish.MemoizedTraversal.run(visit, value)
-
-
-def _invoke_arg_factories(value: Any) -> Any:
-  """Makes a copy of value with any _BuiltArgFactory ``f`` replaced by ``f()``.
-
-  The copy is "shallow" in the sense that only containers that (directly or
-  indirectly) contain _BuiltArgFactories are replaced.  E.g.:
-
-  >>> x = []
-  >>> value = [[], _BuiltArgFactory(list)]
-  >>> result = _invoke_arg_factories(value)
-  >>> assert value[0] is result[0]  # not replaced
-
-  Args:
-    value: The structured value containing _BuiltArgFactories.
-
-  Returns:
-    A copy of ``value``.
-  """
-
-  def visit(node, state: daglish.State):
-    if isinstance(node, _BuiltArgFactory):
-      return node.factory()
-    elif state.is_traversable(node):
-      subtraversal = state.flattened_map_children(node)
-      old_vals, _ = subtraversal.node_traverser.flatten(node)
-      no_child_changed = all(
-          [old is new for (old, new) in zip(old_vals, subtraversal.values)]
-      )
-      return node if no_child_changed else subtraversal.unflatten()
-    else:
-      return node
-
-  return daglish.MemoizedTraversal.run(visit, value)
-
-
-def _promote_arg_factory(arg: Any) -> Any:
-  """Converts a structure-of-ArgFactory's to an ArgFactory-of-structure.
-
-  If `arg` is a `_BuiltArgFactory`, or is a nested structure that doesn't
-  contain any `_BuiltArgFactory`s, then return it as-is.
-
-  Othewise, return a new `_BuiltArgFactory` whose factory returns a copy of
-  `arg` with any `_BuiltArgFactory` `f` replaced by `f()`.
-
-  Args:
-    arg: The argument value to convert.
-
-  Returns:
-    `arg`; or a `_BuiltArgFactory` whose factory returns a copy of `arg` with
-    any `_BuiltArgFactory` `f` replaced by `f()`.
-  """
-  if isinstance(arg, _BuiltArgFactory) or not _contains_arg_factory(arg):
-    return arg
-  else:
-    return _BuiltArgFactory(functools.partial(_invoke_arg_factories, arg))
-
-
-def _build_partial(
-    fn: Callable[..., Any], args: Tuple[Any], kwargs: Dict[str, Any]
-) -> functools.partial:
-  """Returns `functools.partial` or `arg_factory.partial` for `fn`.
-
-  If `args` or `kwargs` contain any `ArgFactory` instances, then return
-  `arg_factory.partial(fn, *args, **kwargs)`.  Otherwise, return
-  `functools.partial(fn, *args, **kwargs)`.  If any `args` or `kwargs`
-  are nested structures that contain one or more `ArgFactory`s, then
-  convert them to an `ArgFactory` that returns a copy of that structure with
-  the nested `ArgFactory`s invoked.
-
-  Args:
-    fn: The function argument for the partial.
-    args: The positional arguments for the partial.
-    kwargs: The keyword arguments for the partial.
-  """
-
-  def is_arg_factory(value):
-    return isinstance(value, _BuiltArgFactory)
-
-  # If there are nested structures containing _BuiltArgFactory objects,
-  # then promote them.
-  args = [_promote_arg_factory(arg) for arg in args]
-  kwargs = {name: _promote_arg_factory(arg) for name, arg in kwargs.items()}
-
-  # Split the keyword args into those that should be handled by functools vs.
-  # arg_factory.
-  arg_factory_kwargs = {
-      name: arg.factory for name, arg in kwargs.items() if is_arg_factory(arg)
-  }
-  functool_kwargs = {
-      name: arg
-      for name, arg in kwargs.items()
-      if not isinstance(arg, _BuiltArgFactory)
-  }
-
-  # Group positional args by whether they are factories; and add partial
-  # wrappers for each group.  Note: this never actually gets exercised by
-  # fdl.build, since `fdl.build` calls `__build__(**arguments)`, and doesn't
-  # pass in any positional arguments; so `args` will always be empty when
-  # this is executed by `fdl.build()`.
-  result = fn
-  for is_factory, arg_values in itertools.groupby(args, is_arg_factory):
-    if is_factory:
-      arg_values = [arg.factory for arg in arg_values]
-      result = arg_factory.partial(result, *arg_values, **arg_factory_kwargs)
-      arg_factory_kwargs = {}
-    else:
-      result = functools.partial(result, *arg_values, **functool_kwargs)
-      functool_kwargs = {}
-
-  if arg_factory_kwargs:
-    result = arg_factory.partial(result, **arg_factory_kwargs)
-  return functools.partial(result, **functool_kwargs)
-
-
-class Partial(Generic[T], Buildable[T]):
-  """A ``Partial`` config creates a partial function or class when built.
-
-  In some cases, it may be desired to leave a function or class uninvoked, and
-  instead output a corresponding ``functools.partial`` object. Where the
-  ``Config`` base class calls its underlying ``__fn_or_cls__`` when built, this
-  ``Partial`` instead results in a partially bound function or class::
-
-      partial_config = Partial(SampleClass)
-      partial_config.arg = 1
-      partial_config.kwarg = 'kwarg'
-      partial_class = build(partial_config)
-      instance = partial_class(arg=2)  # Keyword arguments can be overridden.
-      assert instance.arg == 2
-      assert instance.kwarg == 'kwarg'
-
-  A ``Partial`` can also be created from an existing ``Config``, by passing it
-  to the ``Partial`` constructor. This results in a shallow copy that is
-  decoupled from the ``Config`` used to create it. In the example below, any
-  further changes to ``partial_config`` are not reflected by ``class_config``
-  (and vice versa)::
-
-      partial_config = Partial(class_config)
-      class_config.arg = 'new value'  # Further modification to `class_config`.
-      partial_class = build(partial_config)
-      instance = partial_class()
-      assert instance.arg == 'arg'  # The instance config is still 'arg'.
-  """
-
-  # NOTE(b/201159339): We currently need to repeat this annotation for pytype.
-  __fn_or_cls__: TypeOrCallableProducingT[T]
-
-  def __build__(self, *args, **kwargs):
-    """Builds this ``Partial`` for the given ``args`` and ``kwargs``.
-
-    This method is called during ``build`` to get the output for this
-    ``Partial``.
-
-    Args:
-      *args: Positional arguments to partially bind to ``self.__fn_or_cls__``.
-      **kwargs: Keyword arguments to partially bind to ``self.__fn_or_cls__``.
-
-    Returns:
-      A partial object (``functools.partial`` or ``arg_factory.partial``) for
-      the callable ``self.__fn_or_cls__``, which binds the positional arguments
-      ``args`` and the keyword arguments ``kwargs``.
-    """
-    return _build_partial(self.__fn_or_cls__, args, kwargs)
-
-
-class ArgFactory(Generic[T], Buildable[T]):
-  """A configuration that creates an argument factory when built.
-
-  When an ``ArgFactory`` is used as a parameter for a ``fdl.Partial``, the
-  partial function built from that ``fdl.Partial`` will construct a new value
-  for the parameter each time it is called.  For example:
-
-  >>> def f(x, noise): return x + noise
-  >>> cfg = fdl.Partial(f, noise=fdl.ArgFactory(random.random))
-  >>> p = fdl.build(cfg)
-  >>> p(5) == p(5)  # noise has a different value for each call to `p`.
-  False
-
-  In contrast, if we replaced ``fdl.ArgFactory`` with ``fdl.Config`` in the
-  above example, then the same noise value would be added each time ``p`` is
-  called, since ``random.random`` would be called when ``fdl.build(cfg)`` is
-  called.
-
-  ``ArgFactory``'s can also be nested inside containers that are parameter
-  values for a ``Partial``.  In this case, the partial function will construct
-  the parameter value by copying the containers and replacing any ``ArgFactory``
-  with the result of calling its factory.  Only the containers that (directly or
-  indirectly) contain ``ArgFactory``'s are copied; any elements of the
-  containers that do not contain ``ArgFactory``'s are not copied.
-
-  ``ArgFactory`` can also be used as the parameter for another ``ArgFactory``,
-  in which case a new value will be constructed for the child argument
-  each time the parent argument is created.
-
-  ``ArgFactory`` should *not* be used as a top-level configuration object, or
-  as the argument to a ``fdl.Config``.
-  """
-
-  # TODO(b/272077508): Update build to raise an exception if ArgFactory is built
-  # in an inappropriate context.
-
-  # NOTE(b/201159339): We currently need to repeat this annotation for pytype.
-  __fn_or_cls__: TypeOrCallableProducingT[T]
-
-  def __build__(self, *args, **kwargs):
-    if args or kwargs:
-      return _BuiltArgFactory(_build_partial(self.__fn_or_cls__, args, kwargs))
-    else:
-      return _BuiltArgFactory(self.__fn_or_cls__)
-
-
 def _field_uses_default_factory(dataclass_type: Type[Any], field_name: str):
   """Returns true if <dataclass_type>.<field_name> uses a default_factory."""
   for field in dataclasses.fields(dataclass_type):
     if field.name == field_name:
       return field.default_factory != dataclasses.MISSING
   return False
 
 
-def update_callable(
-    buildable: Buildable,
-    new_callable: TypeOrCallableProducingT,
-    drop_invalid_args: bool = False,
-):
-  """Updates ``config`` to build ``new_callable`` instead.
-
-  When extending a base configuration, it can often be useful to swap one class
-  for another. For example, an experiment may want to swap in a subclass that
-  has augmented functionality.
-
-  ``update_callable`` updates ``config`` in-place (preserving argument history).
-
-  Args:
-    buildable: A ``Buildable`` (e.g. a ``fdl.Config``) to mutate.
-    new_callable: The new callable ``config`` should call when built.
-    drop_invalid_args: If True, arguments that don't exist in the new callable
-      will be removed from buildable. If False, raise an exception for such
-      arguments.
-
-  Raises:
-    TypeError: if ``new_callable`` has varargs, or if there are arguments set on
-      ``config`` that are invalid to pass to ``new_callable``.
-  """
-  # Note: can't just call config.__init__(new_callable, **config.__arguments__)
-  # to preserve history.
-  #
-  # Note: can't call `setattr` on all the args to validate them, because that
-  # will result in duplicate history entries.
-  original_args = buildable.__arguments__
-  signature = signatures.get_signature(new_callable)
-  if any(
-      param.kind == param.VAR_POSITIONAL
-      for param in signature.parameters.values()
-  ):
-    raise NotImplementedError(
-        'Variable positional arguments (aka `*args`) not supported.'
-    )
-  has_var_keyword = any(
-      param.kind == param.VAR_KEYWORD for param in signature.parameters.values()
-  )
-  if not has_var_keyword:
-    invalid_args = [
-        arg for arg in original_args.keys() if arg not in signature.parameters
-    ]
-    if invalid_args:
-      if drop_invalid_args:
-        for arg in invalid_args:
-          delattr(buildable, arg)
-      else:
-        raise TypeError(
-            f'Cannot switch to {new_callable} (from '
-            f'{buildable.__fn_or_cls__}) because the Buildable would '
-            f'have invalid arguments {invalid_args}.'
-        )
-
-  object.__setattr__(buildable, '__fn_or_cls__', new_callable)
-  object.__setattr__(buildable, '__signature__', signature)
-  object.__setattr__(buildable, '_has_var_keyword', has_var_keyword)
-  buildable.__argument_history__.add_new_value('__fn_or_cls__', new_callable)
-
-
-def assign(buildable: Buildable, **kwargs):
-  """Assigns multiple arguments to ``buildable``.
-
-  Although this function does not enable a caller to do something they can't
-  already do with other syntax, this helper function can be useful when
-  manipulating deeply nested configs. Example::
-
-    cfg = # ...
-    fdl.assign(cfg.my.deeply.nested.child.object, arg_a=1, arg_b='b')
-
-  The above code snippet is equivalent to::
-
-    cfg = # ...
-    cfg.my.deeply.nested.child.object.arg_a = 1
-    cfg.my.deeply.nested.child.object.arg_b = 'b'
-
-  Args:
-    buildable: A ``Buildable`` (e.g. a ``fdl.Config``) to set values upon.
-    **kwargs: The arguments and values to assign.
-  """
-  for name, value in kwargs.items():
-    setattr(buildable, name, value)
-
-
 BuildableT = TypeVar('BuildableT', bound=Buildable)
 
 
-def copy_with(buildable: BuildableT, **kwargs) -> BuildableT:
-  """Returns a shallow copy of ``buildable`` with updates to arguments.
-
-  Args:
-    buildable: A ``Buildable`` (e.g. a ``fdl.Config``) to copy and mutate.
-    **kwargs: The arguments and values to assign.
-  """
-  buildable = copy.copy(buildable)
-  assign(buildable, **kwargs)
-  return buildable
-
-
-def deepcopy_with(buildable: Buildable, **kwargs):
-  """Returns a deep copy of ``buildable`` with updates to arguments.
-
-  Note: if any ``Config``'s inside ``buildable`` are shared with ``Config``'s
-  outside of ``buildable``, then they will no longer be shared in the returned
-  value. E.g., if ``cfg1.x.y is cfg2``, then
-  ``fdl.deepcopy_with(cfg1, ...).x.y is cfg2`` will be ``False``.
-
-  Args:
-    buildable: A ``Buildable`` (e.g. a ``fdl.Config``) to copy and mutate.
-    **kwargs: The arguments and values to assign.
-  """
-  buildable = copy.deepcopy(buildable)
-  assign(buildable, **kwargs)
-  return buildable
-
-
 def get_callable(buildable: Buildable[T]) -> Union[Callable[..., T], Type[T]]:
   """Returns the callable of a Buildable."""
   return buildable.__fn_or_cls__
 
 
 def ordered_arguments(
     buildable: Buildable,
     *,
     include_var_keyword: bool = True,
     include_defaults: bool = False,
     include_unset: bool = False,
-    exclude_equal_to_default: bool = False,
-) -> Dict[str, Any]:
+    include_positional: bool = True,
+    include_equal_to_default: bool = True,
+) -> Dict[Union[int, str], Any]:
   """Returns arguments of a Buildable, ordered by the signature.
 
   Args:
     buildable: The buildable whose arguments should be returned.
     include_var_keyword: If True, then include arguments that will be consumed
       by the buildable's callable's `VAR_KEYWORD` parameter (e.g. `**kwargs`).
     include_defaults: If True, then include arguments that have not been
       explicitly set, but that have a default value.  Can not be combined with
-      `exclude_equal_to_default=True`.
+      `include_equal_to_default=False`.
     include_unset: If True, then include arguments that have not been explicitly
       set, that don't have a default value.  The value for these parameters will
       be `fdl.NO_VALUE`.
-    exclude_equal_to_default: If True, then exclude arguments that are equal to
+    include_positional: If False, positional-only and variadic positional
+      arguments will be excluded from the output.
+    include_equal_to_default: If False, then exclude arguments that are equal to
       their default value (using `==`).  Can not be combined with
       `include_defaults=True`.
 
   Returns:
-    A dictionary mapping argument names to values or `fdl.NO_VALUE`.
+    A dictionary mapping argument keys to values or `fdl.NO_VALUE`. Argument
+    keys are either positional indices or names.
   """
-  if exclude_equal_to_default and include_defaults:
+  if not include_equal_to_default and include_defaults:
     raise ValueError(
-        'exclude_equal_to_default and include_defaults are mutually exclusive.'
+        'Exclude_equal_to_default and include_defaults are mutually exclusive.'
     )
   result = {}
-  for name, param in buildable.__signature__.parameters.items():
-    if param.kind != param.VAR_KEYWORD:
-      if name in buildable.__arguments__:
-        value = buildable.__arguments__[name]
-        if (not exclude_equal_to_default) or (value != param.default):
-          result[name] = value
+  unset = object()
+  for index, (name, param) in enumerate(
+      buildable.__signature_info__.parameters.items()
+  ):
+    if param.kind not in (param.VAR_POSITIONAL, param.VAR_KEYWORD):
+      value = unset
+      if name in buildable.__arguments__ or (
+          index in buildable.__arguments__
+          and param.kind == param.POSITIONAL_ONLY
+      ):
+        if name in buildable.__arguments__:
+          value = buildable.__arguments__[name]
+        else:
+          value = buildable.__arguments__[index]
       elif param.default is not param.empty:
         if include_defaults:
-          result[name] = param.default
+          value = param.default
       elif include_unset:
-        result[name] = NO_VALUE
+        value = NO_VALUE
+      if value is not unset:
+        if include_equal_to_default or (value != param.default):
+          if param.kind == param.POSITIONAL_ONLY:
+            result[index] = value
+          else:
+            result[name] = value
+
+    if param.kind == param.VAR_POSITIONAL:
+      # Cannot add defaults for *args in Python, so ignore defaults related
+      # flags and `include_unset` flag here.
+      while index in buildable.__arguments__:
+        result[index] = buildable.__arguments__[index]
+        index += 1
+
   if include_var_keyword:
     for name, value in buildable.__arguments__.items():
-      param = buildable.__signature__.parameters.get(name)
+      param = buildable.__signature_info__.parameters.get(name)
       if param is None or param.kind == param.VAR_KEYWORD:
         result[name] = value
-  return result
-
-
-def add_tag(buildable: Buildable, argument: str, tag: tag_type.TagType) -> None:
-  """Tags `name` with `tag` in `buildable`."""
-  buildable.__validate_param_name__(argument)
-  buildable.__argument_tags__[argument].add(tag)
-  buildable.__argument_history__.add_updated_tags(
-      argument, buildable.__argument_tags__[argument]
-  )
-
-
-def set_tags(
-    buildable: Buildable, argument: str, tags: Collection[tag_type.TagType]
-) -> None:
-  """Sets tags for a parameter in `buildable`, overriding existing tags."""
-  clear_tags(buildable, argument)
-  for tag in tags:
-    add_tag(buildable, argument, tag)
-  buildable.__argument_history__.add_updated_tags(
-      argument, buildable.__argument_tags__[argument]
-  )
-
-
-def remove_tag(
-    buildable: Buildable, argument: str, tag: tag_type.TagType
-) -> None:
-  """Removes a given tag from a named argument of a Buildable."""
-  buildable.__validate_param_name__(argument)
-  field_tag_set = buildable.__argument_tags__[argument]
-  if tag not in field_tag_set:
-    raise ValueError(
-        f'{tag} not set on {argument}; current tags: {field_tag_set}.'
-    )
-  field_tag_set.remove(tag)
-  buildable.__argument_history__.add_updated_tags(
-      argument, buildable.__argument_tags__[argument]
-  )
-
-
-def clear_tags(buildable: Buildable, argument: str) -> None:
-  """Removes all tags from a named argument of a Buildable."""
-  buildable.__validate_param_name__(argument)
-  buildable.__argument_tags__[argument].clear()
-  buildable.__argument_history__.add_updated_tags(
-      argument, buildable.__argument_tags__[argument]
-  )
-
-
-def get_tags(
-    buildable: Buildable, argument: str
-) -> FrozenSet[tag_type.TagType]:
-  return frozenset(buildable.__argument_tags__[argument])
-
 
-_SUPPORTED_CASTS = set()
+  if not include_positional:
+    result = {k: v for k, v in result.items() if isinstance(k, str)}
 
-
-def cast(new_type: Type[BuildableT], buildable: Buildable) -> BuildableT:
-  """Returns a copy of ``buildable`` that has been converted to ``new_type``.
-
-  Requires that ``type(buildable)`` and ``type(new_type)`` be compatible.
-  If the types may not be compatible, a warning will be issued, but the
-  conversion will be attempted.
-
-  Args:
-    new_type: The type to convert to.
-    buildable: The ``Buildable`` that should be copied and converted.
-  """
-  if not isinstance(buildable, Buildable):
-    raise TypeError(f'Expected `buildable` to be a Buildable, got {buildable}')
-  if not isinstance(new_type, type) and issubclass(new_type, Buildable):
-    raise TypeError(
-        f'Expected `new_type` to be a subclass of Buildable, got {buildable}'
-    )
-  src_type = type(buildable)
-  if (src_type, new_type) not in _SUPPORTED_CASTS:
-    logging.warning(
-        (
-            'Conversion from %s to %s has not been marked as '
-            'officially supported.  If you think this conversion '
-            'should be supported, contact the Fiddle team.'
-        ),
-        src_type,
-        new_type,
-    )
-  return new_type.__unflatten__(*buildable.__flatten__())
-
-
-def register_supported_cast(src_type, dst_type):
-  _SUPPORTED_CASTS.add((src_type, dst_type))
-
-
-for _src_type, _dst_type in itertools.product(
-    [Config, Partial, ArgFactory], repeat=2
-):
-  register_supported_cast(_src_type, _dst_type)
+  return result
```

### Comparing `fiddle-0.2.9/fiddle/_src/config_test.py` & `fiddle-0.3.0/fiddle/_src/config_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,33 +9,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for the `fiddle.config` module."""
+"""Tests for the `fiddle._src.config` module."""
 
 import copy
 import dataclasses
-import functools
 import pickle
+import sys
 import threading
-from typing import Any, Callable, Dict, Generic, TypeVar
+from typing import Any, Dict, Generic, TypeVar
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
-from fiddle import arg_factory
 from fiddle import daglish
 from fiddle import history
 from fiddle._src import config as config_lib
 from fiddle._src.experimental import daglish_legacy
 from fiddle._src.testing.example import demo_configs
 import pytype_extensions
-from typing_extensions import Annotated
 
 
 class Tag1(fdl.Tag):
   """One tag."""
 
 
 class Tag2(fdl.Tag):
@@ -71,34 +69,32 @@
   return locals()
 
 
 def fn_with_var_args_and_kwargs(arg1, *args, kwarg1=None, **kwargs):  # pylint: disable=unused-argument
   return locals()
 
 
+def fn_with_args_and_kwargs_only(*args, **kwargs):  # pylint: disable=unused-argument
+  return locals()
+
+
+def fn_with_position_args(a, b=0, /, c=1, *args, kwarg1=None, **kwargs):  # pylint: disable=keyword-arg-before-vararg, unused-argument
+  return locals()
+
+
 def make_typed_config() -> fdl.Config[SampleClass]:
   """Helper function which returns a fdl.Config whose type is known."""
   return fdl.Config(SampleClass, arg1=1, arg2=2)
 
 
 def make_untyped_config(arg_to_configure, **kwargs) -> fdl.Config:
   """Helper function which returns an untyped fdl.Config."""
   return fdl.Config(arg_to_configure, **kwargs)
 
 
-def make_typed_partial() -> fdl.Partial[SampleClass]:
-  """Helper function to create a typed Partial instance."""
-  return fdl.Partial(SampleClass, arg1=1)
-
-
-def make_untyped_partial(arg_to_configure, **kwargs) -> fdl.Partial:
-  """Helper function which returns an untyped fdl.Config."""
-  return fdl.Partial(arg_to_configure, **kwargs)
-
-
 class Unserializable:
 
   def __getstate__(self):
     raise NotImplementedError()
 
 
 def _test_fn_unserializable_default(x=Unserializable()):
@@ -111,22 +107,14 @@
 
 
 @dataclasses.dataclass
 class DataclassParent:
   child: DataclassChild = dataclasses.field(default_factory=DataclassChild)
 
 
-@dataclasses.dataclass
-class DataclassAnnotated:
-  one: Annotated[int, Tag1]
-  two: Annotated[str, Tag1, Tag2]
-
-  three: 'Annotated[float, Tag2]'
-
-
 def raise_error():
   raise ValueError('My fancy exception')
 
 
 _T = TypeVar('_T')
 
 
@@ -152,24 +140,26 @@
     self.assertEqual(instance.arg1, 'arg1')
     self.assertEqual(instance.arg2, 'arg2')
     self.assertEqual(instance.kwarg1, 'kwarg1')
     self.assertEqual(instance.kwarg2, 'kwarg2')
 
   def test_config_for_functions(self):
     fn_config = fdl.Config(basic_fn, 1, kwarg2='kwarg2')
-    pytype_extensions.assert_type(fn_config, fdl.Config[Dict[str, Any]])
+    pytype_extensions.assert_type(
+        fn_config, fdl.Config[Dict[str, Any]]
+    )  # use-fiddle-overlay
     self.assertEqual(fn_config.arg1, 1)
     self.assertEqual(fn_config.kwarg2, 'kwarg2')
     fn_config.arg1 = 'arg1'
     self.assertEqual(fn_config.arg1, 'arg1')
     fn_config.arg2 = 'arg2'
     fn_config.kwarg1 = 'kwarg1'
 
     result = fdl.build(fn_config)
-    pytype_extensions.assert_type(result, Dict[str, Any])
+    pytype_extensions.assert_type(result, Dict[str, Any])  # use-fiddle-overlay
     self.assertEqual(result, {
         'arg1': 'arg1',
         'arg2': 'arg2',
         'kwarg1': 'kwarg1',
         'kwarg2': 'kwarg2'
     })
 
@@ -212,22 +202,226 @@
     })
 
   def test_config_for_functions_with_var_args_and_kwargs(self):
     fn_config = fdl.Config(fn_with_var_args_and_kwargs, arg1='arg1')
     fn_args = fdl.build(fn_config)
     self.assertEqual(fn_args['arg1'], 'arg1')
 
-    fn_config.args = 'kwarg_called_arg'
     fn_config.kwargs = 'kwarg_called_kwarg'
     fn_args = fdl.build(fn_config)
     self.assertEqual(fn_args['kwargs'], {
-        'args': 'kwarg_called_arg',
         'kwargs': 'kwarg_called_kwarg'
     })
 
+  def test_positional_args_access(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    self.assertEqual(fn_config[0], 1)
+    self.assertEqual(fn_config[-1], 5)
+    self.assertSequenceEqual(fn_config[3:], [4, 5])
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3, 4, 5])
+
+  def test_positional_args_modification(self):
+    with self.subTest('with_var_positional'):
+      fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+      fn_config[0] = 0
+      self.assertSequenceEqual(fn_config[:], [0, 2, 3, 4, 5])
+      fn_config[:3] = [5, 6, 7]
+      self.assertSequenceEqual(fn_config[:], [5, 6, 7, 4, 5])
+      fn_config[3:] = [8, 9, 10]
+      self.assertSequenceEqual(fn_config[:], [5, 6, 7, 8, 9, 10])
+      fn_config[:] = [1, 2, 3, 4, 5, 6]
+      self.assertSequenceEqual(fn_config[:], [1, 2, 3, 4, 5, 6])
+
+    with self.subTest('wo_var_positional'):
+
+      def foo(a, b, /, c):
+        return a, b, c
+
+      fn_config = fdl.Config(foo, 1, 2, 3)
+      fn_config[0] = 0
+      self.assertSequenceEqual(fn_config[:], [0, 2, 3])
+      fn_config[:2] = [4, 5]
+      self.assertSequenceEqual(fn_config[:], [4, 5, 3])
+
+  def test_positional_args_delete(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5, 6)
+    del fn_config[0]
+    self.assertEqual(fn_config[:], [config_lib.NO_VALUE, 2, 3, 4, 5, 6])
+    del fn_config[-1]
+    self.assertEqual(fn_config[:], [config_lib.NO_VALUE, 2, 3, 4, 5])
+    del fn_config[3:]
+    self.assertEqual(fn_config[:], [config_lib.NO_VALUE, 2, 3])
+
+  def test_negative_index_access(self):
+    fn_config = fdl.Config(fn_with_position_args, 0, 1, 2, 3, 4, 5)
+    del fn_config.c
+    self.assertEqual(fn_config[:], [0, 1, 1, 3, 4, 5])
+    self.assertEqual(fn_config[-1], 5)
+    self.assertEqual(fn_config[-6], 0)
+
+  def test_negative_index_modify(self):
+    fn_config = fdl.Config(fn_with_position_args, 0, 1, 2, 3, 4, 5)
+    del fn_config.c
+    self.assertEqual(fn_config[:], [0, 1, 1, 3, 4, 5])
+    fn_config[-1] = -5
+    self.assertEqual(fn_config[:], [0, 1, 1, 3, 4, -5])
+    fn_config[-6] = 6
+    self.assertEqual(fn_config[:], [6, 1, 1, 3, 4, -5])
+
+  def test_modify_positional_only_args(self):
+    def foo(a, b, c, /):
+      return a, b, c
+
+    fn_config = fdl.Config(foo)
+    fn_config[2] = 5
+    self.assertEqual(
+        fn_config[:], [config_lib.NO_VALUE, config_lib.NO_VALUE, 5]
+    )
+
+  def test_negative_index_delete(self):
+    fn_config = fdl.Config(fn_with_position_args, 0, 1, 2, 3, 4, 5)
+    del fn_config.c
+    self.assertEqual(fn_config[:], [0, 1, 1, 3, 4, 5])
+    del fn_config[-1]
+    self.assertEqual(fn_config[:], [0, 1, 1, 3, 4])
+    del fn_config[-5]
+    self.assertEqual(
+        fn_config[:],
+        [config_lib.NO_VALUE, 1, 1, 3, 4],
+    )
+
+  def test_varargs_index_handle_access(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    self.assertEqual(fn_config[fdl.VARARGS], 4)
+    self.assertSequenceEqual(fn_config[fdl.VARARGS :], [4, 5])
+
+  def test_varargs_index_handle_modify(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    fn_config[fdl.VARARGS :] = []
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3])
+    fn_config[fdl.VARARGS :] = [7, 8, 9]
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3, 7, 8, 9])
+    fn_config[fdl.VARARGS] = 0
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3, 0, 8, 9])
+
+  def test_varargs_index_handle_delete(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    del fn_config[fdl.VARARGS]
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3, 5])
+    del fn_config[fdl.VARARGS :]
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3])
+
+  def test_modification_when_var_args_are_empty(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3)
+    self.assertEmpty(fn_config[fdl.VARARGS :])
+    fn_config[fdl.VARARGS :] = ['a', 'b', 'c']
+    self.assertSequenceEqual(fn_config[:], [1, 2, 3, 'a', 'b', 'c'])
+
+  def test_only_some_positional_args_are_defined(self):
+    fn_cfg = config_lib.Config(fn_with_position_args, 0)
+    self.assertEqual(fn_cfg[:], [0, 0, 1])
+    fn_cfg[:2] = [5, 6]
+    self.assertEqual(fn_cfg[:], [5, 6, 1])
+
+  def test_positional_args_direct_access_is_forbidden(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    with self.assertRaisesRegex(
+        AttributeError,
+        'Cannot access positional-only or variadic positional arguments',
+    ):
+      _ = fn_config.args
+
+    with self.assertRaisesRegex(
+        AttributeError,
+        'Cannot access positional-only or variadic positional arguments',
+    ):
+      _ = fn_config.a
+
+  def test_positional_args_direct_modification_is_forbidden(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    with self.assertRaisesRegex(
+        AttributeError, 'Cannot access VAR_POSITIONAL parameter'
+    ):
+      fn_config.args = [0]
+
+    with self.assertRaisesRegex(
+        AttributeError, 'Cannot access POSITIONAL_ONLY parameter'
+    ):
+      fn_config.a = 0
+
+  def test_positional_or_keyword_args_have_consistent_values(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    fn_config[2] = 'arg-c'
+    self.assertEqual(fn_config.c, 'arg-c')
+    fn_config.c = 'index-2'
+    self.assertEqual(fn_config[2], 'index-2')
+
+  def test_set_out_of_range_index(self):
+    fn_config = config_lib.Config(fn_with_position_args)
+    arr = [1, 2, 3]
+    added = [7, 8, 9]
+    fn_config[:3] = arr
+    fn_config[10:] = added
+    arr[10:] = added
+    self.assertSequenceEqual(fn_config[:], arr)
+
+  def test_index_out_of_range(self):
+    fn_config = fdl.Config(fn_with_var_args, 1, 2)
+    self.assertLen(fn_config[:], 2)
+    with self.assertRaisesRegex(IndexError, 'index out of range'):
+      fn_config[2] = 'index-2'
+    with self.assertRaisesRegex(IndexError, 'index out of range'):
+      _ = fn_config[2]
+
+  def test_args_config_shallow_copy(self):
+    fn_config = fdl.Config(fn_with_var_args, 1, 2)
+    self.assertLen(fn_config[:], 2)
+    a_copy = fn_config[:]
+    a_copy.append('3')
+    self.assertLen(fn_config[:], 2)
+    self.assertLen(a_copy, 3)
+
+  def test_args_config_build(self):
+    fn_config = fdl.Config(fn_with_position_args, 1, 2, 3, 4, 5)
+    self.assertEqual(
+        fdl.build(fn_config),
+        {'a': 1, 'b': 2, 'c': 3, 'args': (4, 5), 'kwarg1': None, 'kwargs': {}},
+    )
+
+  def test_nested_positional_args_config_build(self):
+    fn_config = fdl.Config(
+        fn_with_position_args,
+        1,
+        2,
+        3,
+        4,
+        5,
+        kwarg1=fdl.Config(
+            fn_with_position_args, 'a', 'b', kwarg1='kwarg1', kwarg2='kwarg2'
+        ),
+    )
+    self.assertEqual(
+        fdl.build(fn_config),
+        {
+            'a': 1,
+            'b': 2,
+            'c': 3,
+            'args': (4, 5),
+            'kwarg1': {
+                'a': 'a',
+                'b': 'b',
+                'c': 1,
+                'kwarg1': 'kwarg1',
+                'args': tuple(),
+                'kwargs': {'kwarg2': 'kwarg2'},
+            },
+            'kwargs': {},
+        },
+    )
+
   def test_config_for_dicts(self):
     dict_config = fdl.Config(dict, a=1, b=2)
     dict_config.c = 3
     instance = fdl.build(dict_config)
     self.assertEqual(instance, {'a': 1, 'b': 2, 'c': 3})
 
   def test_config_with_default_args(self):
@@ -333,16 +527,16 @@
     class_config = fdl.Config(SampleClass, 'arg1', 'arg2')
     fn_config = fdl.Config(basic_fn, class_config, 'fn_arg2')
     fn_config_copy = copy.copy(fn_config)
     # Changing the copy doesn't change the original.
     fn_config_copy.arg2 = 'fn_arg2_copy'
     self.assertEqual(fn_config.arg2, 'fn_arg2')
     # But modifying a shared value is seen by both.
-    fn_config_copy.arg1.arg2 = 'mutated'
-    self.assertEqual(fn_config.arg1.arg2, 'mutated')
+    fn_config_copy.arg1.arg2 = 'mutated'  # pytype: disable=not-writable  # use-fiddle-overlay
+    self.assertEqual(fn_config.arg1.arg2, 'mutated')  # pytype: disable=attribute-error  # use-fiddle-overlay
 
   def test_buildable_subclass(self):
 
     class SampleClassConfig(fdl.Config):
 
       def __init__(self, *args, **kwargs):
         super().__init__(SampleClass, *args, **kwargs)
@@ -388,36 +582,25 @@
     class_config = fdl.Config(SampleClass, 'arg1', 'arg2')
     fn_config = fdl.Config(basic_fn, class_config, 'fn_arg2')
     fn_config_copy = copy.deepcopy(fn_config)
     # Changing the copy doesn't change the original.
     fn_config_copy.arg2 = 'fn_arg2_copy'
     self.assertEqual(fn_config.arg2, 'fn_arg2')
     # With a deep copy, the value is no longer shared.
-    fn_config_copy.arg1.arg2 = 'mutated'
-    self.assertEqual(fn_config.arg1.arg2, 'arg2')
+    fn_config_copy.arg1.arg2 = 'mutated'  # pytype: disable=not-writable  # use-fiddle-overlay
+    self.assertEqual(fn_config.arg1.arg2, 'arg2')  # pytype: disable=attribute-error  # use-fiddle-overlay
 
   def test_deep_copy_preserves_instance_sharing(self):
     class_config = fdl.Config(SampleClass, 'arg1', 'arg2')
     fn_config = fdl.Config(basic_fn, arg1=class_config, arg2=class_config)
     self.assertIs(fn_config.arg1, fn_config.arg2)
     fn_config_copy = copy.deepcopy(fn_config)
     self.assertIsNot(fn_config.arg1, fn_config_copy.arg1)
     self.assertIs(fn_config_copy.arg1, fn_config_copy.arg2)
 
-  def test_deep_copy_partials(self):
-    class_partial = fdl.Partial(SampleClass, 'arg1', 'arg2')
-    fn_config = fdl.Config(
-        basic_fn,
-        arg1=fdl.cast(fdl.Config, class_partial),
-        arg2=fdl.cast(fdl.Config, class_partial))
-    self.assertIsNot(fn_config.arg1, fn_config.arg2)
-    fn_config_copy = copy.deepcopy(fn_config)
-    self.assertIsNot(fn_config_copy.arg1, fn_config_copy.arg2)
-    self.assertIsNot(fn_config.arg1, fn_config_copy.arg1)
-
   def test_deep_copy_no_value(self):
     self.assertIs(fdl.NO_VALUE, copy.copy(fdl.NO_VALUE))
     self.assertIs(fdl.NO_VALUE, copy.deepcopy(fdl.NO_VALUE))
 
   def test_equality_arguments(self):
     cfg1 = fdl.Config(SampleClass, 'arg1')
     cfg2 = fdl.Config(SampleClass, 'arg1')
@@ -439,17 +622,17 @@
       fn_config2 = fdl.Config(
           basic_fn, arg1=fdl.cast(fdl.Partial, class_config), arg2=class_config)
       return fn_config2
 
     cfg1 = make_nested_config()
     cfg2 = make_nested_config()
     self.assertEqual(cfg1, cfg2)
-    cfg2.arg2.arg1.kwarg1 = 'another value'
+    cfg2.arg2.arg1.kwarg1 = 'another value'  # pytype: disable=attribute-error  # use-fiddle-overlay
     self.assertNotEqual(cfg1, cfg2)
-    cfg1.arg2.arg1.kwarg1 = 'another value'
+    cfg1.arg2.arg1.kwarg1 = 'another value'  # pytype: disable=attribute-error  # use-fiddle-overlay
     self.assertEqual(cfg1, cfg2)
 
   def test_equality_fn_or_cls_mismatch(self):
     cls_cfg = fdl.Config(SampleClass, 'arg1')
     fn_cfg = fdl.Config(basic_fn, 'arg1')
     self.assertNotEqual(cls_cfg, fn_cfg)
 
@@ -472,28 +655,41 @@
     # The logic governing how __eq__ is actually invoked from an == comparison
     # actually takes subclassing relationships into account and always calls
     # b.__eq__(a) if isinstance(b, a.__class__), so testing explicitly here.
     self.assertFalse(cfg.__eq__(cfg_subclass))
     self.assertFalse(cfg_subclass.__eq__(cfg))
 
   def test_equality_classmethods(self):
-    cfg_a = fdl.Config(SampleClass.a_classmethod)
-    cfg_b = fdl.Config(SampleClass.a_classmethod)
+    cfg_a = fdl.Config(SampleClass.a_classmethod)  # pytype: disable=invalid-annotation  # use-fiddle-overlay
+    cfg_b = fdl.Config(SampleClass.a_classmethod)  # pytype: disable=invalid-annotation  # use-fiddle-overlay
+    self.assertEqual(cfg_a, cfg_b)
+
+  def test_equality_positional_args_default_value(self):
+    cfg_a = fdl.Config(fn_with_position_args, 'a')
+    cfg_b = fdl.Config(fn_with_position_args, 'a', 0)
+    cfg_c = fdl.Config(fn_with_position_args, 'a', c=1)
+    cfg_d = fdl.Config(fn_with_position_args, 'a', 0, 1, 2, 3, 4, 5)
     self.assertEqual(cfg_a, cfg_b)
+    self.assertEqual(cfg_a, cfg_c)
+    self.assertNotEqual(cfg_a, cfg_d)
 
   def test_default_value_equality(self):
     cfg1 = fdl.Config(SampleClass, 1, 2)
     cfg2 = fdl.Config(SampleClass, 1, 2, None, kwarg2=None)
     self.assertEqual(cfg1, cfg2)
 
     cfg1 = fdl.Config(basic_fn, 1, 2)
     cfg2 = fdl.Config(basic_fn, 1, 2, None, kwarg2=None)
     self.assertEqual(cfg1, cfg2)
 
-  def test_default_value_for_generic_classes(self):
+  def test_generic_classes(self):
+    if sys.version_info >= (3, 9):
+      cfg = fdl.Config(GenericClass, 1)
+      self.assertEqual(fdl.build(cfg), GenericClass(1))
+
     self.assertEqual(fdl.Config(GenericClass).x, 1)
     self.assertEqual(fdl.Config(GenericClass[int]).x, 1)
 
   def test_config_with_non_comparable_values(self):
     # This test ensures that fdl.Config and fdl.build work properly with
     # argument defaults that don't support equality testing. Something related
     # can come up with NumPy arrays, which test for equality against scalars in
@@ -558,108 +754,14 @@
       del fn_config.arg1
 
     with self.assertRaisesRegex(AttributeError, "'unknown_arg'"):
       del fn_config.unknown_arg
 
     self.assertEqual(4, fn_config.arg2)
 
-  def test_tagging(self):
-    cfg = fdl.Config(SampleClass)
-    fdl.add_tag(cfg, 'arg1', Tag1)
-
-    self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'arg1'))
-    self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'arg2'))
-
-    fdl.add_tag(cfg, 'arg1', Tag2)
-    self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg, 'arg1'))
-
-    fdl.remove_tag(cfg, 'arg1', Tag2)
-    self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'arg1'))
-
-    with self.assertRaisesRegex(ValueError, '.*not set.*'):
-      fdl.remove_tag(cfg, 'arg1', Tag2)
-
-  def test_tag_annotations(self):
-    cfg = fdl.Config(DataclassAnnotated)
-
-    self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'one'))
-    self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg, 'two'))
-    self.assertEqual(frozenset([Tag2]), fdl.get_tags(cfg, 'three'))
-
-  def test_tags_flattening_and_unflattening(self):
-    def flatten_unflatten(config):
-      values, metadata = config.__flatten__()
-      return type(config).__unflatten__(values, metadata)
-
-    with self.subTest('tagged_field_without_value'):
-      cfg = fdl.Config(DataclassAnnotated)
-      self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'one'))
-      cfg2 = flatten_unflatten(cfg)
-      self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg2, 'one'))
-
-    with self.subTest('untagged_field_without_value'):
-      cfg = fdl.Config(DataclassAnnotated)
-      fdl.clear_tags(cfg, 'one')
-      self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'one'))
-      cfg2 = flatten_unflatten(cfg)
-      self.assertEqual(frozenset([]), fdl.get_tags(cfg2, 'one'))
-
-    with self.subTest('tagged_field_with_value'):
-      cfg = fdl.Config(DataclassAnnotated)
-      cfg.one = fdl.TaggedValue([Tag2], 3)
-      self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg, 'one'))
-      cfg2 = flatten_unflatten(cfg)
-      self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(cfg2, 'one'))
-
-    with self.subTest('untagged_field_with_value'):
-      cfg = fdl.Config(DataclassAnnotated)
-      cfg.one = 3
-      fdl.clear_tags(cfg, 'one')
-      self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'one'))
-      cfg2 = flatten_unflatten(cfg)
-      self.assertEqual(frozenset([]), fdl.get_tags(cfg2, 'one'))
-
-  def test_setting_tagged_values_with_daglish_traversal(self):
-    cfg = fdl.Config(DataclassAnnotated, one=3)
-
-    def traverse(value, state):
-      if isinstance(value, int):
-        return fdl.TaggedValue([Tag2], value)
-      else:
-        return state.map_children(value)
-
-    # We expect the TaggedValue class *not* to be unwrapped by the constructor
-    # now, because __new__ is called directly.
-    cfg2 = traverse(cfg, daglish.MemoizedTraversal.begin(traverse, cfg))
-    self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg2, 'one'))
-    self.assertEqual(frozenset([Tag2]), fdl.get_tags(cfg2.one, 'value'))
-
-  def test_clear_tags(self):
-    cfg = fdl.Config(SampleClass)
-    fdl.add_tag(cfg, 'arg1', Tag1)
-    fdl.add_tag(cfg, 'arg1', Tag2)
-    fdl.clear_tags(cfg, 'arg1')
-    self.assertEqual(frozenset([]), fdl.get_tags(cfg, 'arg1'))
-
-  def test_set_tags(self):
-    cfg = fdl.Config(SampleClass)
-    fdl.add_tag(cfg, 'arg1', Tag1)
-    fdl.add_tag(cfg, 'arg1', Tag2)
-    fdl.set_tags(cfg, 'arg1', {Tag2})
-    self.assertEqual(frozenset([Tag2]), fdl.get_tags(cfg, 'arg1'))
-
-  def test_flatten_unflatten_tags(self):
-    cfg = fdl.Config(SampleClass)
-    fdl.add_tag(cfg, 'arg1', Tag1)
-    values, metadata = cfg.__flatten__()
-    copied = fdl.Config.__unflatten__(values, metadata)
-    fdl.add_tag(copied, 'arg1', Tag2)
-    self.assertEqual(frozenset([Tag1]), fdl.get_tags(cfg, 'arg1'))
-    self.assertEqual(frozenset([Tag1, Tag2]), fdl.get_tags(copied, 'arg1'))
-
   def test_flatten_unflatten_histories(self):
     cfg = fdl.Config(SampleClass)
     cfg.arg1 = 4
     cfg.arg1 = 5
     values, metadata = cfg.__flatten__()
     copied = fdl.Config.__unflatten__(values, metadata)
     self.assertEqual(
@@ -679,53 +781,14 @@
     self.assertEqual(['arg1', 'arg2', 'kwarg1', 'kwarg2'], dir(cfg))
 
   def test_dir_var_args_and_kwargs(self):
     varargs_config = fdl.Config(fn_with_var_args_and_kwargs)
     varargs_config.abc = '123'
     self.assertEqual(['abc', 'arg1', 'kwarg1'], dir(varargs_config))
 
-  def test_partial_for_classes(self):
-    class_partial = fdl.Partial(SampleClass, 'arg1', 'arg2')
-    pytype_extensions.assert_type(class_partial, fdl.Partial[SampleClass])
-    partial = fdl.build(class_partial)
-    pytype_extensions.assert_type(partial, Callable[..., SampleClass])
-    instance = partial()
-    pytype_extensions.assert_type(instance, SampleClass)
-    self.assertIsInstance(partial, functools.partial)
-    self.assertIsInstance(instance, SampleClass)
-    self.assertEqual(instance.arg1, 'arg1')
-    self.assertEqual(instance.arg2, 'arg2')
-
-    # We can override parameters at the call site.
-    instance = partial(arg1='new_arg1', arg2='new_arg2', kwarg1='new_kwarg1')
-    self.assertEqual(instance.arg1, 'new_arg1')
-    self.assertEqual(instance.arg2, 'new_arg2')
-    self.assertEqual(instance.kwarg1, 'new_kwarg1')
-
-  def test_partial_for_functions(self):
-    fn_partial = fdl.Partial(basic_fn, 1, kwarg2='kwarg2')
-    pytype_extensions.assert_type(fn_partial, fdl.Partial[Dict[str, Any]])
-    self.assertEqual(fn_partial.arg1, 1)
-    self.assertEqual(fn_partial.kwarg2, 'kwarg2')
-    fn_partial.arg1 = 'arg1'
-    self.assertEqual(fn_partial.arg1, 'arg1')
-    fn_partial.arg2 = 'arg2'
-    fn_partial.kwarg1 = 'kwarg1'
-
-    partial = fdl.build(fn_partial)
-    pytype_extensions.assert_type(partial, Callable[..., Dict[str, Any]])
-    value = partial()
-    pytype_extensions.assert_type(value, Dict[str, Any])
-    self.assertEqual(value, {
-        'arg1': 'arg1',
-        'arg2': 'arg2',
-        'kwarg1': 'kwarg1',
-        'kwarg2': 'kwarg2'
-    })
-
   def test_typed_config(self):
     class_config = make_typed_config()
     pytype_extensions.assert_type(class_config, fdl.Config[SampleClass])
     instance = fdl.build(class_config)
     pytype_extensions.assert_type(instance, SampleClass)
     self.assertEqual(instance.arg1, 1)
     self.assertEqual(instance.arg2, 2)
@@ -734,55 +797,14 @@
     class_config = make_untyped_config(SampleClass, arg1=2, arg2=3)
     pytype_extensions.assert_type(class_config, fdl.Config)
     instance = fdl.build(class_config)
     pytype_extensions.assert_type(instance, Any)
     self.assertEqual(instance.arg1, 2)
     self.assertEqual(instance.arg2, 3)
 
-  def test_typed_partial(self):
-    class_partial = make_typed_partial()
-    pytype_extensions.assert_type(class_partial, fdl.Partial[SampleClass])
-    partial = fdl.build(class_partial)
-    pytype_extensions.assert_type(partial, Callable[..., SampleClass])
-    instance = partial(arg2=4)
-    self.assertEqual(instance.arg1, 1)
-    self.assertEqual(instance.arg2, 4)
-
-  def test_untyped_partial(self):
-    class_partial = make_untyped_partial(SampleClass, arg1=2)
-    pytype_extensions.assert_type(class_partial, fdl.Partial)
-    partial = fdl.build(class_partial)
-    pytype_extensions.assert_type(partial, Callable[..., Any])
-    instance = partial(arg2=4)
-    self.assertEqual(instance.arg1, 2)
-    self.assertEqual(instance.arg2, 4)
-
-  def test_convert_partial(self):
-    class_partial = fdl.Partial(SampleClass, 'arg1', 'arg2')
-    class_config = fdl.cast(fdl.Config, class_partial)
-    class_config.arg1 = 'new_arg1'
-    class_config.arg2 = 'new_arg2'
-    class_config.kwarg1 = 'new_kwarg1'
-    self.assertEqual(class_partial.arg2, 'arg2')
-    instance = fdl.build(class_config)
-    self.assertEqual(instance.arg1, 'new_arg1')
-    self.assertEqual(instance.arg2, 'new_arg2')
-    self.assertEqual(instance.kwarg1, 'new_kwarg1')
-
-  def test_convert_partial_nested(self):
-    class_partial = fdl.Partial(SampleClass, 'arg1', 'arg2')
-    class_config = fdl.Config(SampleClass, fdl.cast(fdl.Config, class_partial),
-                              fdl.cast(fdl.Config, class_partial))
-    instance = fdl.build(class_config)
-    self.assertEqual(instance.arg1.arg1, 'arg1')
-    self.assertEqual(instance.arg1.arg2, 'arg2')
-    self.assertEqual(instance.arg2.arg1, 'arg1')
-    self.assertEqual(instance.arg2.arg2, 'arg2')
-    self.assertIsNot(instance.arg1, instance.arg2)
-
   def test_repr_class_config(self):
     class_config = fdl.Config(SampleClass, 1, 2, kwarg1='kwarg1')
     expected_repr = "<Config[SampleClass(arg1=1, arg2=2, kwarg1='kwarg1')]>"
     self.assertEqual(repr(class_config), expected_repr)
 
   def test_repr_nested_indentation(self):
     config = fdl.Config(basic_fn, 1,
@@ -795,79 +817,37 @@
     self.assertEqual(repr(config), expected_repr)
 
   def test_repr_fn_config(self):
     fn_config = fdl.Config(basic_fn, 1, 2, kwarg1='kwarg1')
     expected_repr = "<Config[basic_fn(arg1=1, arg2=2, kwarg1='kwarg1')]>"
     self.assertEqual(repr(fn_config), expected_repr)
 
-  def test_repr_class_partial(self):
-    class_partial = fdl.Partial(SampleClass, 1, 2, kwarg1='kwarg1')
-    expected_repr = "<Partial[SampleClass(arg1=1, arg2=2, kwarg1='kwarg1')]>"
-    self.assertEqual(repr(class_partial), expected_repr)
-
-  def test_repr_fn_partial(self):
-    fn_partial = fdl.Partial(basic_fn, 1, 2, kwarg1='kwarg1')
-    expected_repr = "<Partial[basic_fn(arg1=1, arg2=2, kwarg1='kwarg1')]>"
-    self.assertEqual(repr(fn_partial), expected_repr)
-
   def test_repr_varkwargs(self):
     # Note: in the repr, kwarg1 comes before x and y and z because kwarg1 is an
     # explicit keyword parameter, while x, y, and z are **kwargs parameters.
     cfg = fdl.Config(fn_with_var_kwargs, 1, x=2, z=3, y=4, kwarg1=5)
     expected_repr = (
         '<Config[fn_with_var_kwargs(arg1=1, kwarg1=5, x=2, z=3, y=4)]>')
     self.assertEqual(repr(cfg), expected_repr)
 
-  def test_repr_class_tags(self):
-    config = fdl.Config(
-        SampleClass,
-        1,
-        kwarg1='kwarg1',
-        kwarg2=fdl.Config(
-            SampleClass, 'nested value might be large so ' +
-            'put tag next to param, not after value.'))
-    fdl.add_tag(config, 'arg1', Tag1)
-    fdl.add_tag(config, 'arg2', Tag2)
-    fdl.add_tag(config, 'kwarg2', Tag1)
-    fdl.add_tag(config, 'kwarg2', Tag2)
-    expected_repr = """<Config[SampleClass(
-  arg1[#{module}.Tag1]=1,
-  arg2[#{module}.Tag2],
-  kwarg1='kwarg1',
-  kwarg2[#{module}.Tag1, #{module}.Tag2]=<Config[SampleClass(
-    arg1='nested value might be large so put tag next to param, not after value.')]>)]>"""
-    self.assertEqual(repr(config), expected_repr.format(module=__name__))
-
   def test_nonexistent_attribute_error(self):
     class_config = fdl.Config(SampleClass, 1)
     expected_msg = (r"No parameter 'nonexistent_arg' has been set on "
                     r'<Config\[SampleClass\(arg1=1\)\]>\.')
     with self.assertRaisesRegex(AttributeError, expected_msg):
       getattr(class_config, 'nonexistent_arg')
 
   def test_nonexistent_parameter_error(self):
     class_config = fdl.Config(SampleClass)
     expected_msg = (r"No parameter named 'nonexistent_arg' exists for "
                     r"<class '.*\.SampleClass'>; valid parameter names: "
                     r'arg1, arg2, kwarg1, kwarg2\.')
-    with self.assertRaisesRegex(TypeError, expected_msg):
+    with self.assertRaisesRegex(AttributeError, expected_msg):
       class_config.nonexistent_arg = 'error!'
 
-  def test_nonexistent_var_args_parameter_error(self):
-    fn_config = fdl.Config(fn_with_var_args)
-    expected_msg = (r'Variadic arguments \(e.g. \*args\) are not supported\.')
-    with self.assertRaisesRegex(TypeError, expected_msg):
-      fn_config.args = (1, 2, 3)
-
-  def test_unsupported_var_args_error(self):
-    expected_msg = (r'Variable positional arguments \(aka `\*args`\) not '
-                    r'supported\.')
-    with self.assertRaisesRegex(NotImplementedError, expected_msg):
-      fdl.Config(fn_with_var_args, 1, 2, 3)
-
   def test_build_inside_build(self):
 
     def inner_build(x: int) -> str:
       return str(x)
 
     def nest_call(x: int) -> str:
       cfg = fdl.Config(inner_build, x)
@@ -956,72 +936,42 @@
     """Bulidable types should be pickle-able."""
     cfg = fdl.Config(SampleClass, 1, 'abc')
     self.assertEqual(cfg, pickle.loads(pickle.dumps(cfg)))
     reloaded = pickle.loads(pickle.dumps(cfg))
     reloaded.kwarg1 = 3  # mutate after unpickling.
     self.assertNotEqual(cfg, reloaded)
 
-  def test_pickling_partial(self):
-    cfg = fdl.Partial(SampleClass)
-    cfg.arg1 = 'something'
-    self.assertEqual(cfg, pickle.loads(pickle.dumps(cfg)))
-
-  def test_pickling_composition(self):
-    cfg = fdl.Config(SampleClass, 1, 'abc')
-    cfg.kwarg2 = fdl.Partial(SampleClass)
-    cfg.kwarg2.arg1 = 'something'
-    self.assertEqual(cfg, pickle.loads(pickle.dumps(cfg)))
-
   def test_pickling_non_serializable_default(self):
     pickle.dumps(fdl.Config(_test_fn_unserializable_default))
 
   def test_build_nested_structure(self):
     class_config = fdl.Config(SampleClass, 'arg1', 'arg2')
     built = fdl.build([class_config, {'child': class_config}])
     self.assertIsInstance(built[0], SampleClass)
     self.assertEqual(built[0].arg1, 'arg1')
     self.assertEqual(built[0].arg2, 'arg2')
     self.assertIs(built[0], built[1]['child'])
 
   def test_build_raises_nice_error_too_few_args(self):
     cfg = fdl.Config(basic_fn, fdl.Config(SampleClass, 1), 2)
-    with self.assertRaisesRegex(
-        TypeError, r'.*missing 1 required.*\n\n.*<root>\.arg1.*arg1=1'):
-      fdl.build(cfg)
-
-  def test_build_reraises_nice_error_with_tag_information(self):
-    cfg = fdl.Config(SampleClass)
-    fdl.add_tag(cfg, 'arg2', Tag1)
-
-    with self.assertRaisesRegex(
-        TypeError,
-        r'.*Tags for unset arguments:\n - arg2: #{module}.Tag1.*'.format(
-            module=__name__
-        ),
-    ):
+    with self.assertRaises(TypeError) as e:
       fdl.build(cfg)
-
-  def test_build_reraises_nice_error_multiple_tags(self):
-    cfg = fdl.Config(SampleClass)
-    fdl.add_tag(cfg, 'arg1', Tag2)
-    fdl.add_tag(cfg, 'arg2', Tag1)
-    fdl.add_tag(cfg, 'arg2', Tag2)
-
-    expected_match = (
-        r'.* - arg1: #{module}.Tag2\n - arg2: #{module}.Tag1 #{module}.Tag2.*'
-        .format(module=__name__)
+    self.assertEqual(
+        e.exception.proxy_message,  # pytype: disable=attribute-error
+        '\n\nFiddle context: failed to construct or call SampleClass at '
+        '<root>.arg1 with positional arguments: (), keyword arguments: '
+        '(arg1=1).',
     )
-    with self.assertRaisesRegex(TypeError, expected_match):
-      fdl.build(cfg)
 
   def test_build_raises_exception_on_call(self):
     cfg = fdl.Config(raise_error)
     msg = (
         'My fancy exception\n\nFiddle context: failed to construct or call '
-        'raise_error at <root> with arguments ()'
+        'raise_error at <root> with positional arguments: (), '
+        'keyword arguments: ().'
     )
     with self.assertRaisesWithLiteralMatch(ValueError, msg):
       fdl.build(cfg)
 
   def test_build_error_path(self):
     # This will raise an error, because it doesn't have one arg populated.
     sub_cfg = fdl.Config(basic_fn, 1)
@@ -1030,15 +980,17 @@
 
     with self.assertRaises(TypeError) as e:
       fdl.build(cfg)
 
     self.assertEqual(
         e.exception.proxy_message,  # pytype: disable=attribute-error
         '\n\nFiddle context: failed to construct or call basic_fn at <root>.'
-        "arg1[1]['c'] with arguments (arg1=1)")
+        "arg1[1]['c'] with positional arguments: (), keyword arguments: "
+        '(arg1=1).',
+    )
 
   def test_multithreaded_build(self):
     """Two threads can each invoke build.build without interfering."""
     output = None
     background_entered_build = threading.Event()
     foreground_entered_build = threading.Event()
 
@@ -1062,77 +1014,19 @@
     thread = threading.Thread(target=other_thread)
     thread.start()
     obj = fdl.build(cfg)
     thread.join()
     self.assertEqual(1, obj)
     self.assertEqual(3, output)
 
-  def test_assign(self):
-    cfg = fdl.Config(fn_with_var_kwargs, 1, 2)
-    fdl.assign(cfg, a='a', b='b')
-    self.assertEqual({
-        'arg1': 1,
-        'kwarg1': 2,
-        'kwargs': {
-            'a': 'a',
-            'b': 'b'
-        }
-    }, fdl.build(cfg))
-
-  def test_assign_wrong_argument(self):
-    cfg = fdl.Config(basic_fn)
-    with self.assertRaisesRegex(TypeError, 'not_there'):
-      fdl.assign(cfg, arg1=1, not_there=2)
-
-  @parameterized.product(
-      from_type=[fdl.Config, fdl.Partial, fdl.ArgFactory],
-      to_type=[fdl.Config, fdl.Partial, fdl.ArgFactory],
-  )
-  def test_cast(self, from_type, to_type):
-    cfg1 = from_type(fn_with_var_kwargs, 1, 2)
-    fdl.add_tag(cfg1, 'arg1', Tag1)
-    cfg2 = fdl.cast(to_type, cfg1)
-    self.assertIsInstance(cfg2, to_type)
-    self.assertEqual(fdl.get_callable(cfg1), fdl.get_callable(cfg2))
-    self.assertEqual(cfg1.__arguments__, cfg2.__arguments__)
-    self.assertEqual(cfg1.__argument_tags__, cfg2.__argument_tags__)
-
-  def test_copy_with(self):
-    cfg1 = fdl.Config(fn_with_var_kwargs, 1, 2, c=[])
-    fdl.add_tag(cfg1, 'arg1', Tag1)
-
-    expected_cfg1 = dict(arg1=1, kwarg1=2, kwargs=dict(c=[]))
-    expected_cfg2 = dict(arg1=5, kwarg1=2, kwargs=dict(a='a', b='b', c=[]))
-
-    with self.subTest('cfg1_value'):
-      self.assertEqual(expected_cfg1, fdl.build(cfg1))
-
-    with self.subTest('shallow_copy'):
-      cfg2 = fdl.copy_with(cfg1, arg1=5, a='a', b='b')
-      self.assertIsNot(cfg1, cfg2)
-      self.assertIsNot(cfg1.__arguments__, cfg2.__arguments__)
-      self.assertIsNot(cfg1.__argument_tags__, cfg2.__argument_tags__)
-      self.assertEqual(cfg1.__argument_tags__, cfg2.__argument_tags__)
-      self.assertIs(cfg1.c, cfg2.c)  # Shallow copy.
-      self.assertEqual(expected_cfg2, fdl.build(cfg2))
-
-    with self.subTest('deep_copy'):
-      cfg2 = fdl.deepcopy_with(cfg1, arg1=5, a='a', b='b')
-      self.assertIsNot(cfg1, cfg2)
-      self.assertIsNot(cfg1.__arguments__, cfg2.__arguments__)
-      self.assertIsNot(cfg1.__argument_tags__, cfg2.__argument_tags__)
-      self.assertEqual(cfg1.__argument_tags__, cfg2.__argument_tags__)
-      self.assertIsNot(cfg1.c, cfg2.c)  # Deep copy.
-      self.assertEqual(expected_cfg2, fdl.build(cfg2))
-
   def test_copy_constructor_errors(self):
     cfg1 = fdl.Config(fn_with_var_kwargs, 1, 2)
     fdl.add_tag(cfg1, 'arg1', Tag1)
     with self.assertRaises(ValueError):
-      fdl.Partial(cfg1)
+      fdl.Partial(cfg1)  # pytype: disable=invalid-annotation  # use-fiddle-overlay
 
   def test_copy_constructor_with_updates_errors(self):
     cfg1 = fdl.Config(fn_with_var_kwargs, 1, 2, c=[])
     fdl.add_tag(cfg1, 'arg1', Tag1)
     with self.assertRaises(ValueError):
       fdl.Partial(cfg1, 5, a='a', b='b')
 
@@ -1148,138 +1042,136 @@
         cfg.child.x = 5
 
     with self.subTest('read_ok_after_override'):
       cfg.child = fdl.Config(DataclassChild)  # override default w/ a value
       cfg.child.x = 5  # now it's ok to configure child.
       self.assertEqual(fdl.build(cfg), DataclassParent(DataclassChild(5)))
 
-  @absltest.skip('Enable this after dropping pyhon 3.7 support')
-  def test_config_for_fn_with_special_arg_names(self):
-    # The reason that these tests pass is that we use positional-only
-    # parameters for self, etc. in functions such as Config.__build__.
-    # If we used keyword-or-positional parameters instead, then these
-    # tests would fail with a "multiple values for argument" TypeError.
-
-    def f(self, fn_or_cls, buildable=0):
-      return self + fn_or_cls + buildable
-
-    cfg = fdl.Config(f)
-    cfg.self = 100
-    cfg.fn_or_cls = 200
-    self.assertEqual(fdl.build(cfg), 300)
-
-    fdl.assign(cfg, buildable=10)  # pytype: disable=duplicate-keyword-argument
-    self.assertEqual(fdl.build(cfg), 310)
-
-    cfg2 = fdl.Config(f, self=5, fn_or_cls=1)  # pytype: disable=duplicate-keyword-argument
-    self.assertEqual(fdl.build(cfg2), 6)
-
-
-class CallableApisTest(absltest.TestCase):
-
-  def test_update_callable(self):
-    cfg = fdl.Config(basic_fn, 1, 'xyz', kwarg1='abc')
-    fdl.update_callable(cfg, SampleClass)
-    cfg.kwarg2 = '123'
-    obj = fdl.build(cfg)
-    self.assertIsInstance(obj, SampleClass)
-    self.assertEqual(1, obj.arg1)
-    self.assertEqual('xyz', obj.arg2)
-    self.assertEqual('abc', obj.kwarg1)
-    self.assertEqual('123', obj.kwarg2)
-
-  def test_update_callable_invalid_arg(self):
-    cfg = fdl.Config(fn_with_var_kwargs, abc='123', xyz='321')
-    with self.assertRaisesRegex(TypeError,
-                                r"have invalid arguments \['abc', 'xyz'\]"):
-      fdl.update_callable(cfg, SampleClass)
-
-  def test_update_callable_drop_invalid_arg(self):
-    cfg = fdl.Config(fn_with_var_kwargs, arg1='123', xyz='321')
-    fdl.update_callable(cfg, SampleClass, drop_invalid_args=True)
-    self.assertEqual(cfg, fdl.Config(SampleClass, arg1='123'))
-
-  def test_update_callable_new_kwargs(self):
-    cfg = fdl.Config(SampleClass)
-    cfg.arg1 = 1
-    fdl.update_callable(cfg, fn_with_var_kwargs)
-    cfg.abc = '123'  # A **kwargs value should now be allowed.
-    self.assertEqual({
-        'arg1': 1,
-        'kwarg1': None,
-        'kwargs': {
-            'abc': '123'
-        }
-    }, fdl.build(cfg))
-
-  def test_update_callable_varargs(self):
-    cfg = fdl.Config(fn_with_var_kwargs, 1, 2)
-    with self.assertRaisesRegex(NotImplementedError,
-                                'Variable positional arguments'):
-      fdl.update_callable(cfg, fn_with_var_args_and_kwargs)
-
-  def test_get_callable(self):
-    cfg = fdl.Config(basic_fn)
-    self.assertIs(fdl.get_callable(cfg), basic_fn)
-
 
 class OrderedArgumentsTest(parameterized.TestCase):
 
   def test_ordered_arguments(self):
-    cfg = fdl.Config(fn_with_var_kwargs)
-    cfg.var_kwarg1 = 3
+    cfg = fdl.Config(fn_with_position_args, 0, 1, 2, 3, 4)
+    cfg.var_kwarg1 = 5
     cfg.kwarg1 = 'hi'
-    cfg.arg1 = 4
-    cfg.var_kwarg2 = 0
+    cfg.var_kwarg2 = 6
+    cfg.c = -2
     self.assertEqual(
-        list(cfg.__arguments__.items()), [
-            ('var_kwarg1', 3),
+        list(cfg.__arguments__.items()),
+        [
+            ('c', -2),
+            (0, 0),
+            (1, 1),
+            (3, 3),
+            (4, 4),
+            ('var_kwarg1', 5),
             ('kwarg1', 'hi'),
-            ('arg1', 4),
-            ('var_kwarg2', 0),
-        ])
+            ('var_kwarg2', 6),
+        ],
+    )
     self.assertEqual(
-        list(config_lib.ordered_arguments(cfg).items()), [
-            ('arg1', 4),
+        list(config_lib.ordered_arguments(cfg).items()),
+        [
+            (0, 0),
+            (1, 1),
+            ('c', -2),
+            (3, 3),
+            (4, 4),
             ('kwarg1', 'hi'),
-            ('var_kwarg1', 3),
-            ('var_kwarg2', 0),
-        ])
+            ('var_kwarg1', 5),
+            ('var_kwarg2', 6),
+        ],
+    )
 
     with self.subTest('path element and keys match up'):
       _, metadata = cfg.__flatten__()
       path_elements = cfg.__path_elements__()
+      names = []
+      for path_element in path_elements:
+        if isinstance(path_element, daglish.Attr):
+          names.append(path_element.name)
+        elif isinstance(path_element, daglish.Index):
+          names.append(path_element.index)
+        else:
+          raise ValueError(
+              'No other path element should exists, got:', path_element
+          )
       self.assertEqual(
           metadata.argument_names,
-          tuple(path_element.name for path_element in path_elements))
+          tuple(names),
+      )
 
   @parameterized.parameters([
-      # incl_var_kw, incl_defaults, incl_unset, excl_eq_to_default, expected
-      (False, False, False, False, [('arg2', 5), ('kwarg2', 99)]),
-      (False, True, False, False, [('arg2', 5), ('kwarg1', None),
-                                   ('kwarg2', 99)]),
-      (False, False, True, False, [('arg1', fdl.NO_VALUE), ('arg2', 5),
-                                   ('kwarg2', 99)]),
-      (False, True, True, False, [('arg1', fdl.NO_VALUE), ('arg2', 5),
-                                  ('kwarg1', None), ('kwarg2', 99)]),
-      (True, False, False, False, [('arg2', 5), ('kwarg2', 99), ('foo', 12)]),
-      (True, True, False, False, [('arg2', 5), ('kwarg1', None), ('kwarg2', 99),
-                                  ('foo', 12)]),
-      (True, False, True, False, [('arg1', fdl.NO_VALUE), ('arg2', 5),
-                                  ('kwarg2', 99), ('foo', 12)]),
-      (True, True, True, False, [('arg1', fdl.NO_VALUE), ('arg2', 5),
-                                 ('kwarg1', None), ('kwarg2', 99),
-                                 ('foo', 12)]),
-      (False, False, False, True, [('arg2', 5)]),
-      (True, False, False, True, [('arg2', 5), ('foo', 12)]),
+      # incl_var_kw, incl_defaults, incl_unset, incl_eq_to_default, expected
+      (False, False, False, True, [('arg2', 5), ('kwarg2', 99)]),
+      (
+          False,
+          True,
+          False,
+          True,
+          [('arg2', 5), ('kwarg1', None), ('kwarg2', 99)],
+      ),
+      (
+          False,
+          False,
+          True,
+          True,
+          [('arg1', fdl.NO_VALUE), ('arg2', 5), ('kwarg2', 99)],
+      ),
+      (
+          False,
+          True,
+          True,
+          True,
+          [
+              ('arg1', fdl.NO_VALUE),
+              ('arg2', 5),
+              ('kwarg1', None),
+              ('kwarg2', 99),
+          ],
+      ),
+      (True, False, False, True, [('arg2', 5), ('kwarg2', 99), ('foo', 12)]),
+      (
+          True,
+          True,
+          False,
+          True,
+          [('arg2', 5), ('kwarg1', None), ('kwarg2', 99), ('foo', 12)],
+      ),
+      (
+          True,
+          False,
+          True,
+          True,
+          [('arg1', fdl.NO_VALUE), ('arg2', 5), ('kwarg2', 99), ('foo', 12)],
+      ),
+      (
+          True,
+          True,
+          True,
+          True,
+          [
+              ('arg1', fdl.NO_VALUE),
+              ('arg2', 5),
+              ('kwarg1', None),
+              ('kwarg2', 99),
+              ('foo', 12),
+          ],
+      ),
+      (False, False, False, False, [('arg2', 5)]),
+      (True, False, False, False, [('arg2', 5), ('foo', 12)]),
   ])
-  def test_ordered_arguments_options(self, include_var_keyword,
-                                     include_defaults, include_unset,
-                                     exclude_equal_to_default, expected):
-
+  def test_ordered_arguments_options(
+      self,
+      include_var_keyword,
+      include_defaults,
+      include_unset,
+      include_equal_to_default,
+      expected,
+  ):
     def fn(arg1, arg2, kwarg1=None, kwarg2=99, **kwargs):
       return (arg1, arg2, kwarg1, kwarg2, kwargs)
 
     # Arguments to the function:
     #   * arg1 has no value
     #   * arg2 has an explicit value
     #   * kwarg1 has no value, but has a default value
@@ -1288,185 +1180,21 @@
     cfg = fdl.Config(fn, arg2=5, kwarg2=99, foo=12)
 
     args = fdl.ordered_arguments(
         cfg,
         include_var_keyword=include_var_keyword,
         include_defaults=include_defaults,
         include_unset=include_unset,
-        exclude_equal_to_default=exclude_equal_to_default)
+        include_equal_to_default=include_equal_to_default,
+    )
     self.assertEqual(list(args.items()), expected)
 
-
-class ArgFactoryTest(absltest.TestCase):
-
-  def test_build_argfactory(self):
-    """Build an ArgFactory(...)."""
-    cfg = fdl.ArgFactory(SampleClass, arg1=5)
-    value = fdl.build(cfg)
-    self.assertIsInstance(value.factory, functools.partial)
-    self.assertIs(value.factory.func, SampleClass)
-    self.assertEqual(value.factory.keywords, dict(arg1=5))
-    self.assertEqual(value.factory.args, ())
-
-  def test_build_partial_argfactory(self):
-    """Build a Partial(..., ArgFactory(...))."""
-    cfg = fdl.Partial(basic_fn, fdl.ArgFactory(DataclassChild))
-    partial_fn = fdl.build(cfg)
-    self.assertTrue(arg_factory.is_arg_factory_partial(partial_fn))
-    self.assertPartialsEqual(partial_fn,
-                             arg_factory.partial(basic_fn, arg1=DataclassChild))
-
-    # Run the partial twice, and check for shared values.
-    v1 = partial_fn(arg2=3)
-    v2 = partial_fn(arg2=3)
-    self.assertEqual(v1, v2)
+  def test_include_positional(self):
+    cfg = fdl.Config(fn_with_position_args, 0, 1, 2, 3, 4, 5, kwarg='hi')
     self.assertEqual(
-        v1, dict(arg1=DataclassChild(), arg2=3, kwarg1=None, kwarg2=None))
-    self.assertIsNot(v1['arg1'], v2['arg1'])
-
-  def test_build_partial_argfactory_argfactory(self):
-    """Build a Partial(..., ArgFactory(..., ArgFactory(...)))."""
-    cfg = fdl.Partial(basic_fn,
-                      fdl.ArgFactory(basic_fn, fdl.ArgFactory(DataclassChild)))
-    cfg.arg1.arg2 = 2
-    cfg.arg2 = 3
-    partial_fn = fdl.build(cfg)
-    self.assertTrue(arg_factory.is_arg_factory_partial(partial_fn))
-    self.assertPartialsEqual(
-        partial_fn,
-        functools.partial(
-            arg_factory.partial(
-                basic_fn,
-                arg1=functools.partial(
-                    arg_factory.partial(basic_fn, arg1=DataclassChild),
-                    arg2=2)),
-            arg2=3))
-
-    # Run the partial twice, and check for shared values.
-    v1 = partial_fn()
-    v2 = partial_fn()
-    self.assertEqual(v1, v2)
-    self.assertEqual(
-        v1,
-        dict(
-            arg1=dict(arg1=DataclassChild(), arg2=2, kwarg1=None, kwarg2=None),
-            arg2=3,
-            kwarg1=None,
-            kwarg2=None))
-    self.assertIsInstance(v1['arg1'], dict)
-    self.assertIsInstance(v1['arg1']['arg1'], DataclassChild)
-
-    # Neither the dict nor the DataclassChild is shared.
-    self.assertIsNot(v1['arg1'], v2['arg1'])
-    self.assertIsNot(v1['arg1']['arg1'], v2['arg1']['arg1'])
-
-  def test_build_partial_argfactory_config(self):
-    """Build a Partial(..., ArgFactory(..., Config(...)))."""
-    cfg = fdl.Partial(basic_fn,
-                      fdl.ArgFactory(basic_fn, fdl.Config(DataclassChild)))
-    cfg.arg1.arg2 = 2
-    cfg.arg2 = 3
-    partial_fn = fdl.build(cfg)
-    self.assertTrue(arg_factory.is_arg_factory_partial(partial_fn))
-    self.assertPartialsEqual(
-        partial_fn,
-        functools.partial(
-            arg_factory.partial(
-                basic_fn,
-                arg1=functools.partial(basic_fn, arg1=DataclassChild(),
-                                       arg2=2)),
-            arg2=3))
-
-    # Run the partial twice, and check for shared values.
-    v1 = partial_fn()
-    v2 = partial_fn()
-    self.assertEqual(v1, v2)
-    self.assertEqual(
-        v1,
-        dict(
-            arg1=dict(arg1=DataclassChild(), arg2=2, kwarg1=None, kwarg2=None),
-            arg2=3,
-            kwarg1=None,
-            kwarg2=None))
-    self.assertIsInstance(v1['arg1'], dict)
-    self.assertIsInstance(v1['arg1']['arg1'], DataclassChild)
-
-    # The dict is not shared, but the DataclassChild *is* shared.
-    self.assertIsNot(v1['arg1'], v2['arg1'])
-    self.assertIs(v1['arg1']['arg1'], v2['arg1']['arg1'])
-
-  def test_build_partial_tree_argfactory(self):
-    """Build a Partial(..., Tree(..., ArgFactory(...)))."""
-    cfg = fdl.Partial(basic_fn, {
-        'x': [[fdl.Config(object)],
-              fdl.ArgFactory(DataclassChild)],
-        'y': [1, 2, 3]
-    })
-    partial_fn = fdl.build(cfg)
-    self.assertTrue(arg_factory.is_arg_factory_partial(partial_fn))
-
-    # Run the partial twice, and check for shared values.
-    v1 = partial_fn(arg2=3)
-    v2 = partial_fn(arg2=3)
-    self.assertEqual(v1, v2)
-    obj = v1['arg1']['x'][0][0]  # created from fdl.Config(object)
-    self.assertEqual(
-        v1,
-        dict(
-            arg1={
-                'x': [[obj], DataclassChild()],
-                'y': [1, 2, 3]
-            },
-            arg2=3,
-            kwarg1=None,
-            kwarg2=None))
-    # The DataclassChild and its ancestors are not shared:
-    self.assertIsNot(v1['arg1'], v2['arg1'])
-    self.assertIsNot(v1['arg1']['x'], v2['arg1']['x'])
-    self.assertIsNot(v1['arg1']['x'][1], v2['arg1']['x'][1])
-    # But other parts of the tree (including the object created
-    # by fdl.Config) are shared:
-    self.assertIs(v1['arg1']['x'][0], v2['arg1']['x'][0])
-    self.assertIs(v1['arg1']['x'][0][0], obj)
-    self.assertIs(v2['arg1']['x'][0][0], obj)
-    self.assertIs(v1['arg1']['y'], v2['arg1']['y'])
-
-  def test_build_varargs(self):
-    config = fdl.Partial(fn_with_var_args)
-    list_factory = fdl.build(fdl.ArgFactory(list))
-
-    # Call __build__ with positional args.  (Note: fdl.build only calls
-    # __build__ with keyword args; so we need to use __call__ directly to
-    # test this.)
-    partial_fn = config.__build__(list_factory, 2, [], list_factory, 5)
-
-    # Since we called __build__ with positional arguments that alternate back
-    # and forth between values and factories, it will need to
-    # construct a nested partial object with the following structure.  (Note:
-    # functools.partial automatically merges when its `func` is a partial, so
-    # this ends up being 2 partial objects, not 4.)
-    expected = functools.partial(
-        arg_factory.partial(
-            functools.partial(
-                arg_factory.partial(fn_with_var_args, list), 2, []), list), 5)
-    self.assertPartialsEqual(expected, partial_fn)
-
-    v1 = partial_fn()
-    v2 = partial_fn()
-    self.assertEqual(v1, {'arg1': [], 'args': (2, [], [], 5), 'kwarg1': None})
-    self.assertEqual(v2, {'arg1': [], 'args': (2, [], [], 5), 'kwarg1': None})
-    self.assertIsNot(v1['arg1'], v2['arg1'])  # from list_factory
-    self.assertIs(v1['args'][1], v2['args'][1])  # literal list
-    self.assertIsNot(v1['args'][2], v2['args'][2])  # from list_factory
-
-    v3 = partial_fn(10, kwarg1=20)
-    self.assertEqual(v3, {'arg1': [], 'args': (2, [], [], 5, 10), 'kwarg1': 20})
-
-  def assertPartialsEqual(self, x, y):
-    # Compare using reprs, since `==` will consider different instances of
-    # functools.partial to be different even if they have the same function
-    # and args.
-    self.assertEqual(repr(x), repr(y))
+        config_lib.ordered_arguments(cfg, include_positional=False),
+        {'c': 2, 'kwarg': 'hi'},
+    )
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.9/fiddle/_src/daglish.py` & `fiddle-0.3.0/fiddle/_src/daglish.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,19 @@
   def __lt__(self, other: PathElement) -> bool:
     if type(self) is type(other):
       return self.name < other.name
     else:
       return super().__lt__(other)
 
 
+def attr_or_index(key: Union[str, int]) -> PathElement:
+  """Returns an Attr for a string key or an Index for an int key."""
+  return Index(key) if isinstance(key, int) else Attr(key)
+
+
 class BuildableAttr(Attr):
   """An attribute of a Buildable."""
 
 
 @dataclasses.dataclass(frozen=True)
 class BuildableFnOrCls(Attr):
   """The callable (__fn_or_cls__) for a fdl.Buildable."""
@@ -139,26 +144,29 @@
 class NamedTupleType:
   pass
 
 
 # This has the same type as Path, but different semantic meaning.
 PathElements = Tuple[PathElement, ...]
 PathElementsFn = Callable[[Any], PathElements]
+_ValueAndPath = Tuple[Any, PathElement]
+OptimizedFlattenFn = Callable[[Any], Iterable[_ValueAndPath]]
 FlattenFn = Callable[[Any], Tuple[Tuple[Any, ...], Any]]
 UnflattenFn = Callable[[Iterable[Any], Any], Any]
 
 T = TypeVar("T")
 
 
 @dataclasses.dataclass(frozen=True)
 class NodeTraverser:
   """Contains information required to traverse a given node type."""
   flatten: FlattenFn
   unflatten: UnflattenFn
   path_elements: PathElementsFn
+  flatten_with_paths: OptimizedFlattenFn | None = None
 
 
 class NodeTraverserRegistry:
   """A registry of `NodeTraverser`s."""
 
   def __init__(self, *, use_fallback: Union["NodeTraverserRegistry", bool]):
     """Initializes the instance.
@@ -181,14 +189,15 @@
 
   def register_node_traverser(
       self,
       node_type: Type[Any],
       flatten_fn: FlattenFn,
       unflatten_fn: UnflattenFn,
       path_elements_fn: PathElementsFn,
+      flatten_with_paths_fn: OptimizedFlattenFn | None = None,
   ) -> None:
     """Registers a node traverser for `node_type`.
 
     Args:
       node_type: The node type to regiser a traverser for. The traverser will be
         used *only* for nodes of this type, not subclasses (with the exception
         of the special-cased `daglish.NamedTupleType`).
@@ -198,24 +207,28 @@
         arbitrary traverser-specific data.
       unflatten_fn: A function that unflattens values, which should accept
         `values` and `metadata` and return a new instance of `node_type`.
       path_elements_fn: A function that returns `PathElement` instances for the
         flattened values returned by `flatten_fn`. This should accept an
         instance of `node_type`, and return a sequence of `PathElement`s aligned
         with the values returned by `flatten_fn`.
+      flatten_with_paths_fn: A version of `flatten_fn` that returns an iterable
+        of `(value, path)` pairs, where `value` is a child value and `path` is a
+        `Path` to the value.
     """
     if not isinstance(node_type, type):
       raise TypeError(f"`node_type` ({node_type}) must be a type.")
     if node_type in self._node_traversers:
       raise ValueError(
           f"A node traverser for {node_type} has already been registered.")
     self._node_traversers[node_type] = NodeTraverser(
         flatten=flatten_fn,
         unflatten=unflatten_fn,
         path_elements=path_elements_fn,
+        flatten_with_paths=flatten_with_paths_fn,
     )
 
   def find_node_traverser(
       self,
       node_type: Type[Any],
   ) -> Optional[NodeTraverser]:
     """Finds a `NodeTraverser` for the given `node_type`.
@@ -278,27 +291,31 @@
     unflatten_fn=unflatten_defaultdict,
     path_elements_fn=lambda x: tuple(Key(key) for key in x.keys()))
 
 register_node_traverser(
     tuple,
     flatten_fn=lambda x: (x, None),
     unflatten_fn=lambda x, _: tuple(x),
-    path_elements_fn=lambda x: tuple(Index(i) for i in range(len(x))))
+    path_elements_fn=lambda x: tuple(Index(i) for i in range(len(x))),
+    flatten_with_paths_fn=lambda xs: ((x, Index(i)) for i, x in enumerate(xs)),
+)
 
 register_node_traverser(
     NamedTupleType,
     flatten_fn=lambda x: (tuple(x), type(x)),
     unflatten_fn=lambda values, node_type: node_type(*values),
     path_elements_fn=lambda x: tuple(Attr(name) for name in x._asdict().keys()))
 
 register_node_traverser(
     list,
     flatten_fn=lambda x: (tuple(x), None),
     unflatten_fn=lambda x, _: list(x),
-    path_elements_fn=lambda x: tuple(Index(i) for i in range(len(x))))
+    path_elements_fn=lambda x: tuple(Index(i) for i in range(len(x))),
+    flatten_with_paths_fn=lambda xs: ((x, Index(i)) for i, x in enumerate(xs)),
+)
 
 
 def is_prefix(prefix_path: Path, containing_path: Path):
   """Returns `True` if `prefix_path` is a prefix of `containing_path`.
 
   Args:
     prefix_path: the `Path` that may be a prefix of `containing_path`.
@@ -434,15 +451,15 @@
 
   def initial_state(self) -> State:
     """Returns an initial state for this traversal.
 
     The initial state has a reference to the traversal, the empty path, and no
     parent states.
     """
-    return State(self, (), self.root_obj, _parent=None)  # pytype: disable=attribute-error
+    return State(self, (), self.root_obj, parent=None)
 
   @classmethod
   def begin(cls, fn: Callable[..., Any], root_obj: Any) -> State:
     """Creates a new traversal and returns the initial state.
 
     Args:
       fn: Function which is applied at each node during the traversal.
@@ -480,40 +497,52 @@
   """Contains a current traversal state.
 
   Attributes:
     traversal: Reference to main traversal object.
     current_path: A path that can be followed to the current object. In the case
       of shared objects, there will be other paths to the current object, and
       often these are determined by a somewhat arbitrary DAG traversal order.
+    parent: The parent state.
   """
-  __slots__ = ("traversal", "current_path", "_value", "_parent")
+  __slots__ = ("traversal", "current_path", "_value", "parent")
 
   traversal: Traversal
   current_path: Path
 
   # Implementation note: Please don't use _value outside of the @property
   # accessors.
   _value: Any  # pylint: disable=invalid-name
 
-  _parent: Optional[State]
+  parent: Optional[State]
 
   @property
   def _object_id(self) -> int:
     return id(self._value)
 
   @property
   def _is_memoizable(self) -> bool:
     return is_memoizable(self._value)
 
   @property
+  def original_value(self):
+    """Original value constructed with this state.
+
+    Generally please don't use this value, it's much more clear to use the
+    first argument of your `traverse(value, state)` function, especially since
+    for post-order traversals, you'll often write `value =
+    state.map_children(value)`.
+    """
+    return self._value
+
+  @property
   def ancestors_inclusive(self) -> Iterable[State]:
     """Gets ancestors, including the current state."""
     yield self
-    if self._parent is not None:
-      yield from self._parent.ancestors_inclusive
+    if self.parent is not None:
+      yield from self.parent.ancestors_inclusive
 
   def get_all_paths(self, allow_caching: bool = True) -> List[Path]:
     """Gets all paths to the current value.
 
     Args:
       allow_caching: Whether paths can be cached. Most traverers will compute
         paths to all objects from the root config object. But this can fail to
@@ -591,17 +620,65 @@
 
     Raises:
       ValueError: If `value` is not traversable. Please test beforehand by
       calling `state.is_traversable()`.
     """
     node_traverser = self.traversal.find_node_traverser(type(value))
     if node_traverser is None:
-      raise ValueError("Please handle non-traversable values yourself.")
+      raise ValueError(
+          f"No node traverser found for {value}, please register traverser"
+          " or pre-process the non-traversable values first."
+      )
     return self._flattened_map_children(value, node_traverser)
 
+  def yield_map_child_values(
+      self, value: Any, ignore_leaves: bool = False
+  ) -> Iterable[Any]:
+    """Maps over children for traversable values, but doesn't unflatten results.
+
+    This method only returns result values, so use it in place of
+    `state.flattened_map_children(value).values` when the result is consumed
+    once. If you are calling this for an "effectful" computation (including ones
+    that just gather results in `nonlocal` variables) then consider the
+    following pattern,
+
+    for _ in state.yield_map_child_values(node, ignore_leaves=True):
+      pass  # Run lazy iterator.
+
+    Args:
+      value: Value to map over.
+      ignore_leaves: If True, then this function will return an empty iterable
+        if `value` is not traversable. Otherwise, it will raise a ValueError.
+
+    Yields:
+      Sub-traversal results, the same type as returned by your _traverse
+      function.
+
+    Raises:
+      ValueError: If `value` is not traversable and `ignore_leaves` is `False`.
+      Please test beforehand by calling `state.is_traversable()`.
+    """
+    node_traverser = self.traversal.find_node_traverser(type(value))
+    if node_traverser is None:
+      if ignore_leaves:
+        return
+      else:
+        raise ValueError(
+            f"No node traverser found for {value}, please register traverser"
+            " or pre-process the non-traversable values first."
+        )
+    if node_traverser.flatten_with_paths is not None:
+      for value, path in node_traverser.flatten_with_paths(value):
+        yield self.call(value, path)
+    else:
+      sub_values, unused_meta = node_traverser.flatten(value)
+      path_elements = node_traverser.path_elements(value)
+      for sub_value, path_element in zip(sub_values, path_elements):
+        yield self.call(sub_value, path_element)
+
   def call(self, value, *additional_path: PathElement):
     """Low-level function to execute a sub-traversal.
 
     This creates a new state, and then applies the function bound to the
     traverser.
 
     Args:
@@ -739,16 +816,16 @@
         "are sure this is what you need, contact the Fiddle team, and we can "
         "look into enabling this flag.")
   paths_by_id = {}
 
   def traverse(value, state: State):
     if not memoizable_only or is_memoizable(value):
       paths_by_id.setdefault(id(value), []).append(state.current_path)
-    if state.is_traversable(value):
-      state.flattened_map_children(value)
+    for _ in state.yield_map_child_values(value, ignore_leaves=True):
+      pass  # Run lazy iterator.
 
   traversal = BasicTraversal(traverse, structure, registry=registry)
   traverse(structure, traversal.initial_state())
   return paths_by_id
 
 
 def iterate(
@@ -778,17 +855,16 @@
 
   Returns:
     Iterable of (value, path) tuples.
   """
 
   def _traverse(node, state: State):
     yield node, state.current_path
-    if state.is_traversable(node):
-      for sub_result in state.flattened_map_children(node).values:
-        yield from sub_result
+    for sub_result in state.yield_map_child_values(node, ignore_leaves=True):
+      yield from sub_result
 
   if memoized:
     traversal = MemoizedTraversal(
         _traverse,
         value,
         registry=registry,
         memoize_internables=memoize_internables,
```

### Comparing `fiddle-0.2.9/fiddle/_src/daglish_extensions.py` & `fiddle-0.3.0/fiddle/_src/daglish_extensions.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/daglish_extensions_test.py` & `fiddle-0.3.0/fiddle/_src/daglish_extensions_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/daglish_test.py` & `fiddle-0.3.0/fiddle/_src/daglish_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """Tests for daglish."""
 
 import collections
 import dataclasses
 import enum
 import json
 import random
-from typing import Any, List, NamedTuple, Optional, cast
+from typing import Any, List, NamedTuple, Optional, Tuple, cast
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import daglish
 from fiddle import history
 from fiddle._src.experimental import dataclasses as fdl_dc
@@ -52,28 +52,44 @@
   """`fdl.Tag` to use for testing."""
 
 
 def sample_fn(arg, kwarg="test"):
   return arg, kwarg
 
 
+def fn_with_position_args(  # pylint: disable=keyword-arg-before-vararg
+    a, b, /, c=1, *args, kwarg1=None, karg2=None, **kwargs
+):  # pylint: disable=unused-argument
+  return locals()
+
+
 @dataclasses.dataclass
 class TraversalLoggingMapFunction:
   call_args: List[Any] = dataclasses.field(default_factory=list)
   some_path_args: List[Any] = dataclasses.field(default_factory=list)
   all_path_args: List[Any] = dataclasses.field(default_factory=list)
 
   def __call__(self, value, state: Optional[daglish.State] = None):
     state = state or daglish.MemoizedTraversal.begin(self, value)
     self.call_args.append(value)
     self.some_path_args.append(state.current_path)
     self.all_path_args.append(state.get_all_paths())
     return state.map_children(value)
 
 
+@dataclasses.dataclass
+class NonRecursingLoggingFunction:
+  values_and_paths: List[Tuple[Any, Any]] = dataclasses.field(
+      default_factory=list
+  )
+
+  def __call__(self, value, state: daglish.State):
+    self.values_and_paths.append((value, state.current_path))
+
+
 def switch_buildables_to_args(value, state: Optional[daglish.State] = None):
   """Replaces buildables with their arguments dictionary.
 
   Args:
     value: Nested configuration structure.
     state: Traversal state.
 
@@ -87,14 +103,36 @@
     return fdl.ordered_arguments(value)
   elif isinstance(value, enum.Enum):
     return str(value)
   else:
     return value
 
 
+@dataclasses.dataclass
+class MyRange:
+  start: int
+  end: int
+
+
+def myrange_flatten_with_paths_fn(myrange: MyRange):
+  return (
+      ({"value": i}, daglish.Index(i))
+      for i in range(myrange.start, myrange.end)
+  )
+
+
+daglish.register_node_traverser(
+    MyRange,
+    flatten_fn=NotImplemented,  # pytype: disable=wrong-arg-types
+    unflatten_fn=NotImplemented,  # pytype: disable=wrong-arg-types
+    path_elements_fn=NotImplemented,  # pytype: disable=wrong-arg-types
+    flatten_with_paths_fn=myrange_flatten_with_paths_fn,
+)
+
+
 class PathTest(parameterized.TestCase):
 
   @parameterized.named_parameters(
       dict(
           testcase_name="exact_match",
           prefix_path=".foo.bar",
           containing_path=".foo.bar",
@@ -208,14 +246,28 @@
     self.assertLess(b, c)
 
 
 class TraverserRegistryTest(parameterized.TestCase):
 
   @parameterized.named_parameters([
       ("config", fdl.Config(Foo, bar=1, baz=2)),
+      (
+          "positional_config",
+          fdl.Config(
+              fn_with_position_args,
+              0,
+              1,
+              2,
+              3,
+              4,
+              kwarg1=5,
+              var_kwarg1=6,
+              var_kwarg2=7,
+          ),
+      ),
       ("tagged_value", SampleTag.new()),
       ("namedtuple", SampleNamedTuple("a", "b")),
       ("list", [1, 2, 3]),
       ("tuple", (1, 2, 3)),
       ("dict", dict(a=1, b=2)),
       ("defaultdict", collections.defaultdict(list, a=[1], b=[2])),
   ])
@@ -413,14 +465,81 @@
         cfg.__argument_history__["bar"][-1].location.line_number)
     self.assertEqual(copied.__argument_history__["bar"][0].new_value, 4)
     self.assertEqual(copied.__argument_history__["bar"][1].new_value, 5)
     self.assertEqual(copied.__argument_history__["bar"][-1].kind,
                      history.ChangeKind.NEW_VALUE)
 
 
+_eager_map_fns = [
+    lambda state, obj: state.map_children(obj),
+    lambda state, obj: list(state.yield_map_child_values(obj)),
+    lambda state, obj: state.flattened_map_children(obj),
+]
+
+
+class StateApiTest(parameterized.TestCase):
+
+  @parameterized.parameters(_eager_map_fns)
+  def test_map_dict(self, map_fn):
+    obj = {"a": 1, "b": 2}
+    log_calls = NonRecursingLoggingFunction()
+    traversal = daglish.BasicTraversal(log_calls, obj)
+    state = traversal.initial_state()
+    map_fn(state, obj)
+    self.assertEqual(
+        log_calls.values_and_paths,
+        [(1, (daglish.Key(key="a"),)), (2, (daglish.Key(key="b"),))],
+    )
+
+  @parameterized.parameters(_eager_map_fns)
+  def test_map_tuple(self, map_fn):
+    obj = ((), (1, 2), 3)
+    log_calls = NonRecursingLoggingFunction()
+    traversal = daglish.BasicTraversal(log_calls, obj)
+    state = traversal.initial_state()
+    map_fn(state, obj)
+    self.assertEqual(
+        log_calls.values_and_paths,
+        [
+            ((), (daglish.Index(index=0),)),
+            ((1, 2), (daglish.Index(index=1),)),
+            (3, (daglish.Index(index=2),)),
+        ],
+    )
+
+  @parameterized.parameters(_eager_map_fns)
+  def test_map_memoized(self, map_fn):
+    shared = {"foo": 123}
+    obj = [shared, shared, shared]
+    log_calls = NonRecursingLoggingFunction()
+    traversal = daglish.MemoizedTraversal(log_calls, obj)
+    state = traversal.initial_state()
+    map_fn(state, obj)
+    self.assertEqual(
+        log_calls.values_and_paths, [({"foo": 123}, (daglish.Index(index=0),))]
+    )
+
+  def test_fast_map_calls_flatten_with_paths(self):
+    obj = MyRange(3, 7)
+    log_calls = NonRecursingLoggingFunction()
+    traversal = daglish.MemoizedTraversal(log_calls, obj)
+    state = traversal.initial_state()
+    for _ in state.yield_map_child_values(obj):
+      pass  # Run lazy iterator.
+    self.assertEqual(
+        log_calls.values_and_paths,
+        [
+            ({"value": 3}, (daglish.Index(index=3),)),
+            ({"value": 4}, (daglish.Index(index=4),)),
+            ({"value": 5}, (daglish.Index(index=5),)),
+            ({"value": 6}, (daglish.Index(index=6),)),
+        ],
+    )
+
+
 class ArgsSwitchingFuzzTest(parameterized.TestCase):
 
   def test_fuzz(self):
     # Note: We could use `parameterized.test_cases`, but subTest shows up more
     # compactly in test output.
     for rng_seed in range(100):
       with self.subTest(f"rng_seed={rng_seed}"):
@@ -486,14 +605,41 @@
             (config["dataclass"], "['dataclass']"),
             (3, "['dataclass'].bar"),
             (fdl.Config(sample_fn, "arg"), "['dataclass'].baz"),
             ("arg", "['dataclass'].baz.arg"),
         ],
     )
 
+  def test_walk_positional_arguments(self):
+    config = fdl.Config(
+        fn_with_position_args,
+        0,
+        1,
+        2,
+        3,
+        4,
+        kwarg1=5,
+        var_kwarg1=6,
+        var_kwarg2=7,
+    )
+    self.assertEqual(
+        _iterate_path_strings(config),
+        [
+            (config, ""),
+            (config[0], "[0]"),
+            (config[1], "[1]"),
+            (config.c, ".c"),
+            (config[3], "[3]"),
+            (config[4], "[4]"),
+            (config.kwarg1, ".kwarg1"),
+            (config.var_kwarg1, ".var_kwarg1"),
+            (config.var_kwarg2, ".var_kwarg2"),
+        ],
+    )
+
 
 class MemoizedTraversalTest(absltest.TestCase):
 
   def test_unique_traversals_for_different_ids(self):
     # This test generates a bunch of new objects during traversal, which if
     # cached incorrectly will result in false positive cache hits. (This is
     # because the Python interpreter will garbage collect and reuse the
@@ -525,15 +671,15 @@
         "Fiddle detected a cycle while traversing a value: "
         r"<root>\[3\] is <root>\[3\]\[3\]\.",
     ):
       daglish.MemoizedTraversal.run(traverse, x)
 
   def test_cycle_detection_in_fdl_build(self):
     cfg = fdl.Config(Foo, bar=fdl.Config(Foo))
-    cfg.bar.bar = cfg
+    cfg.bar.bar = cfg  # pytype: disable=not-writable  # use-fiddle-overlay
     with self.assertRaisesRegex(
         ValueError,
         "Fiddle detected a cycle while traversing a value: "
         r"<root>\.bar is <root>\.bar\.bar\.bar\.",
     ):
       fdl.build(cfg)
 
@@ -544,15 +690,15 @@
     def traverse(value, state: daglish.State):
       if state.is_traversable(value):
         return {
             "paths": ", ".join(
                 daglish.path_str(path)
                 for path in state.get_all_paths(allow_caching=True)
             ),
-            "sub_values": state.flattened_map_children(value).values,
+            "sub_values": list(state.yield_map_child_values(value)),
         }
       else:
         return "leaf value"
 
     traverser = daglish.MemoizedTraversal(
         traverse, config, fdl_dc.daglish_dataclass_registry
     )
```

### Comparing `fiddle-0.2.9/fiddle/_src/diffing.py` & `fiddle-0.3.0/fiddle/_src/diffing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # limitations under the License.
 
 """Library for finding differences between Fiddle configurations."""
 
 import abc
 import copy
 import dataclasses
-from typing import Any, Callable, Dict, Iterable, List, Sequence, Tuple, Union, Mapping
+from typing import Any, Callable, Dict, Iterable, List, Mapping, Sequence, Tuple, Union
 
 from fiddle._src import config as config_lib
 from fiddle._src import daglish
+from fiddle._src import mutate_buildable
 from fiddle._src import tag_type
+from fiddle._src import tagging
 from fiddle._src.experimental import daglish_legacy
 
 
 class AlignmentError(ValueError):
   """Indicates that two values cannot be aligned."""
 
 
@@ -142,15 +144,15 @@
   """
   target: daglish.Path
   new_value: Union[Reference, Any]
 
   def apply(self, parent: Any, child: daglish.PathElement):
     """Replaces `child.follow(parent)` with self.new_value."""
     if isinstance(child, daglish.BuildableFnOrCls):
-      config_lib.update_callable(parent, self.new_value)
+      mutate_buildable.update_callable(parent, self.new_value)
     elif isinstance(child, daglish.Attr):
       setattr(parent, child.name, self.new_value)
     elif isinstance(child, daglish.Index):
       parent[child.index] = self.new_value
     elif isinstance(child, daglish.Key):
       parent[child.key] = self.new_value
     else:
@@ -182,15 +184,15 @@
   The target's parent must be a `fdl.Buildable`.
   """
   target: daglish.Path
   tag: tag_type.TagType
 
   def apply(self, parent: Any, child: daglish.PathElement):
     if isinstance(child, daglish.Attr):
-      config_lib.add_tag(parent, child.name, self.tag)
+      tagging.add_tag(parent, child.name, self.tag)
     else:
       raise ValueError(f'DeleteValue does not support {child}.')
 
 
 @dataclasses.dataclass(frozen=True)
 class RemoveTag(DiffOperation):
   """Removes a tag from a Buildable argument.
@@ -198,15 +200,15 @@
   The target's parent must be a `fdl.Buildable`.
   """
   target: daglish.Path
   tag: tag_type.TagType
 
   def apply(self, parent: Any, child: daglish.PathElement):
     if isinstance(child, daglish.Attr):
-      config_lib.remove_tag(parent, child.name, self.tag)
+      tagging.remove_tag(parent, child.name, self.tag)
     else:
       raise ValueError(f'DeleteValue does not support {child}.')
 
 
 @dataclasses.dataclass(frozen=True)
 class AlignedValues:
   """A pair of aligned values."""
@@ -477,17 +479,19 @@
   alignment = DiffAlignment(old, new, old_name, new_name)
   alignment.align(old, new)
 
   # First pass: align by id.
   old_by_id = daglish_legacy.collect_value_by_id(old, memoizable_only=True)
   new_by_id = daglish_legacy.collect_value_by_id(new, memoizable_only=True)
   for (value_id, value) in old_by_id.items():
-    if value_id in new_by_id:
-      if alignment.can_align(value, value):
-        alignment.align(value, value)
+    # Do not align by id for small container objects.
+    if not _is_small_container(value):
+      if value_id in new_by_id:
+        if alignment.can_align(value, value):
+          alignment.align(value, value)
 
   # Second pass: align any objects that are reachable by the same path.
   path_to_old = daglish_legacy.collect_value_by_path(old, memoizable_only=True)
   path_to_new = daglish_legacy.collect_value_by_path(new, memoizable_only=True)
   for (path, old_value) in path_to_old.items():
     if path in path_to_new:
       if alignment.can_align(old_value, path_to_new[path]):
@@ -500,14 +504,21 @@
         if _should_align_by_equality(old_value):
           if alignment.can_align(old_value, new_value):
             alignment.align(old_value, new_value)
 
   return alignment
 
 
+def _is_small_container(value):
+  """Returns if value is a small Sequence or Mapping."""
+  if isinstance(value, (Sequence, Mapping)) and len(repr(value)) < 80:
+    return True
+  return False
+
+
 def _should_align_by_equality(value):
   """Returns true if two equal copies of `value` should be aligned.
 
   Generally, we should avoid aligning "small" values by equality, since
   they might be unrelated, and just happen to be equal.  This function
   uses several heuristics to decide whether the value should be aligned.
 
@@ -994,17 +1005,19 @@
     skip_leaf = (
         isinstance(change, SetValue) or
         isinstance(change.target[-1], daglish.BuildableFnOrCls))
     root = _add_path_to_skeleton(root, change.target, skip_leaf)
     if isinstance(change, (ModifyValue, SetValue)):
       daglish_legacy.traverse_with_path(add_reference_target, change.new_value)
     if isinstance(change, RemoveTag):
-      config_lib.add_tag(
-          daglish.follow_path(root, change.target[:-1]), change.target[-1].name,
-          change.tag)
+      tagging.add_tag(
+          daglish.follow_path(root, change.target[:-1]),
+          change.target[-1].name,
+          change.tag,
+      )
   daglish_legacy.traverse_with_path(add_reference_target,
                                     diff.new_shared_values)
 
   return root
 
 
 def _add_path_to_skeleton(skeleton, path, skip_leaf=False):
```

### Comparing `fiddle-0.2.9/fiddle/_src/diffing_test.py` & `fiddle-0.3.0/fiddle/_src/diffing_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -458,25 +458,25 @@
     expected_changes = (diffing.ModifyValue(parse_path('.x'), 11),
                         diffing.ModifyValue(parse_path('.y.x'), 22))
     self.check_diff(old, new, expected_changes)
 
   def test_modify_sequence_element(self):
     old = fdl.Config(SimpleClass, [1, 2, [3]])
     new = copy.deepcopy(old)
-    new.x[0] = 11
-    new.x[2][0] = 33
+    new.x[0] = 11  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    new.x[2][0] = 33  # pytype: disable=unsupported-operands  # use-fiddle-overlay
     expected_changes = (diffing.ModifyValue(parse_path('.x[0]'), 11),
                         diffing.ModifyValue(parse_path('.x[2][0]'), 33))
     self.check_diff(old, new, expected_changes)
 
   def test_modify_dict_item(self):
     old = fdl.Config(SimpleClass, {'a': 2, 'b': 4, 'c': {'d': 7}})
     new = copy.deepcopy(old)
-    new.x['a'] = 11
-    new.x['c']['d'] = 33
+    new.x['a'] = 11  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    new.x['c']['d'] = 33  # pytype: disable=unsupported-operands  # use-fiddle-overlay
     expected_changes = (diffing.ModifyValue(parse_path(".x['a']"), 11),
                         diffing.ModifyValue(parse_path(".x['c']['d']"), 33))
     self.check_diff(old, new, expected_changes)
 
   def test_set_buildable_argument(self):
     old = fdl.Config(SimpleClass, 1, fdl.Config(AnotherClass, 2, 3))
     new = copy.deepcopy(old)
@@ -485,16 +485,16 @@
     expected_changes = (diffing.SetValue(parse_path('.z'), 11),
                         diffing.SetValue(parse_path('.y.a'), 22))
     self.check_diff(old, new, expected_changes)
 
   def test_set_dict_item(self):
     old = fdl.Config(SimpleClass, {'a': 2, 'b': 4, 'c': {'d': 7}})
     new = copy.deepcopy(old)
-    new.x['foo'] = 11
-    new.x['c']['bar'] = 33
+    new.x['foo'] = 11  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    new.x['c']['bar'] = 33  # pytype: disable=unsupported-operands  # use-fiddle-overlay
     expected_changes = (diffing.SetValue(parse_path(".x['foo']"), 11),
                         diffing.SetValue(parse_path(".x['c']['bar']"), 33))
     self.check_diff(old, new, expected_changes)
 
   def test_delete_buildable_argument(self):
     old = fdl.Config(SimpleClass, 1, fdl.Config(AnotherClass, 2, 3),
                      fdl.Config(SimpleClass, 4))
@@ -506,17 +506,17 @@
                         diffing.DeleteValue(parse_path('.y.x')),
                         diffing.DeleteValue(parse_path('.z')))
     self.check_diff(old, new, expected_changes)
 
   def test_delete_dict_item(self):
     old = fdl.Config(SimpleClass, {'a': 2, 'b': {}, 'c': {'d': 7}})
     new = copy.deepcopy(old)
-    del new.x['a']
-    del new.x['b']
-    del new.x['c']['d']
+    del new.x['a']  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    del new.x['b']  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    del new.x['c']['d']  # pytype: disable=unsupported-operands  # use-fiddle-overlay
     expected_changes = (diffing.DeleteValue(parse_path(".x['a']")),
                         diffing.DeleteValue(parse_path(".x['b']")),
                         diffing.DeleteValue(parse_path(".x['c']['d']")))
     self.check_diff(old, new, expected_changes)
 
   def test_add_shared_new_objects(self):
     old = fdl.Config(
@@ -524,15 +524,15 @@
         x=1,
         y=fdl.Config(SimpleClass, x=2, y=3, z=[12]),
         z=fdl.Config(SimpleClass, x=4))
     new = copy.deepcopy(old)
     new.x = [1, 2, [3, 4], new.y.z]
     new.y.x = new.x
     new.y.y = [99]
-    new.z.y = fdl.Config(SimpleClass, new.x[2], new.y.y)
+    new.z.y = fdl.Config(SimpleClass, new.x[2], new.y.y)  # pytype: disable=not-writable  # use-fiddle-overlay
     expected_new_shared_values = (
         [3, 4],
         [
             1, 2,
             parse_reference('new_shared_values', '[0]'),
             parse_reference('old', '.y.z')
         ],
@@ -697,14 +697,21 @@
         diff_builder.aligned_or_equal(old.first.z[1], new.first.kwarg2))
 
   def test_replace_set(self):
     self.check_diff([set([5])], [set([6])],
                     expected_changes=(diffing.ModifyValue(
                         parse_path('[0]'), set([6])),))
 
+  def test_align_heuristically_identical_configs_w_different_ids(self):
+    a = {'k': [1, 2, 3], 'v': None}
+    b = {'k': [1, 2, 3], 'v': None}
+    x = fdl.Config(make_pair, a, b)
+    y = fdl.Config(make_pair, b, a)
+    self.check_diff(x, y)
+
   def test_root_must_be_aligned(self):
     old = fdl.Config(SimpleClass, 1, 2, 3)
     new = fdl.Config(SimpleClass, 4, 5, 6)
     # Manually construct an alignment with no alignments (where the root
     # `old` and `new` objects are not aligned).  Note that
     # `align_heuristically` always aligns the root objects.
     alignment = diffing.DiffAlignment(old, new)
@@ -1039,21 +1046,21 @@
       ],
       [  # Key
           diffing.Diff(changes=(diffing.DeleteValue(parse_path('["a"]')),)),
           dict(a=diffing.AnyValue())
       ],
       [  # Attr
           diffing.Diff(changes=(diffing.DeleteValue(parse_path('.x')),)),
-          fdl.Config(diffing.AnyCallable(), x=diffing.AnyValue())
+          fdl.Config(diffing.AnyCallable(), x=diffing.AnyValue())  # pytype: disable=invalid-annotation  # use-fiddle-overlay
       ],
       [  # BuildableFnOrCls
           diffing.Diff(
               changes=(diffing.ModifyValue(
                   parse_path('.__fn_or_cls__'), basic_fn),)),
-          fdl.Config(diffing.AnyCallable())
+          fdl.Config(diffing.AnyCallable())  # pytype: disable=invalid-annotation  # use-fiddle-overlay
       ],
       # Test each DiffOperation type.
       [  # DeleteValue
           diffing.Diff(changes=(diffing.DeleteValue(parse_path('["a"]')),)),
           dict(a=diffing.AnyValue())
       ],
       [  # SetValue
@@ -1074,63 +1081,63 @@
       ],
       [  # ModifyValue
           diffing.Diff(changes=(diffing.ModifyValue(parse_path('["a"]'), 1),)),
           dict(a=diffing.AnyValue())
       ],
       [  # AddTag
           diffing.Diff(changes=(diffing.AddTag(parse_path('.x'), GreenTag),)),
-          fdl.Config(diffing.AnyCallable(), x=diffing.AnyValue())
+          fdl.Config(diffing.AnyCallable(), x=diffing.AnyValue())  # pytype: disable=invalid-annotation  # use-fiddle-overlay
       ],
       [  # RemoveTag
           diffing.Diff(
               changes=(diffing.RemoveTag(parse_path('.x'), GreenTag),)),
           config_with_tags(
-              fdl.Config(diffing.AnyCallable(), x=diffing.AnyValue()),
+              fdl.Config(diffing.AnyCallable(), x=diffing.AnyValue()),  # pytype: disable=invalid-annotation  # use-fiddle-overlay
               {'x': {GreenTag}})
       ],
       # Paths with >1 PathElement
       [
           diffing.Diff(changes=(diffing.DeleteValue(parse_path('.x["a"]')),)),
-          fdl.Config(diffing.AnyCallable(), x={'a': diffing.AnyValue()})
+          fdl.Config(diffing.AnyCallable(), x={'a': diffing.AnyValue()})  # pytype: disable=invalid-annotation  # use-fiddle-overlay
       ],
       [
           diffing.Diff(changes=(diffing.DeleteValue(parse_path('.x.y')),)),
-          fdl.Config(
+          fdl.Config(  # pytype: disable=invalid-annotation  # use-fiddle-overlay
               diffing.AnyCallable(),
-              x=fdl.Config(diffing.AnyCallable(), y=diffing.AnyValue()))
+              x=fdl.Config(diffing.AnyCallable(), y=diffing.AnyValue()))  # pytype: disable=invalid-annotation  # use-fiddle-overlay
       ],
       [
           diffing.Diff(changes=(diffing.ModifyValue(parse_path('.x[2]'), 5),)),
-          fdl.Config(
+          fdl.Config(  # pytype: disable=invalid-annotation  # use-fiddle-overlay
               diffing.AnyCallable(),
               x=diffing.ListPrefix(
                   [diffing.AnyValue(),
                    diffing.AnyValue(),
                    diffing.AnyValue()]))
       ],
       [
           diffing.Diff(
               changes=(diffing.ModifyValue(
                   parse_path('.x.__fn_or_cls__'), basic_fn),)),
-          fdl.Config(
-              diffing.AnyCallable(), x=fdl.Config(diffing.AnyCallable()))
+          fdl.Config(  # pytype: disable=invalid-annotation  # use-fiddle-overlay
+              diffing.AnyCallable(), x=fdl.Config(diffing.AnyCallable()))  # pytype: disable=invalid-annotation  # use-fiddle-overlay
       ],
       # Diff with multiple paths.
       [
           diffing.Diff(
               changes=(diffing.DeleteValue(parse_path('.x.y')),
                        diffing.SetValue(parse_path('.y[1].q'), 3),
                        diffing.DeleteValue(parse_path('.z["foo"]')),
                        diffing.ModifyValue(parse_path('.y[2]'), 5))),
-          fdl.Config(
+          fdl.Config(  # pytype: disable=invalid-annotation  # use-fiddle-overlay
               diffing.AnyCallable(),
-              x=fdl.Config(diffing.AnyCallable(), y=diffing.AnyValue()),
+              x=fdl.Config(diffing.AnyCallable(), y=diffing.AnyValue()),  # pytype: disable=invalid-annotation  # use-fiddle-overlay
               y=diffing.ListPrefix([
                   diffing.AnyValue(),
-                  fdl.Config(diffing.AnyCallable()),
+                  fdl.Config(diffing.AnyCallable()),  # pytype: disable=invalid-annotation  # use-fiddle-overlay
                   diffing.AnyValue()
               ]),
               z={'foo': diffing.AnyValue()}),
       ],
   ])
   def test_skeleton_from_diff(self, cfg_diff, expected):
     actual = diffing.skeleton_from_diff(cfg_diff)
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/__init__.py` & `fiddle-0.3.0/fiddle/_src/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/auto_config.py` & `fiddle-0.3.0/fiddle/_src/experimental/auto_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,59 +26,73 @@
 import builtins
 import dataclasses
 import functools
 import inspect
 import linecache
 import textwrap
 import types
-from typing import Any, Callable, Optional, Type, cast
+from typing import Any, Callable, Optional, Type, TypeVar, cast
 
 from fiddle._src import arg_factory
 from fiddle._src import building
+from fiddle._src import casting as cast_lib
 from fiddle._src import config
+from fiddle._src import copying
 from fiddle._src import mutate_buildable
+from fiddle._src import partial
 from fiddle._src.experimental import auto_config_policy
 from fiddle._src.experimental import daglish_legacy
 import libcst as cst
 
 _CALL_HANDLER_ID = '__auto_config_call_handler__'
 _ATTR_LOAD_HANDLER_ID = '__auto_config_attr_load_handler__'
 _ATTR_SAVE_HANDLER_ID = '__auto_config_attr_save_handler__'
 _ATTR_SAVE_TEMP_VAR_ID = '_attr_save_temp'
 _CLOSURE_WRAPPER_ID = '__auto_config_closure_wrapper__'
 _EMPTY_ARGUMENTS = ast.arguments(
-    posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[])
+    posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]
+)
 _BUILTINS = frozenset([
-    builtin for builtin in builtins.__dict__.values()
+    builtin
+    for builtin in builtins.__dict__.values()
     if inspect.isroutine(builtin) or inspect.isclass(builtin)
 ])
 
 
+_GenericCallable = TypeVar('_GenericCallable', bound=Callable[..., Any])
+
+
 @dataclasses.dataclass(frozen=True)
 class AutoConfig:
   """A function wrapper for auto_config'd functions.
 
   In order to support auto_config'ing @classmethod's, we need to customize the
   descriptor protocol for the auto_config'd function. This simple wrapper type
-  is designed to look like a simple `functool.wraps` wrapper, but implements
-  custom behavior for bound methods.
+  is designed to look like a `functool.wraps` wrapper, but implements custom
+  behavior for bound methods.
   """
+
   func: Callable[..., Any]
   buildable_func: Callable[..., config.Buildable]
   always_inline: bool
 
   @property
   def nowrap(self):
     return True  # Tells Flax not to decorate this object, for classmethods.
 
   def __post_init__(self):
     # Must copy-over to correctly implement "functools.wraps"-like
     # functionality.
-    for name in ('__module__', '__name__', '__qualname__', '__doc__',
-                 '__annotations__'):
+    for name in (
+        '__module__',
+        '__name__',
+        '__qualname__',
+        '__doc__',
+        '__annotations__',
+    ):
       try:
         value = getattr(self.func, name)
       except AttributeError:
         pass
       else:
         object.__setattr__(self, name, value)
 
@@ -89,15 +103,16 @@
     return self.buildable_func(*args, **kwargs)
 
   def __get__(self, obj, objtype=None):
     # pytype: disable=attribute-error
     return AutoConfig(
         func=self.func.__get__(obj, objtype),
         buildable_func=self.buildable_func.__get__(obj, objtype),
-        always_inline=self.always_inline)
+        always_inline=self.always_inline,
+    )
     # pytype: enable=attribute-error
 
   @property
   def __wrapped__(self):
     return self.func
 
   def __getattr__(self, name):
@@ -109,19 +124,21 @@
 class UnsupportedLanguageConstructError(SyntaxError):
   pass
 
 
 class _AutoConfigNodeTransformer(ast.NodeTransformer):
   """A NodeTransformer that adds the auto-config call handler into an AST."""
 
-  def __init__(self,
-               source: str,
-               filename: str,
-               line_number: int,
-               allow_control_flow=False):
+  def __init__(
+      self,
+      source: str,
+      filename: str,
+      line_number: int,
+      allow_control_flow=False,
+  ):
     """Initializes the auto config node transformer instance.
 
     Args:
       source: The source code of the node that will be transformed by this
         instance. This is used for better error reporting.
       filename: The filename `source` is from.
       line_number: The line number of `source` within `filename`.
@@ -184,15 +201,16 @@
       return
 
     for decorator in decorator_list[:auto_config_index]:
       if decorator in ('classmethod', 'staticmethod'):
         raise AssertionError(
             f'@{decorator} placed above @auto_config on function {node.name} '
             f'at {self._filename}:{self._line_number}. Reorder decorators so '
-            f'that @auto_config is placed above @{decorator}.')
+            f'that @auto_config is placed above @{decorator}.'
+        )
 
   # pylint: disable=invalid-name
   def visit_Call(self, node: ast.Call):
     return ast.Call(
         func=ast.Name(id=_CALL_HANDLER_ID, ctx=ast.Load()),
         args=[node.func, *(self.visit(arg) for arg in node.args)],
         keywords=[self.visit(keyword) for keyword in node.keywords],
@@ -425,26 +443,28 @@
           ast.FunctionDef(
               name=_CLOSURE_WRAPPER_ID,
               args=_EMPTY_ARGUMENTS,
               body=[
                   *closure_var_definitions,
                   *module.body,
               ],
-              decorator_list=[])
+              decorator_list=[],
+          )
       ],
       type_ignores=[],
   )
   wrapper_module = ast.fix_missing_locations(wrapper_module)
   return wrapper_module
 
 
 def _find_function_code(code: types.CodeType, fn_name: str):
   """Finds the code object within `code` corresponding to `fn_name`."""
   code = [
-      const for const in code.co_consts
+      const
+      for const in code.co_consts
       if inspect.iscode(const) and const.co_name == fn_name
   ]
   assert len(code) == 1, f"Couldn't find function code for {fn_name!r}."
   return code[0]
 
 
 def _unwrap_code_for_fn(code: types.CodeType, fn: types.FunctionType):
@@ -489,15 +509,15 @@
 
   The Fiddle configuration for `my_fn`, on the other hand, looks like,
 
   my_fn_config = fdl.Partial(fn, foo=fdl.ArgFactory(foo_factory),
                              bar=fdl.ArgFactory(bar_factory))
 
   Therefore, we need to wrap `foo_factory` and `bar_factory` in
-  `config.ArgFactory`. Or, if they are already callable sub-configs, then we
+  `partial.ArgFactory`. Or, if they are already callable sub-configs, then we
   wrap them in ArgFactory.
 
   If `foo_factory` or `bar_factory` is not a callable or fdl.Partial, then we
   raise an error. It's techincally possible to pass `foo_factory` as a
   fdl.Config object that, when called, returns another fucntion, but this is
   most likely a mistake in configuration, so we don't allow it.
 
@@ -505,16 +525,16 @@
     arg_factory_cls: The type to use when creating the ArgFactory (normally this
       will just be `fdl.ArgFactory`, but can potentially be customized).
     arg: Intermediate value passed to `arg_factory.partial`.
 
   Returns:
     ArgFactory version of a configuration or callable.
   """
-  if isinstance(arg, config.Partial):
-    return config.cast(arg_factory_cls, arg)
+  if isinstance(arg, partial.Partial):
+    return cast_lib.cast(arg_factory_cls, arg)
   elif callable(arg):
     return arg_factory_cls(arg)
   else:
     raise ValueError(
         "Couldn't figure out how to handle arg_factory argument; please "
         f'bind any constant args with a nested functools.partial. Arg: {arg!r}'
     )
@@ -530,31 +550,31 @@
     *args: Positional arguments, only supported when `config_or_callable` is a
       Partial already.
     **kwargs: Keyword arguments.
 
   Returns:
     New callable.
   """
-  if isinstance(buildable_or_callable, config.Partial):
+  if isinstance(buildable_or_callable, partial.Partial):
     if args:
       # Note: this can cause an issue even in when not chained, if the built
       # functools.partial object is called with arguments. We may later choose
       # to raise exceptions in those cases. For this case however, it's hard to
       # define any reasonable behavior, so we always error.
       raise ValueError(
           'For chained functools.partial calls inside auto_config, e.g. '
           'functools.partial(functools.partial(foo, ...), ...), only keyword '
           f'arguments can be supplied to the outer call. Got: {args!r}'
       )
-    return config.copy_with(buildable_or_callable, **kwargs)
+    return copying.copy_with(buildable_or_callable, **kwargs)
   else:
     return partial_cls(buildable_or_callable, *args, **kwargs)
 
 
-def exempt(fn_or_cls: Callable[..., Any]) -> Callable[..., Any]:
+def exempt(fn_or_cls: _GenericCallable) -> _GenericCallable:
   """Wrap a callable so that it's exempted from auto_config.
 
   This can be used either as a decorator to exempt a function, or used inside
   an auto_config function to inline exempt certain calls to a function.
   During auto_config transformation, exempted function calls will be evaluated
   normally rather than turned into a config object. For example::
 
@@ -580,16 +600,16 @@
       func=fn_or_cls, buildable_func=fn_or_cls, always_inline=True
   )
 
 
 @dataclasses.dataclass(frozen=True)
 class ConfigTypes:
   config_cls: Type[config.Config] = config.Config
-  partial_cls: Type[config.Partial] = config.Partial
-  arg_factory_cls: Type[config.ArgFactory] = config.ArgFactory
+  partial_cls: Type[partial.Partial] = partial.Partial
+  arg_factory_cls: Type[partial.ArgFactory] = partial.ArgFactory
 
 
 def auto_config(
     fn=None,
     *,
     experimental_allow_dataclass_attribute_access=False,
     experimental_allow_control_flow: bool = False,
@@ -771,17 +791,19 @@
           f'Cannot save attribute {attr!r} on object of type {type(obj)}'
           ' within auto_config, as this could lead to inconsistent behavior'
           ' between the Python and as_buildable code paths.'
       )
 
   def make_auto_config(fn):
     if not isinstance(fn, (types.FunctionType, classmethod, staticmethod)):
-      raise ValueError('`auto_config` is only compatible with functions, '
-                       f'`@classmethod`s, and `@staticmethod`s.  Got {fn!r} '
-                       f'with type {type(fn)!r}.')
+      raise ValueError(
+          '`auto_config` is only compatible with functions, '
+          f'`@classmethod`s, and `@staticmethod`s.  Got {fn!r} '
+          f'with type {type(fn)!r}.'
+      )
 
     if isinstance(fn, (classmethod, staticmethod)):
       method_type = type(fn)
       fn = fn.__func__
     else:
       method_type = None
 
@@ -792,15 +814,16 @@
     # the source to provide more informative error messages.
     filename = inspect.getsourcefile(fn)
     line_number = fn.__code__.co_firstlineno
     node_transformer = _AutoConfigNodeTransformer(
         source=source,
         filename=filename,
         line_number=line_number,
-        allow_control_flow=experimental_allow_control_flow)
+        allow_control_flow=experimental_allow_control_flow,
+    )
 
     # Parse the AST, and modify it by intercepting all `Call`s with the
     # `auto_config_call_handler`. Finally, ensure line numbers and code
     # locations match up with the original function, to make errors
     # interpretable.
     node = ast.parse(source)
     node = node_transformer.visit(node)
@@ -875,15 +898,16 @@
     else:
       as_buildable = auto_config_fn
 
     if method_type:
       fn = method_type(fn)
       as_buildable = method_type(as_buildable)
     return AutoConfig(
-        fn, as_buildable, always_inline=experimental_always_inline)
+        fn, as_buildable, always_inline=experimental_always_inline
+    )
 
   # Decorator with empty parenthesis.
   if fn is None:
     return make_auto_config
   else:
     return make_auto_config(fn)
 
@@ -944,29 +968,29 @@
     An ``AutoConfig`` that corresponds to ``fn``.
   """
 
   if experimental_always_inline is None:
     experimental_always_inline = True
 
   def make_unconfig(fn) -> AutoConfig:
-
     @functools.wraps(fn)
     def python_implementation(*args, **kwargs):
       previous = building._state.in_build  # pytype: disable=module-attr # pylint: disable=protected-access
       building._state.in_build = False  # pytype: disable=module-attr # pylint: disable=protected-access
       try:
         cfg = fn(*args, **kwargs)
         return building.build(cfg)
       finally:
         building._state.in_build = previous  # pytype: disable=module-attr # pylint: disable=protected-access
 
     return AutoConfig(
         func=python_implementation,
         buildable_func=fn,
-        always_inline=experimental_always_inline)
+        always_inline=experimental_always_inline,
+    )
 
   # We use this pattern to support using the decorator with and without
   # parenthesis.
   if fn is None:
     return make_unconfig
   return make_unconfig(fn)
 
@@ -1016,28 +1040,35 @@
       the root of a Fiddle DAG that corresponds to it.
 
   Raises:
     ValueError: If ``buildable`` is not a ``Config``, or if ``buildable``
       doesn't correspond to an ``auto_config``'d function.
   """
   if not isinstance(buildable, config.Config):
-    raise ValueError('Cannot `inline` non-Config buildables; '
-                     f'{type(buildable)} is not compatible.')
+    raise ValueError(
+        'Cannot `inline` non-Config buildables; '
+        f'{type(buildable)} is not compatible.'
+    )
   if not is_auto_config(buildable.__fn_or_cls__):
-    raise ValueError('Cannot `inline` a non-auto_config function; '
-                     f'`{buildable.__fn_or_cls__}` is not compatible.')
+    raise ValueError(
+        'Cannot `inline` a non-auto_config function; '
+        f'`{buildable.__fn_or_cls__}` is not compatible.'
+    )
   # Evaluate the `as_buildable` interpretation.
   auto_config_fn = cast(AutoConfig, buildable.__fn_or_cls__)
   tmp_config = auto_config_fn.as_buildable(**buildable.__arguments__)
   if not isinstance(tmp_config, config.Buildable):
-    raise ValueError('You cannot currently inline functions that do not return '
-                     '`fdl.Buildable`s.')
+    raise ValueError(
+        'You cannot currently inline functions that do not return '
+        '`fdl.Buildable`s.'
+    )
 
   mutate_buildable.move_buildable_internals(
-      source=tmp_config, destination=buildable)
+      source=tmp_config, destination=buildable
+  )
 
 
 def _getsource(fn: Any) -> str:
   """Returns the source code for callable `fn`."""
   if _is_lambda(fn):
     return _getsource_for_lambda(fn)
   else:
@@ -1049,19 +1080,20 @@
 
 def _is_lambda(fn: Any) -> bool:
   """Returns True if `fn` is a lambda function."""
   if not inspect.isfunction(fn):
     return False
   if not (hasattr(fn, '__name__') and hasattr(fn, '__code__')):
     return False
-  return ((fn.__name__ == '<lambda>') or (fn.__code__.co_name == '<lambda>'))
+  return (fn.__name__ == '<lambda>') or (fn.__code__.co_name == '<lambda>')
 
 
 class _LambdaFinder(cst.CSTVisitor):
   """CST Visitor that searches for the source code for a given lambda func."""
+
   METADATA_DEPENDENCIES = (cst.metadata.PositionProvider,)
 
   def __init__(self, lambda_fn):
     super().__init__()
     self.lambda_fn = lambda_fn
     self.lineno = lambda_fn.__code__.co_firstlineno
     self.candidates = []
@@ -1088,23 +1120,25 @@
   if len(lambda_finder.candidates) == 1:
     lambda_node = lambda_finder.candidates[0]
     return cst.Module(body=[lambda_node]).code
 
   elif not lambda_finder.candidates:
     raise ValueError(
         'Fiddle auto_config was unable to find the source code for '
-        f'{fn}: could not find lambda on line {lambda_finder.lineno}.')
+        f'{fn}: could not find lambda on line {lambda_finder.lineno}.'
+    )
   else:
     # TODO(b/258671226): If desired, we could narrow down which lambda is
     # used based on the signature (or even fancier things like the checking
     # fn.__code__.co_names).
     raise ValueError(
         'Fiddle auto_config was unable to find the source code for '
         f'{fn}: multiple lambdas found on line {lambda_finder.lineno}; '
-        'try moving each lambda to its own line.')
+        'try moving each lambda to its own line.'
+    )
 
 
 def with_buildable_func(
     buildable_func: Callable[..., Any]
 ) -> Callable[..., Any]:
   """A decorator that adds an auto_config-only code path."""
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/auto_config_policy.py` & `fiddle-0.3.0/fiddle/_src/experimental/auto_config_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 import itertools
 import logging
 import types
 import typing
 
 from fiddle import building
 from fiddle._src import config
+from fiddle._src import partial
 from fiddle._src.experimental import autobuilders
 
 Policy = typing.Callable[[typing.Type[typing.Any]], bool]
 
 BUILTIN_LIST = [
     ArithmeticError,
     AssertionError,
@@ -178,15 +179,15 @@
     zip,
 ]
 
 V1_SKIPLIST = [
     autobuilders.Registry.config,
     building.build,
     config.Config,
-    config.Partial,
+    partial.Partial,
     copy.copy,
     copy.deepcopy,
     inspect.signature,
     itertools.accumulate,
     itertools.chain,
     itertools.chain.from_iterable,
     itertools.combinations,
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/auto_config_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/auto_config_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 
 import ast
 import copy
 import dataclasses
 import functools
 import inspect
 import sys
-from typing import Any
+from typing import Any, TypeVar
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import arg_factory
 from fiddle._src.experimental import auto_config
 from fiddle._src.experimental import auto_config_policy
 from fiddle._src.experimental import autobuilders as ab
 from fiddle._src.testing import test_util
+import pytype_extensions
 
 
 def basic_fn(arg, kwarg='test'):
   return {'arg': arg, 'kwarg': kwarg}
 
 
 def fn_with_kwargs(**kwargs):
@@ -83,15 +84,18 @@
 
   Returns:
     5
   """
   return pass_through(5)
 
 
-def pass_through(arg):
+T = TypeVar('T')
+
+
+def pass_through(arg: T) -> T:
   return arg
 
 
 def _line_number():
   return sys._getframe(1).f_lineno
 
 
@@ -119,14 +123,18 @@
       ),
       (
           'a, b.c = v',
           (
               '(a, _attr_save_temp_0) = v\n'
               "__auto_config_attr_save_handler__(b, 'c', _attr_save_temp_0)"
           ),
+          (
+              'a, _attr_save_temp_0 = v\n'
+              "__auto_config_attr_save_handler__(b, 'c', _attr_save_temp_0)"
+          ),
       ),
       (
           'a = b = c',
           'a = b = c',
       ),
       (
           'a, b.c = x.y.z = foo.bar',
@@ -134,14 +142,22 @@
               '(a, _attr_save_temp_0) = _attr_save_temp_1 = '
               "__auto_config_attr_load_handler__(foo, 'bar')\n"
               "__auto_config_attr_save_handler__(b, 'c', _attr_save_temp_0)\n"
               '__auto_config_attr_save_handler__('
               "__auto_config_attr_load_handler__(x, 'y'), "
               "'z', _attr_save_temp_1)"
           ),
+          (
+              'a, _attr_save_temp_0 = _attr_save_temp_1 = '
+              "__auto_config_attr_load_handler__(foo, 'bar')\n"
+              "__auto_config_attr_save_handler__(b, 'c', _attr_save_temp_0)\n"
+              '__auto_config_attr_save_handler__('
+              "__auto_config_attr_load_handler__(x, 'y'), "
+              "'z', _attr_save_temp_1)"
+          ),
       ),
       # Test transformations when Assign.value is a function call.
       # This test will ensure calls to ``functools.partial`` are replaced by
       # ``fdl.Partial`` properly.
       (
           'a.b.c = functools.partial(foo, x.y)',
           (
@@ -163,24 +179,32 @@
           ),
       ),
       ('a.b[1] = 123', "__auto_config_attr_load_handler__(a, 'b')[1] = 123"),
       (
           # TODO(b/288479702): Add validation for ast.Starred pattern.
           'a, *a.b = foo.bar',
           "(a, *a.b) = __auto_config_attr_load_handler__(foo, 'bar')",
+          "a, *a.b = __auto_config_attr_load_handler__(foo, 'bar')",
       ),
   )
-  def test_attribute_save(self, source, expected):
+  def test_attribute_save(self, source, expected, py11_expected=None):
     version = sys.version_info
     # ast.unparse is available only after Python 3.9
     if version.major >= 3 and version.minor >= 9:
       transfomer = auto_config._AutoConfigNodeTransformer(source, 'dummy.py', 0)
       node = ast.parse(source)
       node = transfomer.visit(node)
-      self.assertEqual(ast.unparse(node), expected)
+      # `ast.unparse` has different behaviors since Python 3.11, for example,
+      # ast.unparse(ast.parse('a, b = c'))
+      # Before Python 3.11, it returns: '(a, b) = c'
+      # From Python 3.11, it returns: 'a, b = c'
+      if version.minor >= 11 and py11_expected is not None:
+        self.assertEqual(ast.unparse(node), py11_expected)
+      else:
+        self.assertEqual(ast.unparse(node), expected)
 
 
 class AutoConfigTest(parameterized.TestCase, test_util.TestCase):
 
   def test_create_basic_config(self):
     expected_config = fdl.Config(FrozenSampleClass, 1, arg2=2)
 
@@ -478,15 +502,15 @@
 
     class CustomPartial(fdl.Partial):
       pass
 
     class CustomArgFactory(fdl.ArgFactory):
       pass
 
-    config_types = auto_config.ConfigTypes(
+    config_types = auto_config.ConfigTypes(  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
         config_cls=CustomConfig,
         partial_cls=CustomPartial,
         arg_factory_cls=CustomArgFactory,
     )
 
     def make_int() -> int:
       return 42
@@ -709,15 +733,15 @@
       def my_fn(self, x):
         return basic_fn(x, kwarg=super().method())
 
     instance = MyClass()
     cfg = instance.my_fn.as_buildable('a')
     self.assertEqual(fdl.get_callable(cfg), basic_fn)
     self.assertEqual(cfg.arg, 'a')
-    self.assertEqual(cfg.kwarg, fdl.Config(super(MyClass, instance).method))
+    self.assertEqual(cfg.kwarg, fdl.Config(super(MyClass, instance).method))  # pytype: disable=invalid-annotation  # use-fiddle-overlay
 
   def test_custom_policy(self):
 
     def make_list(max_value):
       return list(range(max_value))
 
     def custom_policy(fn):
@@ -755,14 +779,19 @@
       )
 
     cfg = make_sample.as_buildable(5)
     self.assertEqual(cfg.arg1, 5)
     self.assertEqual(cfg.arg2.arg1, fdl.Config(pass_through, 5))
     self.assertEqual(cfg.arg2.arg2, 5)
 
+  def test_exemption_type_inference(self):
+    exempted_func = auto_config.exempt(pass_through)
+    value = exempted_func(42)
+    pytype_extensions.assert_type(value, int)
+
   def test_lambda_supported_in_decorator(self):
     @auto_config.auto_config(experimental_exemption_policy=lambda x: False)
     def make_sample():
       return dict(arg1=3)
 
     expected = fdl.Config(dict, arg1=3)
     self.assertEqual(make_sample.as_buildable(), expected)
@@ -806,15 +835,15 @@
       _ = {obj: 1}
 
     @auto_config.auto_config
     def make_sample(obj):
       return obj(1)
 
     cfg = make_sample.as_buildable(obj)
-    self.assertEqual(cfg, fdl.Config(obj, arg1=1))
+    self.assertEqual(cfg, fdl.Config(obj, arg1=1))  # pytype: disable=invalid-annotation  # use-fiddle-overlay
 
   def test_control_flow_if(self):
 
     def test_config(condition):
       if condition:
         return pass_through('true branch')
       else:
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/__init__.py` & `fiddle-0.3.0/fiddle/_src/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders.py` & `fiddle-0.3.0/fiddle/_src/experimental/autobuilders/autobuilders.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/autobuilders/autobuilders_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py` & `fiddle-0.3.0/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy.py` & `fiddle-0.3.0/fiddle/_src/experimental/daglish_legacy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/daglish_legacy_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/daglish_legacy_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/dataclasses.py` & `fiddle-0.3.0/fiddle/_src/experimental/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/dataclasses_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/dict_config.py` & `fiddle-0.3.0/fiddle/_src/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/dict_config_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/dict_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/lazy_imports.py` & `fiddle-0.3.0/fiddle/_src/experimental/lazy_imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 import builtins
 import contextlib
 import dataclasses
 import functools
 import importlib
 import inspect
+import logging
 from typing import Any, Iterator, Optional
 
 
 @contextlib.contextmanager
-def lazy_imports(kw_only=False) -> Iterator[None]:
+def lazy_imports(kw_only=True) -> Iterator[None]:
   """Context manager which replaces import statements with lazy imports.
 
   A ProxyObject is returned for the import statement as dummy module. The
   actual module is not imported until calling `fdl.build()` on Fiddle
   `Buildable` objects.
 
 
@@ -75,25 +76,50 @@
 
   partial = fdl.Partial(module_2.my_function)
   my_fn = fdl.build(partial)  # module_2 not loaded here.
   assert isinstance(my_fn.func, ProxyObject)
   out = my_fn(x=1, ...)  # module_2 is loaded here during call time.
   ```
 
+  NOTE: When using positional arguments for lazy-imported functions/classes,
+  be aware that the config will likely be different from normal-imported
+  functions/classes. As Fiddle does not have signature information for
+  lazy-imported modules, values for positional arguments, like value 'v' in the
+  example below, will be saved as positional-only arguments, and using the index
+  0 as the key in `__arguments__`, even if it actually corresponds to a
+  positional-or-keyword argument.
+
+  # In foo.py
+  def bar(x):
+    return x
+
+  # In file_1.py
+  with fdl.lazy_import():
+    import foo
+  cfg_1 = fdl.Config(foo.bar, 'v')
+  assert cfg_1.__arguments__ == {0: 'v'}
+
+  # In file_2.py
+  import foo
+  cfg_2 = fdl.Config(foo.bar, 'v')
+  assert cfg_2.__arguments__ == {'x': 'v'}
+
 
   Args:
     kw_only: Whether to only allow keyword args usage for lazy imported modules.
+      Defaults to True.
 
   Yields:
     None
   """
   if not kw_only:
-    raise NotImplementedError(
-        'Positional arguments are not supported yet, please set `kw_only` as '
-        'True for `lazy_imports`.'
+    logging.warning(
+        'When using positional arguments for lazy-imported functions/classes,'
+        ' be aware that the config will likely be different from'
+        'normal-imported functions/classes.'
     )
 
   # Need to mock `__import__` (instead of `sys.meta_path`, as we do not want
   # to modify the `sys.modules` cache in any way)
   origin_import = builtins.__import__
   try:
     builtins.__import__ = functools.partial(
@@ -210,15 +236,15 @@
         kw_only=self.kw_only,
         parent=self,
         is_import=False,
     )
     return ret
 
   def __hash__(self):
-    return hash((self.qualname, self.parent))
+    return hash((self.qualname, self.parent, self.kw_only))
 
   def __eq__(self, other):
     if not isinstance(other, ProxyObject):
       return False
     return self.qualname == other.qualname and self.parent == other.parent
 
   def child_import(self, name: str) -> 'ProxyObject':
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/lazy_imports_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/lazy_imports_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import inspect
 from typing import Any
 import unittest
 
 from absl.testing import absltest
 from fiddle._src import building
 from fiddle._src import config as config_lib
+from fiddle._src import partial
 from fiddle._src.experimental import lazy_imports
 from fiddle._src.experimental import serialization
 
 
 @dataclasses.dataclass
 class SampleSumClass:
   arg1: Any
@@ -115,23 +116,14 @@
           inspect.getmodule(c02).__name__,
           'fiddle._src.experimental.lazy_imports',
       )
 
 
 class BuildLazyImportsTest(absltest.TestCase, unittest.TestCase):
 
-  def test_args(self):
-    # TODO(b/291129675): Support args for lazy imported classes/functions.
-    with self.assertRaisesRegex(
-        NotImplementedError, 'Positional arguments are not supported yet'
-    ):
-      with lazy_imports.lazy_imports(kw_only=False):
-        from fiddle._src.experimental import lazy_imports_test_example  # pylint: disable=g-import-not-at-top
-      _ = config_lib.Config(lazy_imports_test_example.MyDataClass, 1, 2)
-
   def test_import_as(self):
     with lazy_imports.lazy_imports(kw_only=True):
       from fiddle._src.experimental import lazy_imports_test_example as example  # pylint: disable=g-import-not-at-top
       from fiddle._src.experimental.lazy_imports_test_example import my_function as my_fn  # pylint: disable=g-import-not-at-top, g-importing-member
 
     with self.subTest('dataclass'):
       cfg = config_lib.Config(example.MyDataClass, x=1, y=2)
@@ -181,21 +173,42 @@
 
     foo = building.build(cfg)
     self.assertEqual(foo.sum(), 753)
 
   def test_partial(self):
     with lazy_imports.lazy_imports(kw_only=True):
       from fiddle._src.experimental import lazy_imports_test_example  # pylint: disable=g-import-not-at-top
-    cfg = config_lib.Partial(lazy_imports_test_example.my_function)
+    cfg = partial.Partial(lazy_imports_test_example.my_function)
     obj = building.build(cfg)
     # Note that the lazy imported module is not loaded at build time but delayed
     # until call time when working with fdl.Partial.
     self.assertIsInstance(obj.func, lazy_imports.ProxyObject)  # pytype: disable=attribute-error
     self.assertEqual(obj(x=5), 128)
 
+  def test_positional_args(self):
+    with lazy_imports.lazy_imports(kw_only=False):
+      from fiddle._src.experimental import lazy_imports_test_example  # pylint: disable=g-import-not-at-top
+    cfg = config_lib.Config(lazy_imports_test_example.MyDataClass, 1, 2)
+    obj = building.build(cfg)
+    self.assertEqual(obj.sum(), 3)
+
+  def test_partial_w_positional_args(self):
+    with lazy_imports.lazy_imports(kw_only=False):
+      from fiddle._src.experimental import lazy_imports_test_example  # pylint: disable=g-import-not-at-top
+    cfg = partial.Partial(lazy_imports_test_example.my_function, 5)
+    obj = building.build(cfg)
+    self.assertIsInstance(obj.func, lazy_imports.ProxyObject)  # pytype: disable=attribute-error
+    self.assertEqual(obj(2), 130)
+
+  def test_kw_only_check(self):
+    with lazy_imports.lazy_imports(kw_only=True):
+      from fiddle._src.experimental import lazy_imports_test_example  # pylint: disable=g-import-not-at-top
+    with self.assertRaisesRegex(TypeError, 'too many positional arguments'):
+      _ = config_lib.Config(lazy_imports_test_example.MyDataClass, 1, 2)
+
 
 class SerializationTest(absltest.TestCase, unittest.TestCase):
 
   def test_regular_import(self):
     from fiddle._src.experimental import lazy_imports_test_example  # pylint: disable=g-import-not-at-top
 
     x = config_lib.Config(lazy_imports_test_example.MyDataClass, x=1, y=2)
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/lazy_imports_test_example.py` & `fiddle-0.3.0/fiddle/_src/experimental/lazy_imports_test_example.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # limitations under the License.
 
 """Example classes/functions for testing lazy imports API."""
 
 import dataclasses
 
 
-def my_function(x):
-  return 123 + x
+def my_function(x, y=0):
+  return 123 + x + y
 
 
 @dataclasses.dataclass(frozen=True)
 class MyDataClass:
   x: int
   y: int
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/namespace_config.py` & `fiddle-0.3.0/fiddle/_src/experimental/namespace_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/namespace_config_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/namespace_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/serialization.py` & `fiddle-0.3.0/fiddle/_src/experimental/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import sys
 import types
 from typing import Any, Dict, Iterable, List, Optional, Type
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src import reraised_exception
+from fiddle._src import special_overrides
 from fiddle._src.experimental import daglish_legacy
 from fiddle._src.experimental import lazy_imports
 
 
 _VERSION = '0.0.1'
 
 
@@ -281,14 +282,17 @@
     ModuleNotFoundError: If `module` can't be found.
     AttributeError: If `symbol` can't be accessed on `module`.
     PyrefPolicyError: If importing `symbol` from `module` is disallowed by
       this `PyrefPolicy`.
   """
   value = PyrefPolicyError.PRE_IMPORT
   if policy.allows_import(module, symbol):
+    module = special_overrides.maybe_get_module_override_for_migrated_serialization_symbol(
+        module, symbol
+    )
     make_message = functools.partial(_fiddle_pyref_context, module, symbol)
     with reraised_exception.try_with_lazy_message(make_message):
       value = importlib.import_module(module)
       for attr_name in symbol.split('.'):
         value = getattr(value, attr_name)
 
     if policy.allows_value(value):
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/transform.py` & `fiddle-0.3.0/fiddle/_src/experimental/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 """Transformation functions for Fiddle buildables."""
 
 from typing import Any, Callable, Iterable, Optional, TypeVar, Union
 
 from fiddle import daglish
 from fiddle._src import config
+from fiddle._src import partial
 
 
 # Any subclass of Buildable
 AnyBuildable = TypeVar(
     "AnyBuildable", bound=Union[config.Buildable, Iterable[config.Buildable]])
 
 
@@ -70,13 +71,14 @@
   """
 
   def transform(value, state: daglish.State):
     # This transform is guaranteed to be safe for fdl.Partial, but subclasses
     # may have specialized behavior such that this transformation no longer
     # makes sense, so do not apply this to subclasses of fdl.Partial.
     # pylint: disable-next=unidiomatic-typecheck
-    if type(value) is config.Partial and not config.ordered_arguments(
-        value, exclude_equal_to_default=True):
+    if type(value) is partial.Partial and not config.ordered_arguments(
+        value, include_equal_to_default=False
+    ):
       value = config.get_callable(value)
     return state.map_children(value)
 
   return daglish.MemoizedTraversal.run(transform, buildable)
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/transform_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/transform_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,44 +44,44 @@
     rather our assumptions about how Python works. Currently, we assume (and
     tested) that Python interns (i.e. share the same instance) tuples that have
     the same value but are declared in different locations in the code. If this
     test ever fails, then it likely means Python is no longer interning tuples,
     so there's no need for unintern_tuples_of_literals as each tuple will have a
     different ID.
     """
-    foo_cfg = fdl.Config(Foo, a_tuple=(1, 2, 3), another_tuple=(1, 2, 3))
+    foo_cfg = fdl.Config(Foo, a_tuple=(1, 2, 3), another_tuple=(1, 2, 3))  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
     self.assertIs(
         foo_cfg.a_tuple, foo_cfg.another_tuple,
         "This likely means Python is no longer interning tuples. We can remove "
         "unintern_tuples_of_literals in that case.")
 
   def test_unintern_tuple_of_literals(self):
-    foo_cfg = fdl.Config(Foo, a_tuple=(1, 2, 3), another_tuple=(1, 2, 3))
+    foo_cfg = fdl.Config(Foo, a_tuple=(1, 2, 3), another_tuple=(1, 2, 3))  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
     uninterned_foo_cfg = transform.unintern_tuples_of_literals(foo_cfg)
 
     self.assertNotEqual(
         id(uninterned_foo_cfg.a_tuple), id(uninterned_foo_cfg.another_tuple),
         "a_tuple and another_tuple have the same id indicating they're the "
         "same instance, expected them to be different instances after "
         "uninterning.")
 
   def test_unintern_tuple_of_literals_in_list(self):
-    foo_cfg = fdl.Config(Foo, a_tuple=(1, 2, 3), another_tuple=(1, 2, 3))
+    foo_cfg = fdl.Config(Foo, a_tuple=(1, 2, 3), another_tuple=(1, 2, 3))  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
 
     uninterned_foo_cfg = transform.unintern_tuples_of_literals(foo_cfg)
 
     self.assertNotEqual(
         id(uninterned_foo_cfg.a_tuple), id(uninterned_foo_cfg.another_tuple),
         "a_tuple and another_tuple have the same id indicating they're the "
         "same instance, expected them to be different instances after "
         "uninterning.")
 
   def test_unintern_tuple_of_non_literals(self):
     not_tuple_of_literals = ([1, 2], 3, 4)
-    foo_cfg = fdl.Config(
+    foo_cfg = fdl.Config(  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
         Foo, a_tuple=not_tuple_of_literals, another_tuple=not_tuple_of_literals)
 
     uninterned_foo_cfg = transform.unintern_tuples_of_literals(foo_cfg)
 
     self.assertEqual(
         id(uninterned_foo_cfg.a_tuple), id(uninterned_foo_cfg.another_tuple),
         "a_tuple and another_tuple have different id indicating they're the "
@@ -91,16 +91,16 @@
   def test_replace_unconfigured_partials_with_callables_replace_top_level(self):
     self.assertIs(
         Foo,
         transform.replace_unconfigured_partials_with_callables(
             fdl.Partial(Foo)))
 
   def test_replace_unconfigured_partials_with_callables_replace_nested(self):
-    cfg = fdl.Config(Foo, a_callable=fdl.Partial(Foo))
-    expected_cfg = fdl.Config(Foo, a_callable=Foo)
+    cfg = fdl.Config(Foo, a_callable=fdl.Partial(Foo))  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
+    expected_cfg = fdl.Config(Foo, a_callable=Foo)  # pytype: disable=wrong-arg-types  # use-fiddle-overlay
     self.assertEqual(
         expected_cfg,
         transform.replace_unconfigured_partials_with_callables(cfg))
 
   def test_replace_unconfigured_partials_with_callables_replace_if_only_defaults(
       self):
     # If an argument is passed to the Partial but it has the same value as the
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/visualize.py` & `fiddle-0.3.0/fiddle/_src/experimental/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def _helper(value, substate: daglish.State) -> bool:
       if not substate.is_traversable(value) or daglish.is_immutable(value):
         return True
 
       for sub_path in substate.get_all_paths():
         if not _goes_through_node(sub_path):
           return False
-      return all(substate.flattened_map_children(value).values)
+      return all(substate.yield_map_child_values(value))
 
     # Creates a sub-traversal using a different function. We eventually might
     # make this part of the daglish API.
     sub_traversal = daglish.MemoizedTraversal(
         traversal_fn=_helper,
         root_obj=parent_state.traversal.root_obj,
         registry=parent_state.traversal.registry,
@@ -142,15 +142,15 @@
     if isinstance(value, config_lib.Buildable):
       deep_defaults = {}
       if remove_deep_defaults:
         deep_defaults = _get_default(value).__arguments__
 
       should_copy = True
       for name, attr_value in list(value.__arguments__.items()):
-        param = value.__signature__.parameters.get(name, None)
+        param = value.__signature_info__.parameters.get(name, None)
         if param is None:
           continue
         param_default = (
             deep_defaults[name] if name in deep_defaults else param.default
         )
         if (
             param.kind != inspect.Parameter.VAR_KEYWORD
@@ -195,16 +195,16 @@
     return sum(1 if isinstance(elt, daglish.Attr) else 0 for elt in path)
 
   def traverse(node, state: daglish.State) -> None:
     if isinstance(node, config_lib.Buildable):
       all_paths = state.get_all_paths(allow_caching=True)
       node_to_depth[id(node)] = min(_path_len(path) for path in all_paths)
       id_to_node[id(node)] = node
-    if state.is_traversable(node):
-      state.flattened_map_children(node)
+    for _ in state.yield_map_child_values(node, ignore_leaves=True):
+      pass  # Run lazy iterator.
 
   daglish.MemoizedTraversal.run(traverse, config)
 
   return [
       id_to_node[key]
       for key, node_depth in node_to_depth.items()
       if node_depth > depth
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/with_tags.py` & `fiddle-0.3.0/fiddle/_src/experimental/with_tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/with_tags_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/with_tags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization.py` & `fiddle-0.3.0/fiddle/_src/experimental/yaml_serialization.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 """
 
 import collections
 import inspect
 from typing import Any
 
 from fiddle._src import config as config_lib
+from fiddle._src import partial
 from fiddle._src import tagging
 import yaml
 
 
 def _defaultdict_representer(dumper, data):
   return dumper.represent_dict(data)
 
@@ -70,15 +71,15 @@
           "tags": [tag.name for tag in data.tags],
           "value": data.value,
       },
   )
 
 
 yaml.SafeDumper.add_representer(config_lib.Config, _config_representer)
-yaml.SafeDumper.add_representer(config_lib.Partial, _partial_representer)
+yaml.SafeDumper.add_representer(partial.Partial, _partial_representer)
 yaml.SafeDumper.add_representer(
     tagging.TaggedValueCls, _taggedvalue_representer
 )
 
 
 def dump_yaml(value: Any) -> str:
   """Returns the YAML serialization of `value`.
```

### Comparing `fiddle-0.2.9/fiddle/_src/experimental/yaml_serialization_test.py` & `fiddle-0.3.0/fiddle/_src/experimental/yaml_serialization_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/__init__.py` & `fiddle-0.3.0/fiddle/_src/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/flax_test.py` & `fiddle-0.3.0/fiddle/_src/extensions/flax_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/jax.py` & `fiddle-0.3.0/fiddle/_src/extensions/jax.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/seqio.py` & `fiddle-0.3.0/fiddle/_src/extensions/seqio.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/seqio_test.py` & `fiddle-0.3.0/fiddle/_src/extensions/seqio_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/tf.py` & `fiddle-0.3.0/fiddle/_src/extensions/tf.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/extensions/tf_test.py` & `fiddle-0.3.0/fiddle/_src/extensions/tf_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/graphviz.py` & `fiddle-0.3.0/fiddle/_src/graphviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 import colorsys
 import copy
 import dataclasses
 import functools
 import html
 import itertools
 import types
-
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Set, Tuple, Type, Union
 
 from fiddle._src import config as config_lib
 from fiddle._src import daglish
 from fiddle._src import diffing
 from fiddle._src import graphviz_custom_object
+from fiddle._src import partial
 from fiddle._src import tag_type
 from fiddle._src import tagging
 from fiddle._src.codegen import formatting_utilities
 from fiddle._src.experimental import daglish_legacy
 from fiddle._src.experimental import visualize
 import graphviz
 
@@ -247,15 +247,15 @@
                   style: str = 'solid'):
     """Constructs a header table row."""
     tr = self.tag('tr')
     header_td = self.tag('td', colspan=colspan, bgcolor=bgcolor, style=style)
     return tr(header_td(header))
 
   def _config_header_style(self, config: config_lib.Buildable) -> str:
-    if isinstance(config, (config_lib.Partial, config_lib.ArgFactory)):
+    if isinstance(config, (partial.Partial, partial.ArgFactory)):
       return 'dashed'
     else:
       return 'solid'
 
   def render(self, value: Any) -> graphviz.Graph:
     """Renders the given value, recursively rendering any nested values."""
     self._find_shared_value_ids(value)
@@ -829,18 +829,18 @@
   changed_parent_ids = _find_mutable_values_with_changed_parents(
       structure_with_changed_values)
 
   def visit(value, state: daglish.State):
     """Returns true if any child has changed."""
     parents_changed = id(value) in changed_parent_ids
     if state.is_traversable(value):
-      subtraversal = state.flattened_map_children(value)
-      any_changed = any(subtraversal.values)
+      child_results = list(state.yield_map_child_values(value))
+      any_changed = any(child_results)
       if isinstance(value, dict) and id(value) in old_value_ids:
-        _trim_dict(value, subtraversal.values)
+        _trim_dict(value, child_results)
       return any_changed or parents_changed
     elif isinstance(value, _ChangedValue):
       state.call(value.old_value, daglish.Attr('old_value'))
       state.call(value.new_value, daglish.Attr('new_value'))
       return True
     elif isinstance(value, _ChangedBuildable):
       args_changed = [
@@ -862,15 +862,16 @@
 
 def _find_mutable_values_with_changed_parents(structure_with_changed_values):
   """Returns a set of ids of mutable objects whose parent(s) changed."""
   result = set()
 
   def visit(value, state: daglish.State):
     if state.is_traversable(value):
-      state.flattened_map_children(value)
+      for _ in state.yield_map_child_values(value):
+        pass  # Run lazy iterator.
     elif isinstance(value, _ChangedValue):
       assert value.old_value is not value.new_value
       if daglish.is_memoizable(value.old_value):
         result.add(id(value.old_value))
       if daglish.is_memoizable(value.new_value):
         result.add(id(value.new_value))
       state.call(value.old_value, daglish.Attr('old_value'))
```

### Comparing `fiddle-0.2.9/fiddle/_src/graphviz_custom_object.py` & `fiddle-0.3.0/fiddle/_src/graphviz_custom_object.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/history.py` & `fiddle-0.3.0/fiddle/_src/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,90 +31,95 @@
     different location provider; see the documentation on the `custom_location`
     context manager for an example.
 """
 
 import contextlib
 import dataclasses
 import enum
+import inspect
 import itertools
 import os
-import re
 import threading
-import traceback
-from typing import Any, Callable, FrozenSet, Iterator, Optional, Set, Union
+from typing import Any, Callable, FrozenSet, Iterator, Optional, Set, Tuple, Union
 
 from fiddle._src import tag_type
 
 # An incrementing counter to allow for time-travel debugging.
 _set_counter = itertools.count()
 
 
 @dataclasses.dataclass(frozen=True)
 class Location:
   """Information about where a parameter was set."""
   filename: str
   line_number: int
   function_name: Optional[str]
 
-  def __str__(self) -> str:
+  def format(self, max_filename_parts: Optional[int] = None):
+    filename = self.filename
+    if max_filename_parts is not None:
+      filename_parts = filename.split(os.path.sep)
+      if len(filename_parts) > max_filename_parts:
+        filename = os.path.sep.join(
+            ["...", *filename_parts[-max_filename_parts:]]
+        )
     if self.function_name is None:
-      return f"{self.filename}:{self.line_number}"
-    return f"{self.filename}:{self.line_number}:{self.function_name}"
+      return f"{filename}:{self.line_number}"
+    return f"{filename}:{self.line_number}:{self.function_name}"
+
+  def __str__(self) -> str:
+    return self.format()
 
   def __deepcopy__(self, memo):
     del memo  # unused
     return self
 
 
 # A function that returns a location.
 LocationProvider = Callable[[], Location]
 
-_exclude_locations: Set[str] = set(
+_exclude_locations: Tuple[str, ...] = tuple(
     map(
         os.path.normpath,
         [
             "fiddle/_src/config.py",
+            "fiddle/_src/copying.py",
             "fiddle/_src/daglish.py",
             "fiddle/_src/history.py",
             "fiddle/_src/materialize.py",
+            "fiddle/_src/mutate_buildable.py",
             "fiddle/_src/experimental/auto_config.py",
         ],
     )
 )
 
 
-def _compile_exclude_regex():
-  return re.compile(r"({})$".format("|".join(
-      re.escape(location) for location in _exclude_locations)))
-
-
-_exclude_regex = _compile_exclude_regex()
-
-
 def add_exclude_location(location: str):
   """Adds a filename pattern to exclude from history stacktraces."""
-  global _exclude_regex
-  _exclude_locations.add(location)
-  _exclude_regex = _compile_exclude_regex()
+  global _exclude_locations
+  _exclude_locations += (location,)
 
 
 def _stacktrace_location_provider() -> Location:
   """Returns a string corresponding to the user-function that set the field.
 
   Raises:
     RuntimeError: if no suitable stack frame can be found.
   """
-  for frame, line_number in traceback.walk_stack(None):
+  frame = inspect.currentframe()
+  while frame:
+    line_number = frame.f_lineno
     filename = frame.f_code.co_filename
-    if not _exclude_regex.search(filename):
+    if not filename.endswith(_exclude_locations):
       function_name = frame.f_code.co_name
       return Location(
           filename=filename,
           line_number=line_number,
           function_name=function_name)
+    frame = frame.f_back
   raise RuntimeError("Cannot find a suitable frame in the stack trace!")
 
 
 # The location provider to use when instantiating new HistoryEntry's.
 _location_provider: LocationProvider = _stacktrace_location_provider
```

### Comparing `fiddle-0.2.9/fiddle/_src/history_test.py` & `fiddle-0.3.0/fiddle/_src/history_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,30 @@
     self.assertEqual(str(location), "my_file.py:123")
     location = history.Location(
         filename="my_other_file.py",
         line_number=321,
         function_name="make_config")
     self.assertEqual(str(location), "my_other_file.py:321:make_config")
 
+  def test_location_formatting_concise(self):
+    location = history.Location(
+        filename="foo/bar/baz/my_file.py", line_number=123, function_name=None
+    )
+    self.assertEqual(location.format(3), ".../bar/baz/my_file.py:123")
+    self.assertEqual(location.format(2), ".../baz/my_file.py:123")
+    location = history.Location(
+        filename="foo/bar/baz/my_other_file.py",
+        line_number=321,
+        function_name="make_config",
+    )
+    self.assertEqual(
+        location.format(4), "foo/bar/baz/my_other_file.py:321:make_config"
+    )
+    self.assertEqual(location.format(1), ".../my_other_file.py:321:make_config")
+
   def test_entry_simple(self):
     entry = history.new_value("x", 1)
     self.assertEqual(entry.param_name, "x")
     self.assertEqual(entry.kind, history.ChangeKind.NEW_VALUE)
     self.assertEqual(entry.new_value, 1)
 
   def test_entry_deletion(self):
```

### Comparing `fiddle-0.2.9/fiddle/_src/materialize.py` & `fiddle-0.3.0/fiddle/_src/materialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,14 @@
 
   Args:
     value: A nested collection which may contain Buildable arguments.
   """
 
   def traverse(node, state: daglish.State):
     if isinstance(node, config.Buildable):
-      for arg in node.__signature__.parameters.values():
+      for arg in node.__signature_info__.parameters.values():
         if arg.default is not arg.empty and arg.name not in node.__arguments__:
           setattr(node, arg.name, arg.default)
-    if state.is_traversable(node):
-      state.flattened_map_children(node)
+    for _ in state.yield_map_child_values(node, ignore_leaves=True):
+      pass  # Run lazy iterator.
 
   daglish.MemoizedTraversal.run(traverse, value)
```

### Comparing `fiddle-0.2.9/fiddle/_src/materialize_test.py` & `fiddle-0.3.0/fiddle/_src/materialize_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/module_reflection.py` & `fiddle-0.3.0/fiddle/_src/module_reflection.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/module_reflection_test.py` & `fiddle-0.3.0/fiddle/_src/module_reflection_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/module_reflection_test_module.py` & `fiddle-0.3.0/fiddle/_src/module_reflection_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/printing.py` & `fiddle-0.3.0/fiddle/_src/printing.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 """Functions to output representations of `fdl.Buildable`s."""
 
 import copy
 import dataclasses
 import inspect
 import types
-from typing import Any, Iterator, List, Optional, Type
+from typing import Any, Dict, Iterator, List, Optional, Type
 
 from fiddle._src import config
 from fiddle._src import daglish
 from fiddle._src import history
 from fiddle._src import tagging
 from fiddle._src.codegen import formatting_utilities
 
@@ -41,17 +41,17 @@
       default_value = _format_value(
           self.parameter.default, raw_value_repr=False)
       return f'<[unset; default: {default_value}]>'
 
 
 def _has_nested_builder(value: Any, state=None) -> bool:
   state = state or daglish.MemoizedTraversal.begin(_has_nested_builder, value)
-  return (isinstance(value, config.Buildable) or
-          (state.is_traversable(value) and
-           any(state.flattened_map_children(value).values)))
+  return isinstance(value, config.Buildable) or (
+      state.is_traversable(value) and any(state.yield_map_child_values(value))
+  )
 
 
 def _path_str(path: daglish.Path) -> str:
   """Formats path in a way customized to this file.
 
   In the future, we may wish to consider a format that is readable for printing
   more arbitrary collections.
@@ -106,18 +106,18 @@
   if not path or not isinstance(path[-1], daglish.Attr):
     return None
   value = cfg
   for path_element in path[:-1]:
     value = path_element.follow(value)
   if isinstance(value, config.Buildable):
     try:
-      param = value.__signature__.parameters[path[-1].name]
+      param = value.__signature_info__.parameters[path[-1].name]
     except KeyError:
       # Try to use the kwarg annotation
-      for param in value.__signature__.parameters.values():
+      for param in value.__signature_info__.parameters.values():
         if param.kind == param.VAR_KEYWORD:
           return None if param.annotation is param.empty else param.annotation
       return None  # probably a kwarg
     return None if param.annotation is param.empty else param.annotation
 
 
 def _get_tags(cfg, path):
@@ -127,39 +127,42 @@
     if isinstance(child, daglish.Attr):
       parent = daglish.follow_path(cfg, path[:-1])
       if isinstance(parent, config.Buildable):
         return parent.__argument_tags__.get(child.name)
     return None
 
 
-def _rearrange_buildable_args_and_insert_unset_sentinels(
-    value: config.Buildable) -> config.Buildable:
+def _rearrange_buildable_args(
+    value: config.Buildable, insert_unset_sentinels: bool = True
+) -> config.Buildable:
   """Returns a copy of a Buildable with normalized arguments.
 
   This normalizes arguments by re-creating the __arguments__ dictionary in the
   order of the configured function or class' signature. It also inserts "unset"
   sentinels for values in the signature that don't have a value set.
 
   Args:
     value: Buildable to copy and normalize.
+    insert_unset_sentinels: If true, insert unset sentinels to arguments as the
+      default values.
 
   Returns:
     Copy of `value` with arguments normalized.
   """
   # TODO(b/243576914): Consider pulling part of this function into a shared
   # module, or achieving the same effect by modifying traversal order.
   value = copy.copy(value)
   old_arguments = dict(value.__arguments__)
   new_arguments = {}
-  for param_name, param in value.__signature__.parameters.items():
+  for param_name, param in value.__signature_info__.parameters.items():
     if param.kind in {param.VAR_KEYWORD, param.VAR_POSITIONAL}:
       continue
     elif param_name in old_arguments:
       new_arguments[param_name] = old_arguments.pop(param_name)
-    else:
+    elif insert_unset_sentinels:
       new_arguments[param_name] = _UnsetValue(param)
   new_arguments.update(old_arguments)  # Add in kwargs, in current order.
   object.__setattr__(value, '__arguments__', new_arguments)
   return value
 
 
 def as_str_flattened(cfg: config.Buildable,
@@ -186,27 +189,27 @@
 
     tags = _get_tags(cfg, state.current_path)
     if tags:
       value = tagging.TaggedValue(tags=tags, default=value)
 
     # Rearrange parameters in signature order, and add "unset" sentinels.
     if isinstance(value, config.Buildable):
-      value = _rearrange_buildable_args_and_insert_unset_sentinels(value)
+      value = _rearrange_buildable_args(value)
 
     if isinstance(value, tagging.TaggedValueCls):
       value = _TaggedValueWrapper(value)
       annotation = _get_annotation(cfg, state.current_path)
       yield _LeafSetting(state.current_path, annotation, value)
     elif not _has_nested_builder(value):
       annotation = _get_annotation(cfg, state.current_path)
       yield _LeafSetting(state.current_path, annotation, value)
     else:
       # value must be a Buildable or a traversable containing a Buidable.
       assert state.is_traversable(value)
-      for sub_result in state.flattened_map_children(value).values:
+      for sub_result in state.yield_map_child_values(value):
         yield from sub_result
 
   # Used in format_line below.  The use of getattr and the dummy type default
   # is to maintain Python 3.8 compatibility.
   dummy_type = type('', (), {})
   generic_alias = getattr(types, 'GenericAlias', dummy_type)
 
@@ -273,22 +276,23 @@
           yield from state.call(sub_value, daglish.Attr(name))
         else:
           path = (*state.current_path, daglish.Attr(name))
           yield _make_per_leaf_history_text(path, param_history, raw_value_repr)
 
       # Add in unset fields.
       unset_fields = sorted(
-          set(value.__signature__.parameters.keys()) -
-          set(value.__argument_history__.keys()))
+          set(value.__signature_info__.parameters.keys())
+          - set(value.__argument_history__.keys())
+      )
       for name in unset_fields:
         path = (*state.current_path, daglish.Attr(name))
         yield f'{_path_str(path)} = <[unset]>'
 
     elif state.is_traversable(value):
-      for sub_result in state.flattened_map_children(value).values:
+      for sub_result in state.yield_map_child_values(value):
         yield from sub_result
     else:
       yield f'{_path_str(state.current_path)} = {value}'
 
   return traverse(cfg)
 
 
@@ -326,7 +330,40 @@
     past = '\n' + past  # prefix with a newline.
   else:
     past = ''
   current_value = _format_value(
       value_history[-1].new_value, raw_value_repr=raw_value_repr)
   current = f'{current_value} @ {value_history[-1].location}'
   return f'{_path_str(path)} = {current}{past}'
+
+
+def as_dict_flattened(cfg: config.Buildable) -> Dict[str, Any]:
+  """Returns a flattened dict of cfg's paths (dot syntax) and values.
+
+  Default values and tags won't be included in the flattened dict.
+
+  Args:
+    cfg: A buildable to generate a flattened dict representation for.
+
+  Returns: A flattened Dict representation of `cfg`.
+  """
+
+  def dict_generate(value, state=None) -> Iterator[_LeafSetting]:
+    state = state or daglish.BasicTraversal.begin(dict_generate, value)
+
+    # Rearrange parameters in signature order.
+    if isinstance(value, config.Buildable):
+      value = _rearrange_buildable_args(value, insert_unset_sentinels=False)
+
+    if not _has_nested_builder(value):
+      yield _LeafSetting(state.current_path, None, value)
+    else:
+      # value must be a Buildable or a traversable containing a Buildable.
+      assert state.is_traversable(value)
+      for sub_result in state.yield_map_child_values(value):
+        yield from sub_result
+
+  args_dict = {}
+  for leaf in dict_generate(cfg):
+    args_dict[_path_str(leaf.path)] = leaf.value
+
+  return args_dict
```

### Comparing `fiddle-0.2.9/fiddle/_src/printing_test.py` & `fiddle-0.3.0/fiddle/_src/printing_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -394,18 +394,18 @@
         y = 'abc' @ .*/printing_test.py:\d+:test_simple_history""".strip('\n'))
     self.assertRegex(output, expected)
 
   def test_nested_in_collections(self):
     cfg = fdl.Config(fn_x_y,
                      [fdl.Config(fn_x_y, 1, '1'),
                       fdl.Config(SampleClass, 2)])
-    cfg.x[0].x = 3
-    cfg.x[1].a = 2  # Reset to same value.
-    cfg.x[0].y = 'abc'
-    cfg.x[0].x = 4
+    cfg.x[0].x = 3  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    cfg.x[1].a = 2  # Reset to same value.  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    cfg.x[0].y = 'abc'  # pytype: disable=unsupported-operands  # use-fiddle-overlay
+    cfg.x[0].x = 4  # pytype: disable=unsupported-operands  # use-fiddle-overlay
     output = printing.history_per_leaf_parameter(cfg)
     self.assertTrue(printing._has_nested_builder(cfg.x))
     expected = textwrap.dedent(rf"""
         __fn_or_cls__ = .*fn_x_y .+/printing_test.py:\d+:test_nested_in_collections
         x\[0\].__fn_or_cls__ = .*fn_x_y .+/printing_test.py:\d+:test_nested_in_collections
         x\[0\].x = 4 @ .*/printing_test.py:\d+:test_nested_in_collections
           - previously: 3 @ .*/printing_test.py:\d+:test_nested_in_collections
@@ -469,9 +469,168 @@
         \[1\].__fn_or_cls__ = <function fn_x_y at .*> @ {name}
         \[1\].y = 4 @ {name}
           - previously: 3 @ {name}
         \[1\].x = 10 @ {name}""".strip('\n'))
     self.assertRegex(output, expected)
 
 
+class AsFlattenedDictTests(absltest.TestCase):
+
+  def test_simple_flattened_dict(self):
+    cfg = fdl.Config(fn_x_y, 1, 'abc')
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 1, 'y': 'abc'}
+    self.assertEqual(output, expected)
+
+  def test_skip_unset_argument(self):
+    cfg = fdl.Config(fn_x_y, 3.14)
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 3.14}
+    self.assertEqual(output, expected)
+
+  def test_nested(self):
+    cfg = fdl.Config(fn_x_y, 'x', fdl.Config(fn_x_y, 'nest_x', 123))
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 'x', 'y.x': 'nest_x', 'y.y': 123}
+    self.assertEqual(output, expected)
+
+  def test_class(self):
+    cfg = fdl.Config(SampleClass, 'a_param', b=123)
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'a': 'a_param', 'b': 123}
+    self.assertEqual(output, expected)
+
+  def test_kwargs(self):
+    cfg = fdl.Config(fn_with_kwargs, 1, abc='extra kwarg value')
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 1, 'abc': 'extra kwarg value'}
+    self.assertEqual(output, expected)
+
+  def test_nested_kwargs(self):
+    cfg = fdl.Config(
+        fn_with_kwargs, extra=fdl.Config(fn_with_kwargs, 1, nested_extra='whee')
+    )
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'extra.x': 1, 'extra.nested_extra': 'whee'}
+    self.assertEqual(output, expected)
+
+  def test_nested_collections(self):
+    cfg = fdl.Config(
+        fn_x_y, [fdl.Config(fn_x_y, 1, '1'), fdl.Config(SampleClass, 2)]
+    )
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x[0].x': 1, 'x[0].y': '1', 'x[1].a': 2}
+    self.assertEqual(output, expected)
+
+  def test_multiple_nested_collections(self):
+    cfg = fdl.Config(
+        fn_x_y,
+        {'a': fdl.Config(fn_with_kwargs, abc=[1, 2, 3]), 'b': [3, 2, 1]},
+        [fdl.Config(fn_x_y, [fdl.Config(fn_x_y, 1, 2)])],
+    )
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {
+        "x['a'].abc": [1, 2, 3],
+        "x['b']": [3, 2, 1],
+        'y[0].x[0].x': 1,
+        'y[0].x[0].y': 2,
+    }
+    self.assertEqual(output, expected)
+
+  def test_skip_default_values(self):
+    def test_fn(w, x, y=3, z='abc'):  # pylint: disable=unused-argument
+      pass
+
+    cfg = fdl.Config(test_fn, 1)
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'w': 1}
+    self.assertEqual(output, expected)
+
+  def test_tagged_values(self):
+    cfg = fdl.Config(fn_x_y, x=SampleTag.new(), y=SampleTag.new(default='abc'))
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'y': 'abc'}
+    self.assertEqual(output, expected)
+
+    fdl.set_tagged(cfg, tag=SampleTag, value='cba')
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 'cba', 'y': 'cba'}
+    self.assertEqual(output, expected)
+
+  def test_partial(self):
+    partial = fdl.Partial(fn_x_y)
+    partial.x = 'abc'
+    output = printing.as_dict_flattened(partial)
+
+    expected = {'x': 'abc'}
+    self.assertEqual(output, expected)
+
+  def test_builtin_types_annotations(self):
+    cfg = fdl.Config(fn_with_type_annotations, 1)
+    cfg.y = 'abc'
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 1, 'y': 'abc'}
+    self.assertEqual(output, expected)
+
+  def test_annotated_kwargs(self):
+    cfg = fdl.Config(annotated_kwargs_helper, x=1, y='oops')
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 1, 'y': 'oops'}
+    self.assertEqual(output, expected)
+
+  def test_disabling_type_annotations(self):
+    cfg = fdl.Config(fn_with_type_annotations, 1)
+    cfg.y = 'abc'
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 1, 'y': 'abc'}
+    self.assertEqual(output, expected)
+
+  def test_union_type(self):
+    def to_integer(x: Union[int, str]):
+      return int(x)
+
+    cfg = fdl.Config(to_integer, 1)
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': 1}
+    self.assertEqual(output, expected)
+
+  def test_parameterized_generic(self):
+    if not (sys.version_info.major == 3 and sys.version_info.minor >= 9):
+      self.skipTest('types.GenericAlias is 3.9+ only.')
+
+    def takes_list(x: list[int]):
+      return x
+
+    cfg = fdl.Config(takes_list, [1, 2, 3])
+    output = printing.as_dict_flattened(cfg)
+
+    expected = {'x': [1, 2, 3]}
+    self.assertEqual(output, expected)
+
+  def test_materialized_default_values(self):
+    def test_fn(w, x, y=3, z='abc'):
+      del w, x, y, z  # Unused.
+
+    cfg = fdl.Config(test_fn, 1)
+    fdl.materialize_defaults(cfg)
+    output = printing.as_dict_flattened(cfg)
+    expected = {'w': 1, 'y': 3, 'z': 'abc'}
+    self.assertEqual(output, expected)
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.9/fiddle/_src/reraised_exception.py` & `fiddle-0.3.0/fiddle/_src/reraised_exception.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/reraised_exception_test.py` & `fiddle-0.3.0/fiddle/_src/reraised_exception_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/selectors.py` & `fiddle-0.3.0/fiddle/_src/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 def _memoized_walk_leaves_first(value, state=None):
   """Yields all values (memoized) from a configuration DAG."""
   state = state or daglish.MemoizedTraversal.begin(_memoized_walk_leaves_first,
                                                    value)
   if state.is_traversable(value):
-    for sub_result in state.flattened_map_children(value).values:
+    for sub_result in state.yield_map_child_values(value):
       yield from sub_result
   yield value
 
 
 @dataclasses.dataclass(frozen=True)
 class NodeSelection(Selection):
   """Represents a selection of nodes.
```

### Comparing `fiddle-0.2.9/fiddle/_src/selectors_test.py` & `fiddle-0.3.0/fiddle/_src/selectors_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/signatures_test_helper.py` & `fiddle-0.3.0/fiddle/_src/signatures_test_helper.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/tag_type.py` & `fiddle-0.3.0/fiddle/_src/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/tagging_test_module.py` & `fiddle-0.3.0/fiddle/_src/tagging_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/__init__.py` & `fiddle-0.3.0/fiddle/_src/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/autotest.py` & `fiddle-0.3.0/fiddle/_src/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/example/__init__.py` & `fiddle-0.3.0/fiddle/_src/testing/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/example/demo_configs.py` & `fiddle-0.3.0/fiddle/_src/testing/example/demo_configs.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/example/fake_encoder_decoder.py` & `fiddle-0.3.0/fiddle/_src/testing/example/fake_encoder_decoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,22 +49,22 @@
   dtype: Any
 
 
 # In real models there are multiple layers, but pretend there is just one for
 # this test.
 @dataclasses.dataclass
 class FakeEncoder:
-  embedders: Dict[str, Any]
+  embedders: Dict[str, TokenEmbedder]
   attention: Attention
   mlp: Mlp
 
 
 @dataclasses.dataclass
 class FakeDecoder:
-  embedders: Dict[str, Any]
+  embedders: Dict[str, TokenEmbedder]
   self_attention: Attention
   encoder_decoder_attention: CrossAttention
   mlp: Mlp
 
 
 @dataclasses.dataclass
 class FakeEncoderDecoder:
```

### Comparing `fiddle-0.2.9/fiddle/_src/testing/example/person_friend_toy.py` & `fiddle-0.3.0/fiddle/_src/testing/example/person_friend_toy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/nested_values.py` & `fiddle-0.3.0/fiddle/_src/testing/nested_values.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,22 @@
 
 import enum
 import random
 from typing import Any, List, Union
 
 from fiddle import daglish
 from fiddle._src import config
+from fiddle._src import partial
 from fiddle._src import tagging
 
 
+def args_only_fn(*args):
+  return args
+
+
 def kwargs_fn(**kwargs):
   return kwargs
 
 
 class SampleTag(tagging.Tag):
   """`fdl.Tag` that can be used for testing purposes."""
 
@@ -116,20 +121,24 @@
   def generate_dict(key_generator=None):
     length = rng.randint(0, max_container_size)
     key_generator = key_generator or rng.choice(
         [generate_int, generate_float, generate_string])
     return {key_generator(): generate_value() for _ in range(length)}
 
   def generate_buildable():
-    buildable_type = rng.choice([config.Config, config.Partial])
-    arguments = generate_dict(key_generator=generate_string)
-    buildable = buildable_type(kwargs_fn, **arguments)
-    if generate_bool() and arguments:
-      argument = rng.choice(list(arguments))
-      config.set_tags(buildable, argument, {SampleTag})
+    buildable_type = rng.choice([config.Config, partial.Partial])
+    if generate_bool():
+      arguments = generate_list()
+      return buildable_type(args_only_fn, *arguments)
+    else:
+      arguments = generate_dict(key_generator=generate_string)
+      buildable = buildable_type(kwargs_fn, **arguments)
+      if generate_bool() and arguments:
+        argument = rng.choice(list(arguments))
+        tagging.set_tags(buildable, argument, {SampleTag})
     return buildable
 
   def generate_alias():
     for value in enumerate(share_objects):
       if calculate_nested_value_depth(value) < max_depth:
         return value
     return generate_value()
```

### Comparing `fiddle-0.2.9/fiddle/_src/testing/nested_values_test.py` & `fiddle-0.3.0/fiddle/_src/testing/nested_values_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/test_util.py` & `fiddle-0.3.0/fiddle/_src/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/_src/testing/test_util_test.py` & `fiddle-0.3.0/fiddle/_src/testing/test_util_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/absl_flags/__init__.py` & `fiddle-0.3.0/fiddle/absl_flags/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,9 +14,12 @@
 # limitations under the License.
 
 """The public API for the absl_flags Fiddle extension."""
 
 from fiddle._src.absl_flags.flags import apply_fiddlers_to
 from fiddle._src.absl_flags.flags import apply_overrides_to
 from fiddle._src.absl_flags.flags import create_buildable_from_flags
+from fiddle._src.absl_flags.flags import DEFINE_fiddle_config
 from fiddle._src.absl_flags.flags import fdl_flags_supplied
+from fiddle._src.absl_flags.flags import FiddleFlag
+from fiddle._src.absl_flags.flags import FiddleFlagSerializer
 from fiddle._src.absl_flags.flags import flags_parser
```

### Comparing `fiddle-0.2.9/fiddle/absl_flags/example/__init__.py` & `fiddle-0.3.0/fiddle/absl_flags/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/absl_flags/example/business_logic.py` & `fiddle-0.3.0/fiddle/absl_flags/example/business_logic.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/absl_flags/example/configs.py` & `fiddle-0.3.0/fiddle/absl_flags/example/configs.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/absl_flags/example/example.py` & `fiddle-0.3.0/fiddle/absl_flags/example/example.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/absl_flags/example/tags.py` & `fiddle-0.3.0/fiddle/absl_flags/example/tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/arg_factory.py` & `fiddle-0.3.0/fiddle/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/building.py` & `fiddle-0.3.0/fiddle/building.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/codegen/__init__.py` & `fiddle-0.3.0/fiddle/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/codegen/auto_config/__init__.py` & `fiddle-0.3.0/fiddle/_src/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.3.0/fiddle/codegen/auto_config/experimental_top_level_api.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/codegen/codegen.py` & `fiddle-0.3.0/fiddle/codegen/codegen.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,13 +12,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Library for generating code from a Config or Partial object."""
 
 # pylint: disable=unused-import
+from fiddle._src.codegen.auto_config.experimental_top_level_api import auto_config_codegen
+from fiddle._src.codegen.auto_config.experimental_top_level_api import code_generator as auto_config_code_generator
+from fiddle._src.codegen.import_manager import register_import_alias
 from fiddle._src.codegen.legacy_codegen import assignment_path
 from fiddle._src.codegen.legacy_codegen import codegen_dot_syntax
 from fiddle._src.codegen.legacy_codegen import mini_ast
 from fiddle._src.codegen.legacy_codegen import SharedBuildableManager
 from fiddle._src.codegen.new_codegen import code_generator
 from fiddle._src.codegen.new_codegen import new_codegen
```

### Comparing `fiddle-0.2.9/fiddle/codegen/codegen_diff.py` & `fiddle-0.3.0/fiddle/extensions/jax.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,11 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Library for converting generating fiddlers from diffs."""
+"""Fiddle extensions to handle JAX code more elegantly.
+
+Currently this just affects codegen, graphviz, and other debugging functions.
+"""
 
 # pylint: disable=unused-import
-from fiddle._src.codegen.codegen_diff import fiddler_from_diff
+from fiddle._src.extensions.jax import enable
```

### Comparing `fiddle-0.2.9/fiddle/codegen/py_val_to_cst_converter.py` & `fiddle-0.3.0/fiddle/codegen/py_val_to_cst_converter.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/config.py` & `fiddle-0.3.0/fiddle/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Defines the `Config` class and associated subclasses and functions."""
 
 # pylint: disable=unused-import
 
-from fiddle._src.config import ArgFactory
 from fiddle._src.config import Buildable
 from fiddle._src.config import BuildableTraverserMetadata
 from fiddle._src.config import Config
 from fiddle._src.config import NO_VALUE
 from fiddle._src.config import NoValue
-from fiddle._src.config import Partial
+from fiddle._src.partial import ArgFactory
+from fiddle._src.partial import Partial
+from fiddle._src.signatures import VARARGS
```

### Comparing `fiddle-0.2.9/fiddle/config_test.py` & `fiddle-0.3.0/fiddle/config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/daglish.py` & `fiddle-0.3.0/fiddle/daglish.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 """Library for manipulating DAGs."""
 
 # pylint: disable=unused-import
 from fiddle._src.daglish import add_path_element
 from fiddle._src.daglish import Attr
+from fiddle._src.daglish import attr_or_index
 from fiddle._src.daglish import BasicTraversal
 from fiddle._src.daglish import BuildableAttr
 from fiddle._src.daglish import BuildableFnOrCls
 from fiddle._src.daglish import collect_paths_by_id
 from fiddle._src.daglish import find_node_traverser
 from fiddle._src.daglish import follow_path
 from fiddle._src.daglish import Index
```

### Comparing `fiddle-0.2.9/fiddle/diffing.py` & `fiddle-0.3.0/fiddle/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/examples/__init__.py` & `fiddle-0.3.0/fiddle/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/examples/colabs/__init__.py` & `fiddle-0.3.0/fiddle/examples/colabs/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/__init__.py` & `fiddle-0.3.0/fiddle/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/auto_config.py` & `fiddle-0.3.0/fiddle/experimental/auto_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/auto_config_policy.py` & `fiddle-0.3.0/fiddle/experimental/auto_config_policy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/autobuilders/__init__.py` & `fiddle-0.3.0/fiddle/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/configurator.py` & `fiddle-0.3.0/fiddle/experimental/namespace_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A midlevel API for creating configs, between core APIs and auto_config.
-
-This API is a Fiddle version of
-https://detectron2.readthedocs.io/en/latest/tutorials/lazyconfigs.html .
-
-WARNING: THIS API IS EXPERIMENTAL AND MAY BE DELETED. Please use auto_config
-right now for non-experimental projects, or fork this file.
-"""
+"""A Config that builds a `types.SimpleNamespace` from any argument."""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.configurator import configurator
+from fiddle._src.experimental.namespace_config import NamespaceConfig
```

### Comparing `fiddle-0.2.9/fiddle/experimental/dataclasses.py` & `fiddle-0.3.0/fiddle/experimental/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/dict_config.py` & `fiddle-0.3.0/fiddle/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/lazy_imports.py` & `fiddle-0.3.0/fiddle/experimental/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/namespace_config.py` & `fiddle-0.3.0/fiddle/extensions/tf.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,11 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A Config that builds a `types.SimpleNamespace` from any argument."""
+"""Fiddle extensions to handle TensorFlow code more elegantly.
+
+Currently this affects codegen, graphviz, serialization, and other
+debugging functions.
+"""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.namespace_config import NamespaceConfig
+from fiddle._src.extensions.tf import enable
```

### Comparing `fiddle-0.2.9/fiddle/experimental/serialization.py` & `fiddle-0.3.0/fiddle/experimental/serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/transform.py` & `fiddle-0.3.0/fiddle/experimental/transform.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/visualize.py` & `fiddle-0.3.0/fiddle/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/experimental/yaml_serialization.py` & `fiddle-0.3.0/fiddle/experimental/yaml_serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/extensions/__init__.py` & `fiddle-0.3.0/fiddle/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/extensions/jax.py` & `fiddle-0.3.0/fiddle/extensions/seqio.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle extensions to handle JAX code more elegantly.
+"""Fiddle extensions to handle SeqIO code more elegantly.
+
+(See https://github.com/google/seqio.)
 
 Currently this just affects codegen, graphviz, and other debugging functions.
 """
 
 # pylint: disable=unused-import
-from fiddle._src.extensions.jax import enable
+from fiddle._src.extensions.seqio import enable
```

### Comparing `fiddle-0.2.9/fiddle/extensions/seqio.py` & `fiddle-0.3.0/fiddle/extensions/numpy.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle extensions to handle SeqIO code more elegantly.
+"""Fiddle extensions to handle numpy code more elegantly.
 
-(See https://github.com/google/seqio.)
-
-Currently this just affects codegen, graphviz, and other debugging functions.
+Currently this affects codegen, graphviz, and other debugging functions.
 """
 
 # pylint: disable=unused-import
-from fiddle._src.extensions.seqio import enable
+from fiddle._src.extensions.numpy import enable
```

### Comparing `fiddle-0.2.9/fiddle/extensions/tf.py` & `fiddle-0.3.0/fiddle/testing/test_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle extensions to handle TensorFlow code more elegantly.
-
-Currently this affects codegen, graphviz, serialization, and other
-debugging functions.
-"""
+"""Utility functions for tests that use fiddle.experimental.daglish."""
 
 # pylint: disable=unused-import
-from fiddle._src.extensions.tf import enable
+from fiddle._src.testing.test_util import TestCase
```

### Comparing `fiddle-0.2.9/fiddle/graphviz.py` & `fiddle-0.3.0/fiddle/graphviz.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/history.py` & `fiddle-0.3.0/fiddle/history.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/printing.py` & `fiddle-0.3.0/fiddle/printing.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Functions to output representations of `fdl.Buildable`s."""
 
 # pylint: disable=unused-import
+from fiddle._src.printing import as_dict_flattened
 from fiddle._src.printing import as_str_flattened
 from fiddle._src.printing import history_per_leaf_parameter
```

### Comparing `fiddle-0.2.9/fiddle/selectors.py` & `fiddle-0.3.0/fiddle/selectors.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/signatures.py` & `fiddle-0.3.0/fiddle/signatures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/tag_type.py` & `fiddle-0.3.0/fiddle/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/tagging.py` & `fiddle-0.3.0/fiddle/tagging.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/testing/__init__.py` & `fiddle-0.3.0/fiddle/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/testing/autotest.py` & `fiddle-0.3.0/fiddle/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.9/fiddle/testing/test_util.py` & `fiddle-0.3.0/fiddle/_src/validation/fake_experiment.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,11 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Utility functions for tests that use fiddle.experimental.daglish."""
+"""Fake experiment overrides for the encoder-decoder."""
 
-# pylint: disable=unused-import
-from fiddle._src.testing.test_util import TestCase
+from fiddle._src.testing.example import fake_encoder_decoder
+
+
+def fake_experiment():
+  config = fake_encoder_decoder.fixture.as_buildable()
+  config.encoder.attention.dtype = "float64"
+  return config
```

### Comparing `fiddle-0.2.9/fiddle/version.py` & `fiddle-0.3.0/fiddle/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Current Fiddle version at head on Github."""
-__version__ = "0.2.9"
+"""Current Fiddle version at head on GitHub."""
+__version__ = "0.3.0"
```

### Comparing `fiddle-0.2.9/fiddle.egg-info/PKG-INFO` & `fiddle-0.3.0/fiddle.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.9
+Version: 0.3.0
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
@@ -14,20 +14,22 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: flags
 Provides-Extra: testing
 License-File: LICENSE
 
 
 # Fiddle
```

### Comparing `fiddle-0.2.9/fiddle.egg-info/SOURCES.txt` & `fiddle-0.3.0/fiddle.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,31 @@
 fiddle/graphviz.py
 fiddle/history.py
 fiddle/printing.py
 fiddle/selectors.py
 fiddle/signatures.py
 fiddle/tag_type.py
 fiddle/tagging.py
+fiddle/validation.py
 fiddle/version.py
 fiddle.egg-info/PKG-INFO
 fiddle.egg-info/SOURCES.txt
 fiddle.egg-info/dependency_links.txt
 fiddle.egg-info/requires.txt
 fiddle.egg-info/top_level.txt
 fiddle/_src/__init__.py
 fiddle/_src/arg_factory.py
 fiddle/_src/arg_factory_test.py
 fiddle/_src/building.py
 fiddle/_src/building_test.py
+fiddle/_src/casting.py
 fiddle/_src/config.py
 fiddle/_src/config_test.py
+fiddle/_src/copying.py
+fiddle/_src/copying_test.py
 fiddle/_src/daglish.py
 fiddle/_src/daglish_extensions.py
 fiddle/_src/daglish_extensions_test.py
 fiddle/_src/daglish_test.py
 fiddle/_src/diffing.py
 fiddle/_src/diffing_test.py
 fiddle/_src/graphviz.py
@@ -41,31 +45,35 @@
 fiddle/_src/materialize.py
 fiddle/_src/materialize_test.py
 fiddle/_src/module_reflection.py
 fiddle/_src/module_reflection_test.py
 fiddle/_src/module_reflection_test_module.py
 fiddle/_src/mutate_buildable.py
 fiddle/_src/mutate_buildable_test.py
+fiddle/_src/partial.py
+fiddle/_src/partial_test.py
 fiddle/_src/printing.py
 fiddle/_src/printing_test.py
 fiddle/_src/reraised_exception.py
 fiddle/_src/reraised_exception_test.py
 fiddle/_src/selectors.py
 fiddle/_src/selectors_test.py
 fiddle/_src/signatures.py
 fiddle/_src/signatures_test.py
 fiddle/_src/signatures_test_helper.py
+fiddle/_src/special_overrides.py
 fiddle/_src/tag_type.py
 fiddle/_src/tagging.py
 fiddle/_src/tagging_test.py
 fiddle/_src/tagging_test_module.py
 fiddle/_src/absl_flags/__init__.py
 fiddle/_src/absl_flags/flags.py
 fiddle/_src/absl_flags/legacy_flags.py
 fiddle/_src/absl_flags/sample_module_for_flags_test.py
+fiddle/_src/absl_flags/sample_test_binary.py
 fiddle/_src/absl_flags/utils.py
 fiddle/_src/codegen/__init__.py
 fiddle/_src/codegen/codegen_diff.py
 fiddle/_src/codegen/formatting_utilities.py
 fiddle/_src/codegen/import_manager.py
 fiddle/_src/codegen/import_manager_test.py
 fiddle/_src/codegen/legacy_codegen.py
@@ -78,22 +86,25 @@
 fiddle/_src/codegen/newcg_symbolic_references.py
 fiddle/_src/codegen/newcg_symbolic_references_test.py
 fiddle/_src/codegen/py_val_to_cst_converter.py
 fiddle/_src/codegen/py_val_to_cst_converter_test.py
 fiddle/_src/codegen/special_value_codegen.py
 fiddle/_src/codegen/test_util.py
 fiddle/_src/codegen/auto_config/__init__.py
+fiddle/_src/codegen/auto_config/add_type_signatures.py
+fiddle/_src/codegen/auto_config/add_type_signatures_test.py
 fiddle/_src/codegen/auto_config/code_ir.py
 fiddle/_src/codegen/auto_config/code_ir_test.py
 fiddle/_src/codegen/auto_config/complex_to_variables.py
 fiddle/_src/codegen/auto_config/complex_to_variables_test.py
 fiddle/_src/codegen/auto_config/experimental_top_level_api.py
 fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
 fiddle/_src/codegen/auto_config/get_history_comments.py
 fiddle/_src/codegen/auto_config/get_history_comments_test.py
+fiddle/_src/codegen/auto_config/import_manager_wrapper.py
 fiddle/_src/codegen/auto_config/init_task.py
 fiddle/_src/codegen/auto_config/init_task_test.py
 fiddle/_src/codegen/auto_config/ir_printer.py
 fiddle/_src/codegen/auto_config/ir_printer_test.py
 fiddle/_src/codegen/auto_config/ir_to_cst.py
 fiddle/_src/codegen/auto_config/ir_to_cst_test.py
 fiddle/_src/codegen/auto_config/make_symbolic_references.py
@@ -111,15 +122,14 @@
 fiddle/_src/codegen/auto_config/test_fixtures.py
 fiddle/_src/codegen/test_submodule/__init__.py
 fiddle/_src/codegen/test_submodule/test_util.py
 fiddle/_src/experimental/__init__.py
 fiddle/_src/experimental/auto_config.py
 fiddle/_src/experimental/auto_config_policy.py
 fiddle/_src/experimental/auto_config_test.py
-fiddle/_src/experimental/configurator.py
 fiddle/_src/experimental/daglish_legacy.py
 fiddle/_src/experimental/daglish_legacy_test.py
 fiddle/_src/experimental/dataclasses.py
 fiddle/_src/experimental/dataclasses_test.py
 fiddle/_src/experimental/dict_config.py
 fiddle/_src/experimental/dict_config_test.py
 fiddle/_src/experimental/lazy_imports.py
@@ -138,28 +148,38 @@
 fiddle/_src/experimental/autobuilders/__init__.py
 fiddle/_src/experimental/autobuilders/autobuilders.py
 fiddle/_src/experimental/autobuilders/autobuilders_test.py
 fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
 fiddle/_src/extensions/__init__.py
 fiddle/_src/extensions/flax_test.py
 fiddle/_src/extensions/jax.py
+fiddle/_src/extensions/numpy.py
+fiddle/_src/extensions/numpy_test.py
 fiddle/_src/extensions/seqio.py
 fiddle/_src/extensions/seqio_test.py
 fiddle/_src/extensions/tf.py
 fiddle/_src/extensions/tf_test.py
 fiddle/_src/testing/__init__.py
 fiddle/_src/testing/autotest.py
 fiddle/_src/testing/nested_values.py
 fiddle/_src/testing/nested_values_test.py
 fiddle/_src/testing/test_util.py
 fiddle/_src/testing/test_util_test.py
 fiddle/_src/testing/example/__init__.py
 fiddle/_src/testing/example/demo_configs.py
 fiddle/_src/testing/example/fake_encoder_decoder.py
 fiddle/_src/testing/example/person_friend_toy.py
+fiddle/_src/validation/__init__.py
+fiddle/_src/validation/baseline_style.py
+fiddle/_src/validation/baseline_style_test.py
+fiddle/_src/validation/check_types.py
+fiddle/_src/validation/check_types_test.py
+fiddle/_src/validation/fake_experiment.py
+fiddle/_src/validation/no_custom_objects.py
+fiddle/_src/validation/no_custom_objects_test.py
 fiddle/absl_flags/__init__.py
 fiddle/absl_flags/example/__init__.py
 fiddle/absl_flags/example/business_logic.py
 fiddle/absl_flags/example/configs.py
 fiddle/absl_flags/example/example.py
 fiddle/absl_flags/example/tags.py
 fiddle/codegen/__init__.py
@@ -169,24 +189,24 @@
 fiddle/codegen/auto_config/__init__.py
 fiddle/codegen/auto_config/experimental_top_level_api.py
 fiddle/examples/__init__.py
 fiddle/examples/colabs/__init__.py
 fiddle/experimental/__init__.py
 fiddle/experimental/auto_config.py
 fiddle/experimental/auto_config_policy.py
-fiddle/experimental/configurator.py
 fiddle/experimental/dataclasses.py
 fiddle/experimental/dict_config.py
 fiddle/experimental/lazy_imports.py
 fiddle/experimental/namespace_config.py
 fiddle/experimental/serialization.py
 fiddle/experimental/transform.py
 fiddle/experimental/visualize.py
 fiddle/experimental/yaml_serialization.py
 fiddle/experimental/autobuilders/__init__.py
 fiddle/extensions/__init__.py
 fiddle/extensions/jax.py
+fiddle/extensions/numpy.py
 fiddle/extensions/seqio.py
 fiddle/extensions/tf.py
 fiddle/testing/__init__.py
 fiddle/testing/autotest.py
 fiddle/testing/test_util.py
```

### Comparing `fiddle-0.2.9/setup.py` & `fiddle-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 # pylint: disable=g-long-ternary
 setup(
     name='fiddle',
     version=__version__,
     include_package_data=True,
     packages=find_packages(exclude=['docs']),  # Required
     package_data={'testdata': ['testdata/*.fiddle']},
+    python_requires='>=3.8',
     install_requires=[
         'absl-py',
         'graphviz',
         'libcst',
         'typing-extensions',
     ],
     extras_require={
@@ -62,15 +63,20 @@
         'testing': [
             'cloudpickle',
             'fiddle[flags]',
             'flax',
             'graphviz',
             'pytest',
             'pytype',
-        ] + ['seqio-nightly'] if sys.platform != 'darwin' else []
+        ] + [
+            'seqio',
+            # Temporarily pin the TFDS version to avoid pip backtracking during
+            # unit tests.
+            'tfds_nightly>=4.9.2.dev202308090034',
+        ] if sys.platform != 'darwin' else []
     },
     description='Fiddle: A Python-first configuration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/google/fiddle',
     author='The Fiddle Team',
     author_email='noreply@google.com',
@@ -86,14 +92,15 @@
         'License :: OSI Approved :: Apache Software License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
 
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

