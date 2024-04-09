# Comparing `tmp/bioimageio.spec-0.5.1.tar.gz` & `tmp/bioimageio.spec-0.5.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.spec-0.5.1.tar", last modified: Thu Mar 21 16:17:05 2024, max compression
+gzip compressed data, was "bioimageio.spec-0.5.1.post1.tar", last modified: Tue Apr  9 09:13:43 2024, max compression
```

## Comparing `bioimageio.spec-0.5.1.tar` & `bioimageio.spec-0.5.1.post1.tar`

### file list

```diff
@@ -1,138 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.525102 bioimageio.spec-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-03-21 16:17:05.525102 bioimageio.spec-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17946 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.505102 bioimageio.spec-0.5.1/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.513102 bioimageio.spec-0.5.1/bioimageio/spec/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_build_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.513102 bioimageio.spec-0.5.1/bioimageio/spec/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/_generated_spdx_license_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/common_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/field_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/field_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/io_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/packaging_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/root_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/validator_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_internal/warning_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.513102 bioimageio.spec-0.5.1/bioimageio/spec/application/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/application/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/application/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/collection/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/collection/v0_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/dataset/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/dataset/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/generic/_v0_2_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/generic/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15276 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/generic/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/generic/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/model/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/model/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/model/_v0_4_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    40031 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/model/v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    94166 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/model/v0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/notebook/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/notebook/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/partner_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/partner_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.517102 bioimageio.spec-0.5.1/bioimageio/spec/partner_utils/imjoy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/partner_utils/imjoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/pretty_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/bioimageio/spec/static/
--rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/static/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/bioimageio/spec/static/tag_categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/bioimageio/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.509102 bioimageio.spec-0.5.1/bioimageio.spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18769 2024-03-21 16:17:05.000000 bioimageio.spec-0.5.1/bioimageio.spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-03-21 16:17:05.000000 bioimageio.spec-0.5.1/bioimageio.spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 16:17:05.000000 bioimageio.spec-0.5.1/bioimageio.spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-21 16:17:05.000000 bioimageio.spec-0.5.1/bioimageio.spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-21 16:17:05.000000 bioimageio.spec-0.5.1/bioimageio.spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.505102 bioimageio.spec-0.5.1/example_descriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.505102 bioimageio.spec-0.5.1/example_descriptions/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/example_descriptions/collections/unet2d_nuclei_broad_coll/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-21 16:14:40.000000 bioimageio.spec-0.5.1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.509102 bioimageio.spec-0.5.1/example_descriptions/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_diff_output_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_fixed_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_fixed_shape/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_multi_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_nuclei_broad/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/example_descriptions/models/upsample_test_model/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/example_descriptions/models/upsample_test_model/upsample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/compare_yaml_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/generate_dtype_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17786 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/generate_spec_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/generate_version_submodule_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/report_invalid_rdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/scripts/update_spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 16:17:05.525102 bioimageio.spec-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_bioimageio_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_example_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.521102 bioimageio.spec-0.5.1/tests/test_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_generic/test_v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_generic/test_v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.525102 bioimageio.spec-0.5.1/tests/test_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/test_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_internal/test_file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_internal/test_license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_internal/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_internal/test_validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_internal/test_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:17:05.525102 bioimageio.spec-0.5.1/tests/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_model/test_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_model/test_v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-21 16:14:41.000000 bioimageio.spec-0.5.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-21 16:17:00.000000 bioimageio.spec-0.5.1/tests/test_specific_reexports_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18775 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17946 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.689105 bioimageio.spec-0.5.1.post1/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.697106 bioimageio.spec-0.5.1.post1/bioimageio/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_build_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_generated_spdx_license_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/common_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20406 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/packaging_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/root_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validator_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/warning_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11106 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12553 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.701105 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_4_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40287 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99793 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/pretty_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/bioimageio/spec/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/static/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/static/tag_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/bioimageio/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18775 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 09:13:43.000000 bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/example_descriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/example_descriptions/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.693106 bioimageio.spec-0.5.1.post1/example_descriptions/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_diff_output_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_fixed_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-04-09 09:10:58.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_fixed_shape/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_multi_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/example_descriptions/models/upsample_test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/example_descriptions/models/upsample_test_model/upsample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.705105 bioimageio.spec-0.5.1.post1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/compare_yaml_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_dtype_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_spec_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/generate_version_submodule_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/report_invalid_rdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/scripts/update_spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-09 09:13:41.000000 bioimageio.spec-0.5.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_bioimageio_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_example_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/test_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_internal/test_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:13:43.709106 bioimageio.spec-0.5.1.post1/tests/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-09 09:10:59.000000 bioimageio.spec-0.5.1.post1/tests/test_specific_reexports_generics.py
```

### Comparing `bioimageio.spec-0.5.1/LICENSE` & `bioimageio.spec-0.5.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/PKG-INFO` & `bioimageio.spec-0.5.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.1
+Version: 0.5.1.post1
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
```

### Comparing `bioimageio.spec-0.5.1/README.md` & `bioimageio.spec-0.5.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_build_description.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_build_description.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, Callable, Mapping, Optional, Type, TypeVar, Union
+from typing import Any, Callable, List, Mapping, Optional, Type, TypeVar, Union
 
 from ._internal.common_nodes import InvalidDescr, ResourceDescrBase
 from ._internal.io import BioimageioYamlContent
 from ._internal.types import FormatVersionPlaceholder
 from ._internal.validation_context import ValidationContext, validation_context_var
-from .generic import GenericDescr
+from .summary import ErrorEntry, ValidationDetail
 
 ResourceDescrT = TypeVar("ResourceDescrT", bound=ResourceDescrBase)
 
 
 DISCOVER: FormatVersionPlaceholder = "discover"
 """placeholder for whatever format version an RDF specifies"""
 
@@ -46,24 +46,56 @@
     /,
     *,
     context: Optional[ValidationContext] = None,
     format_version: Union[FormatVersionPlaceholder, str] = DISCOVER,
     get_rd_class: Callable[[Any, Any], Type[ResourceDescrT]],
 ) -> Union[ResourceDescrT, InvalidDescr]:
     context = context or validation_context_var.get()
-    if not isinstance(content, dict):
-        # "Invalid content of type '{type(content)}'"
-        rd_class = GenericDescr
-
-    typ = content.get("type")
-    rd_class = get_rd_class(typ, content.get("format_version"))
+    errors: List[ErrorEntry] = []
+    if isinstance(content, dict):
+        for minimum in ("type", "format_version"):
+            if minimum not in content:
+                errors.append(
+                    ErrorEntry(
+                        loc=(minimum,), msg=f"Missing field '{minimum}'", type="error"
+                    )
+                )
+            elif not isinstance(content[minimum], str):
+                errors.append(
+                    ErrorEntry(
+                        loc=(minimum,),
+                        msg=f"Invalid type '{type(content[minimum])}'",
+                        type="error",
+                    )
+                )
+    else:
+        errors.append(
+            ErrorEntry(
+                loc=(), msg=f"Invalid content of type '{type(content)}'", type="error"
+            )
+        )
+        content = {}
+
+    if errors:
+        ret = InvalidDescr(**content)  # pyright: ignore[reportArgumentType]
+        ret.validation_summary.add_detail(
+            ValidationDetail(
+                name="extract fields to chose description class",
+                status="failed",
+                errors=errors,
+            )
+        )
+        return ret
 
+    typ = content["type"]
+    rd_class = get_rd_class(typ, content["format_version"])
     rd = rd_class.load(content, context=context)
-    assert rd.validation_summary is not None
+
     if format_version != DISCOVER and not isinstance(rd, InvalidDescr):
+        # load with requested format_version
         discover_details = rd.validation_summary.details
         as_rd_class = get_rd_class(typ, format_version)
         rd = as_rd_class.load(content, context=context)
         assert rd.validation_summary is not None
         rd.validation_summary.details[:0] = discover_details
 
     return rd
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_description.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/_generated_spdx_license_literals.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_generated_spdx_license_literals.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/_settings.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/_settings.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/common_nodes.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/common_nodes.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/constants.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/docs_utils.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/docs_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/field_validation.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_validation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/field_warning.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/field_warning.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,13 +135,15 @@
 #   and use a loguru handler to format warnings accordingly
 def issue_warning(
     msg: LiteralString,
     *,
     value: Any,
     severity: WarningSeverity = WARNING,
     msg_context: Optional[Dict[str, Any]] = None,
+    field: Optional[str] = None,
 ):
     msg_context = {"value": value, "severity": severity, **(msg_context or {})}
     if severity >= validation_context_var.get().warning_level:
         raise PydanticCustomError("warning", msg, msg_context)
     elif validation_context_var.get().log_warnings:
-        logger.log(severity, msg.format(**msg_context))
+        log_msg = (field + ": " if field else "") + (msg.format(**msg_context))
+        logger.log(severity, log_msg)
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/io.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from zipfile import ZipFile, is_zipfile
 
 import pooch
 import pydantic
 from pydantic import (
     AnyUrl,
     DirectoryPath,
+    Field,
     FilePath,
     GetCoreSchemaHandler,
     PlainSerializer,
     PrivateAttr,
     RootModel,
     SerializationInfo,
     StringConstraints,
@@ -107,14 +108,17 @@
         """the absolute path/url (resolved at time of initialization with the root of the ValidationContext)"""
         return self._absolute
 
     def model_post_init(self, __context: Any) -> None:
         if self.root.is_absolute():
             raise ValueError(f"{self.root} is an absolute path.")
 
+        if self.root.parts and self.root.parts[0] in ("http:", "https:"):
+            raise ValueError(f"{self.root} looks like an http url.")
+
         self._absolute = (  # pyright: ignore[reportAttributeAccessIssue]
             self.get_absolute(validation_context_var.get().root)
         )
         super().model_post_init(__context)
 
     # @property
     # def __members(self):
@@ -191,14 +195,20 @@
         ):
             raise ValueError(f"{absolute} does not exist")
 
         return absolute
 
 
 class RelativeFilePath(RelativePathBase[Union[AbsoluteFilePath, HttpUrl]], frozen=True):
+    def model_post_init(self, __context: Any) -> None:
+        if not self.root.parts:  # an empty path can only be a directory
+            raise ValueError(f"{self.root} is not a valid file path.")
+
+        super().model_post_init(__context)
+
     def get_absolute(
         self, root: "RootHttpUrl | Path | AnyUrl"
     ) -> "AbsoluteFilePath | HttpUrl":
         absolute = self._get_absolute_impl(root)
         if (
             isinstance(absolute, Path)
             and validation_context_var.get().perform_io_checks
@@ -222,15 +232,18 @@
             and not absolute.is_dir()
         ):
             raise ValueError(f"{absolute} does not point to an existing directory")
 
         return absolute
 
 
-FileSource = Union[FilePath, RelativeFilePath, HttpUrl, pydantic.HttpUrl]
+FileSource = Annotated[
+    Union[FilePath, RelativeFilePath, HttpUrl, pydantic.HttpUrl],
+    Field(union_mode="left_to_right"),
+]
 PermissiveFileSource = Union[FileSource, str]
 
 V_suffix = TypeVar("V_suffix", bound=FileSource)
 path_or_url_adapter = TypeAdapter(Union[FilePath, DirectoryPath, HttpUrl])
 
 
 def validate_suffix(
@@ -499,26 +512,28 @@
     original_file_name: FileName
 
 
 class HashKwargs(TypedDict):
     sha256: NotRequired[Optional[Sha256]]
 
 
-StrictFileSource = Union[HttpUrl, FilePath, RelativeFilePath]
+StrictFileSource = Annotated[
+    Union[HttpUrl, FilePath, RelativeFilePath], Field(union_mode="left_to_right")
+]
 _strict_file_source_adapter = TypeAdapter(StrictFileSource)
 
 
 def interprete_file_source(file_source: PermissiveFileSource) -> StrictFileSource:
+    if isinstance(file_source, (HttpUrl, Path)):
+        return file_source
+
     if isinstance(file_source, pydantic.AnyUrl):
         file_source = str(file_source)
 
-    if isinstance(file_source, str):
-        return _strict_file_source_adapter.validate_python(file_source)
-    else:
-        return file_source
+    return _strict_file_source_adapter.validate_python(file_source)
 
 
 def _get_known_hash(hash_kwargs: HashKwargs):
     if "sha256" in hash_kwargs and hash_kwargs["sha256"] is not None:
         return f"sha256:{hash_kwargs['sha256']}"
     else:
         return None
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/io_utils.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/io_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/license_id.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/node.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/packaging_context.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/packaging_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/root_url.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/root_url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/types.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/url.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/url.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,25 +12,31 @@
 
 
 def _validate_url(url: Union[str, pydantic.HttpUrl]) -> pydantic.AnyUrl:
     url = str(url)
     if not validation_context_var.get().perform_io_checks:
         return pydantic.AnyUrl(url)
 
+    val_url = url
+
     if url.startswith("https://colab.research.google.com/github/"):
-        # head request for colab returns "Value error, 405: Method Not Allowed"
-        # therefore we check if the source notebook exists at github instead
+        # get requests for colab returns 200 even if the source notebook does not exists.
+        # We therefore validate the url to the notebbok instead (for github notebooks)
         val_url = url.replace(
             "https://colab.research.google.com/github/", "https://github.com/"
         )
-    else:
-        val_url = url
+    elif url.startswith("https://colab.research.google.com/"):
+        # TODO: improve validation of non-github colab urls
+        issue_warning(
+            "colab urls currently pass even if the notebook url was not found. Cannot fully validate {value}",
+            value=url,
+        )
 
     try:
-        response = requests.head(val_url, timeout=(3, 3))
+        response = requests.get(val_url, timeout=(3, 3))
     except (
         requests.exceptions.ChunkedEncodingError,
         requests.exceptions.ContentDecodingError,
         requests.exceptions.InvalidHeader,
         requests.exceptions.InvalidJSONError,
         requests.exceptions.InvalidSchema,
         requests.exceptions.InvalidURL,
@@ -52,54 +58,38 @@
     except Exception as e:
         issue_warning(
             "Failed to validate URL '{value}': {error}",
             value=url,
             msg_context={"error": str(e)},
         )
     else:
-        follow_up_with_get = False
         if response.status_code == 302:  # found
             pass
         elif response.status_code in (301, 303, 308):
             issue_warning(
                 "URL redirected ({status_code}): consider updating {value} with new"
                 + " location: {location}",
                 value=url,
                 msg_context={
                     "status_code": response.status_code,
                     "location": response.headers.get("location"),
                 },
             )
-        elif response.status_code == 403:  # forbidden
-            follow_up_with_get = True
-            issue_warning(
-                "{status_code}: {reason} {value}",
-                value=url,
-                msg_context={
-                    "status_code": response.status_code,
-                    "reason": response.reason,
-                },
-            )
         elif response.status_code == 405:
             issue_warning(
                 "{status_code}: {reason} {value}",
                 value=url,
                 msg_context={
                     "status_code": response.status_code,
                     "reason": response.reason,
                 },
             )
         elif response.status_code != 200:
             raise ValueError(f"{response.status_code}: {response.reason} {url}")
 
-        if follow_up_with_get:
-            pass
-            # TODO follow up forbidden head request with get
-            # motivating example: 403: Forbidden https://elifesciences.org/articles/57613
-
     return pydantic.AnyUrl(url)
 
 
 class HttpUrl(RootHttpUrl):
     root_model: ClassVar[Type[RootModel[Any]]] = RootModel[
         Annotated[pydantic.HttpUrl, AfterValidator(_validate_url)]
     ]
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/utils.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/validated_string.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/validation_context.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validation_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/validator_annotations.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/validator_annotations.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/version_type.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/version_type.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_internal/warning_levels.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_internal/warning_levels.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_io.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/_package.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     ensure_is_valid_bioimageio_yaml_name,
 )
 from ._internal.io_basics import BIOIMAGEIO_YAML, AbsoluteFilePath, FileName
 from ._internal.io_utils import open_bioimageio_yaml, write_yaml, write_zip
 from ._internal.packaging_context import PackagingContext
 from ._internal.url import HttpUrl
 from ._internal.validation_context import validation_context_var
+from ._internal.warning_levels import ERROR
 from ._io import load_description
 from .model.v0_4 import ModelDescr as ModelDescr04
 from .model.v0_4 import WeightsFormat
 from .model.v0_5 import ModelDescr as ModelDescr05
 
 
 def get_os_friendly_file_name(name: str) -> str:
@@ -249,19 +250,20 @@
 
     write_zip(
         output_path,
         package_content,
         compression=compression,
         compression_level=compression_level,
     )
-    if isinstance((exported := load_description(output_path)), InvalidDescr):
-        raise ValueError(
-            f"Exported package '{output_path}' is invalid:"
-            + f" {exported.validation_summary}"
-        )
+    with validation_context_var.get().replace(warning_level=ERROR):
+        if isinstance((exported := load_description(output_path)), InvalidDescr):
+            raise ValueError(
+                f"Exported package '{output_path}' is invalid:"
+                + f" {exported.validation_summary}"
+            )
 
     return output_path
 
 
 def save_bioimageio_package_to_stream(
     source: Union[BioimageioYamlSource, ResourceDescr],
     /,
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/application/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/application/v0_2.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/application/v0_3.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/application/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/collection/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/collection/v0_2.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,17 +173,18 @@
             # set entry specific root as it might be adapted in the presence of an external entry source
             entry_root = context.root
             entry_file_name = context.file_name
 
             if entry.rdf_source is not None:
                 if not context.perform_io_checks:
                     issue_warning(
-                        "Skipping IO relying validation for collection[{i}]",
+                        "Skipping IO dependent validation (perform_io_checks=False)",
                         value=entry.rdf_source,
                         msg_context=dict(i=i),
+                        field=f"collection[{i}]",
                     )
                     continue
 
                 external_data = open_bioimageio_yaml(entry.rdf_source)
                 # add/overwrite common collection entry content with external source
                 entry_data.update(external_data.content)
                 entry_root = external_data.original_root
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/collection/v0_3.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/collection/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/dataset/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/dataset/v0_2.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/dataset/v0_3.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/dataset/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/generic/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/generic/_v0_2_converter.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/_v0_2_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/generic/v0_2.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_2.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,19 +77,22 @@
 
 VALID_COVER_IMAGE_EXTENSIONS = (
     ".gif",
     ".jpeg",
     ".jpg",
     ".png",
     ".svg",
+    ".tif",
+    ".tiff",
 )
 
 _WithImageSuffix = WithSuffix(VALID_COVER_IMAGE_EXTENSIONS, case_sensitive=False)
 CoverImageSource = Annotated[
-    Union[HttpUrl, AbsoluteFilePath, RelativeFilePath],
+    Union[AbsoluteFilePath, RelativeFilePath, HttpUrl],
+    Field(union_mode="left_to_right"),
     _WithImageSuffix,
     include_in_package_serializer,
 ]
 
 
 class AttachmentsDescr(Node):
     model_config = {**Node.model_config, "extra": "allow"}
@@ -230,29 +233,29 @@
     @classmethod
     def accept_author_strings(cls, authors: Union[Any, Sequence[Any]]) -> Any:
         """we unofficially accept strings as author entries"""
         if isinstance(authors, collections.abc.Sequence):
             authors = [{"name": a} if isinstance(a, str) else a for a in authors]
 
         if not authors:
-            issue_warning("No author specified.", value=authors)
+            issue_warning("missing", value=authors, field="authors")
 
         return authors
 
     attachments: Optional[AttachmentsDescr] = None
     """file and other attachments"""
 
     cite: List[CiteEntry] = Field(default_factory=list)
     """citations"""
 
     @field_validator("cite", mode="after")
     @classmethod
     def _warn_empty_cite(cls, value: Any):
         if not value:
-            issue_warning("No cite entry specified.", value=value)
+            issue_warning("missing", value=value, field="cite")
 
         return value
 
     config: Annotated[
         Dict[str, YamlValue],
         Field(
             examples=[
@@ -392,36 +395,42 @@
         ),
     ] = None
     """∈📦 URL or relative path to a markdown file with additional documentation.
     The recommended documentation file name is `README.md`. An `.md` suffix is mandatory."""
 
     license: Annotated[
         Union[LicenseId, DeprecatedLicenseId, str, None],
-        Field(
-            union_mode="left_to_right", examples=["CC0-1.0", "MIT", "BSD-2-Clause"]
-        ),
+        Field(union_mode="left_to_right", examples=["CC0-1.0", "MIT", "BSD-2-Clause"]),
     ] = None
     """A [SPDX license identifier](https://spdx.org/licenses/).
     We do not support custom license beyond the SPDX license list, if you need that please
     [open a GitHub issue](https://github.com/bioimage-io/spec-bioimage-io/issues/new/choose
     ) to discuss your intentions with the community."""
 
     @field_validator("license", mode="after")
     @classmethod
     def deprecated_spdx_license(
         cls, value: Optional[Union[LicenseId, DeprecatedLicenseId, str]]
     ):
         if isinstance(value, LicenseId):
             pass
         elif value is None:
-            issue_warning("missing license.", value=value)
+            issue_warning("missing", value=value, field="license")
         elif isinstance(value, DeprecatedLicenseId):
-            issue_warning("'{value}' is a deprecated license identifier.", value=value)
+            issue_warning(
+                "'{value}' is a deprecated license identifier.",
+                value=value,
+                field="license",
+            )
         elif isinstance(value, str):
-            issue_warning("'{value}' is an unknown license identifier.", value=value)
+            issue_warning(
+                "'{value}' is an unknown license identifier.",
+                value=value,
+                field="license",
+            )
         else:
             assert_never(value)
 
         return value
 
 
 ResourceDescrType = TypeVar("ResourceDescrType", bound=GenericDescrBase)
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/generic/v0_3.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/generic/v0_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,29 +53,36 @@
     AfterValidator,
     Predicate,
     RestrictCharacters,
 )
 from .._internal.version_type import Version as Version
 from .._internal.warning_levels import ALERT, INFO
 from ._v0_3_converter import convert_from_older_format
-from .v0_2 import VALID_COVER_IMAGE_EXTENSIONS, CoverImageSource
 from .v0_2 import Author as _Author_v0_2
 from .v0_2 import BadgeDescr as BadgeDescr
+from .v0_2 import CoverImageSource
 from .v0_2 import Doi as Doi
 from .v0_2 import Maintainer as _Maintainer_v0_2
 from .v0_2 import OrcidId as OrcidId
 from .v0_2 import Uploader as Uploader
 
 KNOWN_SPECIFIC_RESOURCE_TYPES = (
     "application",
     "collection",
     "dataset",
     "model",
     "notebook",
 )
+VALID_COVER_IMAGE_EXTENSIONS = (
+    ".gif",
+    ".jpeg",
+    ".jpg",
+    ".png",
+    ".svg",
+)
 
 
 class ResourceId(ValidatedString):
     root_model: ClassVar[Type[RootModel[Any]]] = RootModel[
         Annotated[
             NotEmpty[str],
             RestrictCharacters(string.ascii_lowercase + string.digits + "_-/."),
@@ -88,14 +95,15 @@
 
 def _validate_md_suffix(value: V_suffix) -> V_suffix:
     return validate_suffix(value, suffix=".md", case_sensitive=True)
 
 
 DocumentationSource = Annotated[
     Union[AbsoluteFilePath, RelativeFilePath, HttpUrl],
+    Field(union_mode="left_to_right"),
     AfterValidator(_validate_md_suffix),
     include_in_package_serializer,
 ]
 
 
 def _has_no_slash(s: str) -> bool:
     return "/" not in s and "\\" not in s
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/model/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/model/_v0_3_converter.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/model/_v0_4_converter.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/_v0_4_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/model/v0_4.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_4.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,28 +127,31 @@
         *mods, callname = valid_string_data.split(".")
         return dict(module_name=".".join(mods), callable_name=callname)
 
 
 class CallableFromFile(StringNode):
     _pattern = r"^.+:.+$"
     source_file: Annotated[
-        Union[HttpUrl, RelativeFilePath],
+        Union[RelativeFilePath, HttpUrl],
+        Field(union_mode="left_to_right"),
         include_in_package_serializer,
     ]
     """∈📦 Python module that implements `callable_name`"""
     callable_name: Identifier
     """The Python identifier of  """
 
     @classmethod
     def _get_data(cls, valid_string_data: str):
         *file_parts, callname = valid_string_data.split(":")
         return dict(source_file=":".join(file_parts), callable_name=callname)
 
 
-CustomCallable = Union[CallableFromFile, CallableFromDepencency]
+CustomCallable = Annotated[
+    Union[CallableFromFile, CallableFromDepencency], Field(union_mode="left_to_right")
+]
 
 
 class Dependencies(StringNode):
     _pattern = r"^.+:.+$"
     manager: Annotated[NotEmpty[str], Field(examples=["conda", "maven", "pip"])]
     """Dependency manager"""
 
@@ -264,18 +267,19 @@
     """TensorFlow version used to create these weights"""
 
     @field_validator("tensorflow_version", mode="after")
     @classmethod
     def _tfv(cls, value: Any):
         if value is None:
             issue_warning(
-                "Missing TensorFlow version. Please specify the TensorFlow version"
+                "missing. Please specify the TensorFlow version"
                 + " these weights were created with.",
                 value=value,
                 severity=ALERT,
+                field="tensorflow_version",
             )
         return value
 
 
 class OnnxWeightsDescr(WeightsEntryDescrBase):
     type = "onnx"
     weights_format_name: ClassVar[str] = "ONNX"
@@ -288,14 +292,15 @@
         if value is None:
             issue_warning(
                 "Missing ONNX opset version (aka ONNX opset number). "
                 + "Please specify the ONNX opset version these weights were created"
                 + " with.",
                 value=value,
                 severity=ALERT,
+                field="opset_version",
             )
         return value
 
 
 class PytorchStateDictWeightsDescr(WeightsEntryDescrBase):
     type = "pytorch_state_dict"
     weights_format_name: ClassVar[str] = "Pytorch State Dict"
@@ -344,18 +349,19 @@
     (`dependencies` overrules `pytorch_version`)"""
 
     @field_validator("pytorch_version", mode="after")
     @classmethod
     def _ptv(cls, value: Any):
         if value is None:
             issue_warning(
-                "Missing PyTorch version. Please specify the PyTorch version these"
+                "missing. Please specify the PyTorch version these"
                 + " PyTorch state dict weights were created with.",
                 value=value,
                 severity=ALERT,
+                field="pytorch_version",
             )
         return value
 
 
 class TorchscriptWeightsDescr(WeightsEntryDescrBase):
     type = "torchscript"
     weights_format_name: ClassVar[str] = "TorchScript"
@@ -363,18 +369,19 @@
     """Version of the PyTorch library used."""
 
     @field_validator("pytorch_version", mode="after")
     @classmethod
     def _ptv(cls, value: Any):
         if value is None:
             issue_warning(
-                "Missing PyTorch version. Please specify the PyTorch version these"
+                "missing. Please specify the PyTorch version these"
                 + " Torchscript weights were created with.",
                 value=value,
                 severity=ALERT,
+                field="pytorch_version",
             )
         return value
 
 
 class TensorflowJsWeightsDescr(WeightsEntryDescrBase):
     type = "tensorflow_js"
     weights_format_name: ClassVar[str] = "Tensorflow.js"
@@ -382,18 +389,19 @@
     """Version of the TensorFlow library used."""
 
     @field_validator("tensorflow_version", mode="after")
     @classmethod
     def _tfv(cls, value: Any):
         if value is None:
             issue_warning(
-                "Missing TensorFlow version. Please specify the TensorFlow version"
+                "missing. Please specify the TensorFlow version"
                 + " these TensorflowJs weights were created with.",
                 value=value,
                 severity=ALERT,
+                field="tensorflow_version",
             )
         return value
 
     source: ImportantFileSource
     """∈📦 The multi-file weights.
     All required files/folders should be a zip archive."""
 
@@ -405,18 +413,19 @@
     """Version of the TensorFlow library used."""
 
     @field_validator("tensorflow_version", mode="after")
     @classmethod
     def _tfv(cls, value: Any):
         if value is None:
             issue_warning(
-                "Missing TensorFlow version. Please specify the TensorFlow version"
+                "missing. Please specify the TensorFlow version"
                 + " these Tensorflow saved model bundle weights were created with.",
                 value=value,
                 severity=ALERT,
+                field="tensorflow_version",
             )
         return value
 
 
 class ParameterizedInputShape(Node):
     """A sequence of valid shapes given by `shape_k = min + k * step for k in {0, 1, ...}`."""
 
@@ -440,15 +449,15 @@
 class ImplicitOutputShape(Node):
     """Output tensor shape depending on an input tensor shape.
     `shape(output_tensor) = shape(input_tensor) * scale + 2 * offset`"""
 
     reference_tensor: TensorName
     """Name of the reference tensor."""
 
-    scale: NotEmpty[List[Union[float, None]]]
+    scale: NotEmpty[List[Optional[float]]]
     """output_pix/input_pix for each dimension.
     'null' values indicate new dimensions, whose length is defined by 2*`offset`"""
 
     offset: NotEmpty[List[Union[int, Annotated[float, MultipleOf(0.5)]]]]
     """Position of origin wrt to input."""
 
     def __len__(self) -> int:
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/model/v0_5.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/model/v0_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import string
 import warnings
 from abc import ABC
 from copy import deepcopy
 from datetime import datetime
 from itertools import chain
+from math import ceil
 from pathlib import Path, PurePosixPath
 from tempfile import mkdtemp
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
@@ -33,16 +34,18 @@
 
 import imageio
 import numpy as np
 from annotated_types import Ge, Gt, Interval, MaxLen, MinLen, Predicate
 from imageio.v3 import imread  # pyright: ignore[reportUnknownVariableType]
 from numpy.typing import NDArray
 from pydantic import (
+    Discriminator,
     Field,
     RootModel,
+    Tag,
     ValidationInfo,
     field_validator,
     model_validator,
 )
 from typing_extensions import Annotated, LiteralString, Self, assert_never
 
 from .._internal.common_nodes import (
@@ -238,14 +241,18 @@
             )
 
         return size
 
     def get_size(self, n: ParameterizedSize.N) -> int:
         return self.min + self.step * n
 
+    def get_n(self, s: int) -> ParameterizedSize.N:
+        """return smallest n parameterizing a size greater or equal than `s`"""
+        return ceil((s - self.min) / self.step)
+
 
 ARBITRARY_SIZE = ParameterizedSize(min=1, step=1)
 
 
 class DataDependentSize(Node):
     min: Annotated[int, Gt(0)] = 1
     max: Annotated[Optional[int], Gt(1)] = None
@@ -309,24 +316,28 @@
         axis: Union[
             ChannelAxis,
             IndexInputAxis,
             IndexOutputAxis,
             TimeInputAxis,
             SpaceInputAxis,
             TimeOutputAxis,
+            TimeOutputAxisWithHalo,
             SpaceOutputAxis,
+            SpaceOutputAxisWithHalo,
         ],
         ref_axis: Union[
             ChannelAxis,
             IndexInputAxis,
             IndexOutputAxis,
             TimeInputAxis,
             SpaceInputAxis,
             TimeOutputAxis,
+            TimeOutputAxisWithHalo,
             SpaceOutputAxis,
+            SpaceOutputAxisWithHalo,
         ],
         n: ParameterizedSize.N,
     ):
         """helper method to compute concrete size for a given axis and its reference axis.
         If the reference axis is parameterized, `n` is used to compute the concrete size of it, see `ParameterizedSize`.
         """
         assert (
@@ -365,15 +376,17 @@
         axis: Union[
             ChannelAxis,
             IndexInputAxis,
             IndexOutputAxis,
             TimeInputAxis,
             SpaceInputAxis,
             TimeOutputAxis,
+            TimeOutputAxisWithHalo,
             SpaceOutputAxis,
+            SpaceOutputAxisWithHalo,
         ],
     ):
         return axis.unit
 
 
 # this Axis definition is compatible with the NGFF draft from July 10, 2023
 # https://ngff.openmicroscopy.org/latest/#axes-md
@@ -383,23 +396,39 @@
     id: AxisId
     """An axis id unique across all axes of one tensor."""
 
     description: Annotated[str, MaxLen(128)] = ""
 
 
 class WithHalo(Node):
-    halo: Annotated[int, Ge(0)] = 0
+    halo: Annotated[int, Ge(1)]
     """The halo should be cropped from the output tensor to avoid boundary effects.
     It is to be cropped from both sides, i.e. `size_after_crop = size - 2 * halo`.
     To document a halo that is already cropped by the model use `size.offset` instead."""
 
+    size: Annotated[
+        SizeReference,
+        Field(
+            examples=[
+                10,
+                SizeReference(
+                    tensor_id=TensorId("t"), axis_id=AxisId("a"), offset=5
+                ).model_dump(mode="json"),
+            ]
+        ),
+    ]
+    """reference to another axis with an optional offset (see `SizeReference`)"""
+
+
+BATCH_AXIS_ID = AxisId("batch")
+
 
 class BatchAxis(AxisBase):
     type: Literal["batch"] = "batch"
-    id: Annotated[AxisId, Predicate(lambda x: x == AxisId("batch"))] = AxisId("batch")
+    id: Annotated[AxisId, Predicate(lambda x: x == BATCH_AXIS_ID)] = BATCH_AXIS_ID
     size: Optional[Literal[1]] = None
     """The batch size may be fixed to 1,
     otherwise (the default) it may be chosen arbitrarily depending on available memory"""
 
     @property
     def scale(self):
         return 1.0
@@ -456,32 +485,14 @@
     """The size/length of this axis can be specified as
     - fixed integer
     - parameterized series of valid sizes (`ParameterizedSize`)
     - reference to another axis with an optional offset (`SizeReference`)
     """
 
 
-class _WithOutputAxisSize(Node):
-    size: Annotated[
-        Union[Annotated[int, Gt(0)], SizeReference],
-        Field(
-            examples=[
-                10,
-                SizeReference(
-                    tensor_id=TensorId("t"), axis_id=AxisId("a"), offset=5
-                ).model_dump(mode="json"),
-            ]
-        ),
-    ]
-    """The size/length of this axis can be specified as
-    - fixed integer
-    - reference to another axis with an optional offset (`SizeReference`)
-    """
-
-
 class IndexInputAxis(IndexAxisBase, _WithInputAxisSize):
     pass
 
 
 class IndexOutputAxis(IndexAxisBase):
     size: Annotated[
         Union[Annotated[int, Gt(0)], SizeReference, DataDependentSize],
@@ -525,24 +536,75 @@
 
 _InputAxisUnion = Union[
     BatchAxis, ChannelAxis, IndexInputAxis, TimeInputAxis, SpaceInputAxis
 ]
 InputAxis = Annotated[_InputAxisUnion, Field(discriminator="type")]
 
 
-class TimeOutputAxis(TimeAxisBase, WithHalo, _WithOutputAxisSize):
+class _WithOutputAxisSize(Node):
+    size: Annotated[
+        Union[Annotated[int, Gt(0)], SizeReference],
+        Field(
+            examples=[
+                10,
+                SizeReference(
+                    tensor_id=TensorId("t"), axis_id=AxisId("a"), offset=5
+                ).model_dump(mode="json"),
+            ]
+        ),
+    ]
+    """The size/length of this axis can be specified as
+    - fixed integer
+    - reference to another axis with an optional offset (see `SizeReference`)
+    """
+
+
+class TimeOutputAxis(TimeAxisBase, _WithOutputAxisSize):
     pass
 
 
-class SpaceOutputAxis(SpaceAxisBase, WithHalo, _WithOutputAxisSize):
+class TimeOutputAxisWithHalo(TimeAxisBase, WithHalo):
     pass
 
 
+def _get_halo_axis_discriminator_value(v: Any) -> Literal["with_halo", "wo_halo"]:
+    if isinstance(v, dict):
+        return "with_halo" if "halo" in v else "wo_halo"
+    else:
+        return "with_halo" if hasattr(v, "halo") else "wo_halo"
+
+
+_TimeOutputAxisUnion = Annotated[
+    Union[
+        Annotated[TimeOutputAxis, Tag("wo_halo")],
+        Annotated[TimeOutputAxisWithHalo, Tag("with_halo")],
+    ],
+    Discriminator(_get_halo_axis_discriminator_value),
+]
+
+
+class SpaceOutputAxis(SpaceAxisBase, _WithOutputAxisSize):
+    pass
+
+
+class SpaceOutputAxisWithHalo(SpaceAxisBase, WithHalo):
+    pass
+
+
+_SpaceOutputAxisUnion = Annotated[
+    Union[
+        Annotated[SpaceOutputAxis, Tag("wo_halo")],
+        Annotated[SpaceOutputAxisWithHalo, Tag("with_halo")],
+    ],
+    Discriminator(_get_halo_axis_discriminator_value),
+]
+
+
 _OutputAxisUnion = Union[
-    BatchAxis, ChannelAxis, IndexOutputAxis, TimeOutputAxis, SpaceOutputAxis
+    BatchAxis, ChannelAxis, IndexOutputAxis, _TimeOutputAxisUnion, _SpaceOutputAxisUnion
 ]
 OutputAxis = Annotated[_OutputAxisUnion, Field(discriminator="type")]
 
 AnyAxis = Union[InputAxis, OutputAxis]
 
 TVs = Union[
     NotEmpty[List[int]],
@@ -1238,32 +1300,39 @@
                     offset_from_scale = 0
                 size = SizeReference(
                     tensor_id=TensorId(t_id),
                     axis_id=AxisId(a_id),
                     offset=int(offset_from_scale + 2 * shape.offset[i]),
                 )
         elif isinstance(shape, collections.abc.Sequence):
-            size: Any = shape[i]
+            size = shape[i]
             assert isinstance(size, int)
         else:
             assert_never(shape)
 
         if axis_type == "time":
             if tensor_type == "input":
                 ret.append(TimeInputAxis(size=size, scale=scale))
             else:
-                ret.append(
-                    TimeOutputAxis(
-                        size=size, scale=scale, halo=0 if halo is None else halo[i]
+                assert not isinstance(size, ParameterizedSize)
+                if halo is None:
+                    ret.append(TimeOutputAxis(size=size, scale=scale))
+                else:
+                    assert not isinstance(size, int)
+                    ret.append(
+                        TimeOutputAxisWithHalo(size=size, scale=scale, halo=halo[i])
                     )
-                )
+
         elif axis_type == "index":
             if tensor_type == "input":
                 ret.append(IndexInputAxis(size=size))
             else:
+                if isinstance(size, ParameterizedSize):
+                    size = DataDependentSize(min=size.min)
+
                 ret.append(IndexOutputAxis(size=size))
         elif axis_type == "channel":
             assert not isinstance(size, ParameterizedSize)
             if isinstance(size, SizeReference):
                 warnings.warn(
                     "Conversion of channel size from an implicit output shape may by"
                     + " wrong"
@@ -1281,15 +1350,24 @@
                         channel_names=[Identifier(f"channel{i}") for i in range(size)]
                     )
                 )
         elif axis_type == "space":
             if tensor_type == "input":
                 ret.append(SpaceInputAxis(id=AxisId(a), size=size, scale=scale))
             else:
-                ret.append(SpaceOutputAxis(id=AxisId(a), size=size, scale=scale))
+                assert not isinstance(size, ParameterizedSize)
+                if halo is None:
+                    ret.append(SpaceOutputAxis(id=AxisId(a), size=size, scale=scale))
+                else:
+                    assert not isinstance(size, int)
+                    ret.append(
+                        SpaceOutputAxisWithHalo(
+                            id=AxisId(a), size=size, scale=scale, halo=halo[i]
+                        )
+                    )
 
     return ret
 
 
 _AXIS_TYPE_MAP = {
     "b": "batch",
     "t": "time",
@@ -1654,15 +1732,18 @@
 
 
 class ArchitectureFromLibraryDescr(_ArchitectureCallableDescr):
     import_from: str
     """Where to import the callable from, i.e. `from <import_from> import <callable>`"""
 
 
-ArchitectureDescr = Union[ArchitectureFromFileDescr, ArchitectureFromLibraryDescr]
+ArchitectureDescr = Annotated[
+    Union[ArchitectureFromFileDescr, ArchitectureFromLibraryDescr],
+    Field(union_mode="left_to_right"),
+]
 
 
 class _ArchFileConv(
     Converter[
         _CallableFromFile_v0_4,
         ArchitectureFromFileDescr,
         Optional[Sha256],
@@ -1838,14 +1919,15 @@
             issue_warning(
                 "Exactly one weights entry may not specify the `parent` field (got"
                 + " {value}).That entry is considered the original set of model weights."
                 + " Other weight formats are created through conversion of the orignal or"
                 + " already converted weights. They have to reference the weights format"
                 + " they were converted from as their `parent`.",
                 value=len(entries_wo_parent),
+                field="weights",
             )
 
         for wtype, entry in self:
             if entry is None:
                 continue
 
             assert hasattr(entry, "type")
@@ -1878,18 +1960,27 @@
 
 class _DataDepSize(NamedTuple):
     min: int
     max: Optional[int]
 
 
 class _AxisSizes(NamedTuple):
+    """the lenghts of all axes of model inputs and outputs"""
+
     inputs: Dict[Tuple[TensorId, AxisId], int]
     outputs: Dict[Tuple[TensorId, AxisId], Union[int, _DataDepSize]]
 
 
+class _TensorSizes(NamedTuple):
+    """_AxisSizes as nested dicts"""
+
+    inputs: Dict[TensorId, Dict[AxisId, int]]
+    outputs: Dict[TensorId, Dict[AxisId, Union[int, _DataDepSize]]]
+
+
 class ModelDescr(GenericModelDescrBase, title="bioimage.io model specification"):
     """Specification of the fields used in a bioimage.io-compliant RDF to describe AI models with pretrained weights.
     These fields are typically stored in a YAML file which we call a model resource description file (model RDF).
     """
 
     format_version: Literal["0.5.0"] = "0.5.0"
     """Version of the bioimage.io model description specification used.
@@ -1926,15 +2017,17 @@
         if not validation_context_var.get().perform_io_checks:
             return value
 
         doc_path = download(value).path
         doc_content = doc_path.read_text()
         if not re.match("#.*[vV]alidation", doc_content):
             issue_warning(
-                "No '# Validation' (sub)section found in {value}.", value=value
+                "No '# Validation' (sub)section found in {value}.",
+                value=value,
+                field="documentation",
             )
 
         return value
 
     inputs: NotEmpty[Sequence[InputTensorDescr]]
     """Describes the input tensors expected by this model."""
 
@@ -1977,73 +2070,80 @@
         a: int,
         axis: AnyAxis,
         valid_independent_refs: Dict[
             Tuple[TensorId, AxisId],
             Tuple[TensorDescr, AnyAxis, Union[int, ParameterizedSize]],
         ],
     ):
-        if isinstance(axis, BatchAxis) or isinstance(axis.size, int):
+        if isinstance(axis, BatchAxis) or isinstance(
+            axis.size, (int, ParameterizedSize, DataDependentSize)
+        ):
             return
+        elif not isinstance(axis.size, SizeReference):
+            assert_never(axis.size)
 
-        if isinstance(axis.size, (ParameterizedSize, DataDependentSize)):
-            if isinstance(axis, WithHalo) and (axis.size.min - 2 * axis.halo) < 1:
-                raise ValueError(
-                    f"axis {axis.id} with minimum size {axis.size.min} is too small for"
-                    + f" halo {axis.halo}."
-                )
-
-        elif isinstance(axis.size, SizeReference):
-            ref = (axis.size.tensor_id, axis.size.axis_id)
-            if ref not in valid_independent_refs:
-                raise ValueError(
-                    "Invalid tensor axis reference at"
-                    + f" {field_name}[{i}].axes[{a}].size: {axis.size}."
-                )
-            if ref == (tensor_id, axis.id):
+        # validate axis.size SizeReference
+        ref = (axis.size.tensor_id, axis.size.axis_id)
+        if ref not in valid_independent_refs:
+            raise ValueError(
+                "Invalid tensor axis reference at"
+                + f" {field_name}[{i}].axes[{a}].size: {axis.size}."
+            )
+        if ref == (tensor_id, axis.id):
+            raise ValueError(
+                "Self-referencing not allowed for"
+                + f" {field_name}[{i}].axes[{a}].size: {axis.size}"
+            )
+        if axis.type == "channel":
+            if valid_independent_refs[ref][1].type != "channel":
                 raise ValueError(
-                    "Self-referencing not allowed for"
-                    + f" {field_name}[{i}].axes[{a}].size: {axis.size}"
+                    "A channel axis' size may only reference another fixed size"
+                    + " channel axis."
                 )
-            if axis.type == "channel":
-                if valid_independent_refs[ref][1].type != "channel":
-                    raise ValueError(
-                        "A channel axis' size may only reference another fixed size"
-                        + " channel axis."
-                    )
-                if isinstance(axis.channel_names, str) and "{i}" in axis.channel_names:
-                    ref_size = valid_independent_refs[ref][2]
-                    assert isinstance(ref_size, int), (
-                        "channel axis ref (another channel axis) has to specify fixed"
-                        + " size"
-                    )
-                    generated_channel_names = [
-                        Identifier(axis.channel_names.format(i=i))
-                        for i in range(1, ref_size + 1)
-                    ]
-                    axis.channel_names = generated_channel_names
-
-            if (ax_unit := getattr(axis, "unit", None)) != (
-                ref_unit := getattr(valid_independent_refs[ref][1], "unit", None)
-            ):
-                raise ValueError(
-                    "The units of an axis and its reference axis need to match, but"
-                    + f" '{ax_unit}' != '{ref_unit}'."
+            if isinstance(axis.channel_names, str) and "{i}" in axis.channel_names:
+                ref_size = valid_independent_refs[ref][2]
+                assert isinstance(ref_size, int), (
+                    "channel axis ref (another channel axis) has to specify fixed"
+                    + " size"
                 )
-            min_size = valid_independent_refs[ref][2]
-            if isinstance(min_size, ParameterizedSize):
-                min_size = min_size.min
+                generated_channel_names = [
+                    Identifier(axis.channel_names.format(i=i))
+                    for i in range(1, ref_size + 1)
+                ]
+                axis.channel_names = generated_channel_names
+
+        if (ax_unit := getattr(axis, "unit", None)) != (
+            ref_unit := getattr(valid_independent_refs[ref][1], "unit", None)
+        ):
+            raise ValueError(
+                "The units of an axis and its reference axis need to match, but"
+                + f" '{ax_unit}' != '{ref_unit}'."
+            )
+        ref_axis = valid_independent_refs[ref][1]
+        if isinstance(ref_axis, BatchAxis):
+            raise ValueError(
+                f"Invalid reference axis '{ref_axis.id}' for {tensor_id}.{axis.id}"
+                + " (a batch axis is not allowed as reference)."
+            )
 
-            if isinstance(axis, WithHalo) and (min_size - 2 * axis.halo) < 1:
+        if isinstance(axis, WithHalo):
+            min_size = axis.size.get_size(axis, ref_axis, n=0)
+            if (min_size - 2 * axis.halo) < 1:
                 raise ValueError(
                     f"axis {axis.id} with minimum size {min_size} is too small for halo"
                     + f" {axis.halo}."
                 )
 
-        else:
-            assert_never(axis.size)
+            input_halo = axis.halo * axis.scale / ref_axis.scale
+            if input_halo != int(input_halo) or input_halo % 2 == 1:
+                raise ValueError(
+                    f"input_halo {input_halo} (output_halo {axis.halo} *"
+                    + f" output_scale {axis.scale} / input_scale {ref_axis.scale})"
+                    + f" is not an even integer for {tensor_id}.{axis.id}."
+                )
 
     @model_validator(mode="after")
     def _validate_test_tensors(self) -> Self:
         if not validation_context_var.get().perform_io_checks:
             return self
 
         test_arrays = [
@@ -2210,15 +2310,15 @@
     No standard run modes are defined yet."""
 
     timestamp: Datetime = Datetime(datetime.now())
     """Timestamp in [ISO 8601](#https://en.wikipedia.org/wiki/ISO_8601) format
     with a few restrictions listed [here](https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat).
     (In Python a datetime object is valid, too)."""
 
-    training_data: Union[LinkedDataset, DatasetDescr, None] = None
+    training_data: Union[None, LinkedDataset, DatasetDescr] = None
     """The dataset used to train this model"""
 
     weights: WeightsDescr
     """The weights for this model.
     Weights can be given for different formats, but should otherwise be equivalent.
     The available weight formats determine which consumers can use this model."""
 
@@ -2233,14 +2333,15 @@
                 [(t, load_array(t.test_tensor.download().path)) for t in self.outputs],
             )
         except Exception as e:
             issue_warning(
                 "Failed to generate cover image(s): {e}",
                 value=self.covers,
                 msg_context=dict(e=e),
+                field="covers",
             )
         else:
             self.covers.extend(generated_covers)
 
         return self
 
     def get_input_test_arrays(self) -> List[NDArray[Any]]:
@@ -2249,72 +2350,148 @@
         return data
 
     def get_output_test_arrays(self) -> List[NDArray[Any]]:
         data = [load_array(out.test_tensor.download().path) for out in self.outputs]
         assert all(isinstance(d, np.ndarray) for d in data)
         return data
 
+    @staticmethod
+    def get_batch_size(tensor_sizes: Mapping[TensorId, Mapping[AxisId, int]]) -> int:
+        batch_size = 1
+        tensor_with_batchsize: Optional[TensorId] = None
+        for tid in tensor_sizes:
+            for aid, s in tensor_sizes[tid].items():
+                if aid != BATCH_AXIS_ID or s == 1 or s == batch_size:
+                    continue
+
+                if batch_size != 1:
+                    assert tensor_with_batchsize is not None
+                    raise ValueError(
+                        f"batch size mismatch for tensors '{tensor_with_batchsize}' ({batch_size}) and '{tid}' ({s})"
+                    )
+
+                batch_size = s
+                tensor_with_batchsize = tid
+
+        return batch_size
+
+    def get_output_tensor_sizes(
+        self, input_sizes: Mapping[TensorId, Mapping[AxisId, int]]
+    ) -> Dict[TensorId, Dict[AxisId, Union[int, _DataDepSize]]]:
+        batch_size = self.get_batch_size(input_sizes)
+        ns = self.get_ns(input_sizes)
+
+        tensor_sizes = self.get_tensor_sizes(ns, batch_size=batch_size)
+        assert tensor_sizes.inputs == {k: dict(v) for k, v in input_sizes.items()}
+        return tensor_sizes.outputs
+
+    def get_ns(self, input_sizes: Mapping[TensorId, Mapping[AxisId, int]]):
+        ret: Dict[Tuple[TensorId, AxisId], ParameterizedSize.N] = {}
+        axes = {t.id: {a.id: a for a in t.axes} for t in self.inputs}
+        for tid in input_sizes:
+            for aid, s in input_sizes[tid].items():
+                size_descr = axes[tid][aid].size
+                if size_descr is None or isinstance(size_descr, (int, SizeReference)):
+                    pass
+                elif isinstance(size_descr, ParameterizedSize):
+                    ret[(tid, aid)] = size_descr.get_n(s)
+                else:
+                    assert_never(size_descr)
+
+        return ret
+
+    def get_tensor_sizes(
+        self, ns: Mapping[Tuple[TensorId, AxisId], ParameterizedSize.N], batch_size: int
+    ) -> _TensorSizes:
+        axis_sizes = self.get_axis_sizes(ns, batch_size=batch_size)
+        return _TensorSizes(
+            {
+                t: {
+                    aa: axis_sizes.inputs[(tt, aa)]
+                    for tt, aa in axis_sizes.inputs
+                    if tt == t
+                }
+                for t in {tt for tt, _ in axis_sizes.inputs}
+            },
+            {
+                t: {
+                    aa: axis_sizes.outputs[(tt, aa)]
+                    for tt, aa in axis_sizes.outputs
+                    if tt == t
+                }
+                for t in {tt for tt, _ in axis_sizes.outputs}
+            },
+        )
+
     def get_axis_sizes(
-        self, ns: Dict[Tuple[TensorId, AxisId], ParameterizedSize.N], batch_size: int
+        self, ns: Mapping[Tuple[TensorId, AxisId], ParameterizedSize.N], batch_size: int
     ) -> _AxisSizes:
         all_axes = {
             t.id: {a.id: a for a in t.axes} for t in chain(self.inputs, self.outputs)
         }
 
         inputs: Dict[Tuple[TensorId, AxisId], int] = {}
         outputs: Dict[Tuple[TensorId, AxisId], Union[int, _DataDepSize]] = {}
-        input_ids = {d.id for d in self.inputs}
-        output_ids = {d.id for d in self.outputs}
-        for t_descr in chain(self.inputs, self.outputs):
-            for a in t_descr.axes:
-                if isinstance(a, BatchAxis):
-                    if (t_descr.id, a.id) in ns:
-                        raise ValueError(
-                            f"No size increment factor (n) for batch axis of tensor {t_descr.id} expected."
-                        )
-                    s = batch_size
-                elif isinstance(a.size, int):
-                    if (t_descr.id, a.id) in ns:
-                        raise ValueError(
-                            f"No size increment factor (n) for fixed size axis {a.id} of tensor {t_descr.id} expected."
-                        )
-                    s = a.size
-                elif isinstance(a.size, ParameterizedSize):
-                    if (t_descr.id, a.id) not in ns:
-                        raise ValueError(
-                            f"Size increment factor (n) not given for parametrized axis {a.id} of tensor {t_descr.id}."
-                        )
-                    s = a.size.get_size(ns[(t_descr.id, a.id)])
-                elif isinstance(a.size, SizeReference):
-                    assert not isinstance(a, BatchAxis)
-                    ref_axis = all_axes[a.size.tensor_id][a.size.axis_id]
-                    assert not isinstance(ref_axis, BatchAxis)
-                    if (a.size.tensor_id, a.size.axis_id) not in ns:
-                        raise ValueError(
-                            f"No increment (n) provided for axis {a.id} of tensor {t_descr.id}. Expected reference from tensor {a.size.tensor_id} and axis {a.size.axis_id}."
-                        )
-                    s = a.size.get_size(
-                        axis=a, ref_axis=ref_axis, n=ns[(t_descr.id, a.id)]
+
+        def get_axis_size(a: Union[InputAxis, OutputAxis]):
+            if isinstance(a, BatchAxis):
+                if (t_descr.id, a.id) in ns:
+                    raise ValueError(
+                        "No size increment factor (n) for batch axis of tensor"
+                        + f" '{t_descr.id}' expected."
                     )
-                elif isinstance(a.size, DataDependentSize):
-                    if (t_descr.id, a.id) in ns:
-                        raise ValueError(
-                            f"No size increment factor (n) for data dependent size axis {a.id} of tensor {t_descr.id} expected."
-                        )
-                    assert t_descr.id in output_ids
-                    outputs[t_descr.id, a.id] = _DataDepSize(a.size.min, a.size.max)
-                    continue
-                else:
-                    assert_never(a.size)
+                return batch_size
+            elif isinstance(a.size, int):
+                if (t_descr.id, a.id) in ns:
+                    raise ValueError(
+                        "No size increment factor (n) for fixed size axis"
+                        + f" '{a.id}' of tensor '{t_descr.id}' expected."
+                    )
+                return a.size
+            elif isinstance(a.size, ParameterizedSize):
+                if (t_descr.id, a.id) not in ns:
+                    raise ValueError(
+                        "Size increment factor (n) missing for parametrized axis"
+                        + f" '{a.id}' of tensor '{t_descr.id}'."
+                    )
+                return a.size.get_size(ns[(t_descr.id, a.id)])
+            elif isinstance(a.size, SizeReference):
+                if (t_descr.id, a.id) in ns:
+                    raise ValueError(
+                        f"No size increment factor (n) for axis '{a.id}' of tensor"
+                        + f" '{t_descr.id}' with size reference expected."
+                    )
+                assert not isinstance(a, BatchAxis)
+                ref_axis = all_axes[a.size.tensor_id][a.size.axis_id]
+                assert not isinstance(ref_axis, BatchAxis)
+                return a.size.get_size(
+                    axis=a,
+                    ref_axis=ref_axis,
+                    n=ns.get((a.size.tensor_id, a.size.axis_id), 0),
+                )
+            elif isinstance(a.size, DataDependentSize):
+                if (t_descr.id, a.id) in ns:
+                    raise ValueError(
+                        "No size increment factor (n) for data dependent size axis"
+                        + f" '{a.id}' of tensor '{t_descr.id}' expected."
+                    )
+                return _DataDepSize(a.size.min, a.size.max)
+            else:
+                assert_never(a.size)
 
-                if t_descr.id in input_ids:
-                    inputs[t_descr.id, a.id] = s
-                else:
-                    assert t_descr.id in output_ids
-                    outputs[t_descr.id, a.id] = s
+        for t_descr in self.inputs:
+            for a in t_descr.axes:
+                s = get_axis_size(a)
+                assert not isinstance(s, _DataDepSize)
+                inputs[t_descr.id, a.id] = s
+
+        for t_descr in chain(self.inputs, self.outputs):
+            for a in t_descr.axes:
+                s = get_axis_size(a)
+                outputs[t_descr.id, a.id] = s
 
         return _AxisSizes(inputs=inputs, outputs=outputs)
 
     @model_validator(mode="before")
     @classmethod
     def _convert(cls, data: Dict[str, Any]) -> Dict[str, Any]:
         if (
```

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/notebook/__init__.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/notebook/v0_2.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/notebook/v0_3.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/notebook/v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/pretty_validation_errors.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/pretty_validation_errors.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/static/spdx_licenses.json` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/static/spdx_licenses.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/static/tag_categories.json` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/static/tag_categories.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/bioimageio/spec/summary.py` & `bioimageio.spec-0.5.1.post1/bioimageio/spec/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from itertools import chain
 from pathlib import Path
 from types import MappingProxyType
 from typing import Any, Iterable, List, Literal, Mapping, Tuple, Union, no_type_check
 
+import rich.console
+import rich.markdown
 from pydantic import BaseModel, Field, model_validator
 from pydantic_core.core_schema import ErrorType
 from typing_extensions import TypedDict, assert_never
 
 from ._internal.constants import VERSION
 from ._internal.warning_levels import (
     ALERT,
@@ -275,20 +277,23 @@
     @no_type_check
     def display(self) -> None:
         formatted = self.format()
         try:
             from IPython.core.getipython import get_ipython
             from IPython.display import Markdown, display
         except ImportError:
-            print(formatted)
+            pass
         else:
-            if get_ipython() is None:
-                print(formatted)
-            else:
+            if get_ipython() is not None:
                 _ = display(Markdown(formatted))
+                return
+
+        rich_markdown = rich.markdown.Markdown(formatted)
+        console = rich.console.Console()
+        console.print(rich_markdown)
 
     def add_detail(self, detail: ValidationDetail):
         if detail.status == "failed":
             self.status = "failed"
         elif detail.status != "passed":
             assert_never(detail.status)
```

### Comparing `bioimageio.spec-0.5.1/bioimageio.spec.egg-info/PKG-INFO` & `bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.1
+Version: 0.5.1.post1
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
```

### Comparing `bioimageio.spec-0.5.1/bioimageio.spec.egg-info/SOURCES.txt` & `bioimageio.spec-0.5.1.post1/bioimageio.spec.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 tests/test_generic/__init__.py
 tests/test_generic/test_v0_2.py
 tests/test_generic/test_v0_3.py
 tests/test_internal/__init__.py
 tests/test_internal/test_base_nodes.py
 tests/test_internal/test_constants.py
 tests/test_internal/test_file_source.py
+tests/test_internal/test_io.py
 tests/test_internal/test_license_id.py
 tests/test_internal/test_node.py
 tests/test_internal/test_types.py
 tests/test_internal/test_utils.py
 tests/test_internal/test_validate.py
 tests/test_internal/test_validated_string.py
 tests/test_internal/test_version_type.py
```

### Comparing `bioimageio.spec-0.5.1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py` & `bioimageio.spec-0.5.1.post1/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py` & `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/example_descriptions/models/unet2d_fixed_shape/unet.py` & `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_fixed_shape/unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py` & `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py` & `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py` & `bioimageio.spec-0.5.1.post1/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/pyproject.toml` & `bioimageio.spec-0.5.1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/scripts/compare_yaml_syntax.py` & `bioimageio.spec-0.5.1.post1/scripts/compare_yaml_syntax.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/scripts/generate_json_schemas.py` & `bioimageio.spec-0.5.1.post1/scripts/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/scripts/generate_spec_documentation.py` & `bioimageio.spec-0.5.1.post1/scripts/generate_spec_documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         self, t: Any, abbreviate: bool, inline: bool = True, multiline_level: int = 0
     ) -> str:
         if isinstance(t, FieldInfo):
             parts = list(t.metadata)
             if t.discriminator:
                 parts.append(f"discriminator={t.discriminator}")
 
-            return "; ".join(parts)
+            return "; ".join(map(str, parts))
 
         s = self.slim(str(t))
         if s.startswith("Annotated["):
             args = get_args(t)
             if abbreviate:
                 return f"{self.get_name(args[0], abbreviate, inline, multiline_level)}*"
```

### Comparing `bioimageio.spec-0.5.1/scripts/generate_version_submodule_imports.py` & `bioimageio.spec-0.5.1.post1/scripts/generate_version_submodule_imports.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/scripts/report_invalid_rdfs.py` & `bioimageio.spec-0.5.1.post1/scripts/report_invalid_rdfs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/scripts/update_spdx_licenses.py` & `bioimageio.spec-0.5.1.post1/scripts/update_spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/setup.py` & `bioimageio.spec-0.5.1.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Get the long description from the README file
 ROOT_DIR = Path(__file__).parent.resolve()
 long_description = (ROOT_DIR / "README.md").read_text(encoding="utf-8")
 VERSION_FILE = ROOT_DIR / "bioimageio" / "spec" / "VERSION"
 VERSION = json.loads(VERSION_FILE.read_text(encoding="utf-8"))["version"]
 
 
-setup(
+_ = setup(
     name="bioimageio.spec",
     version=VERSION,
     description="Parser and validator library for bioimage.io specifications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bioimage-io/spec-bioimage-io",
     author="bioimage.io Team",
@@ -35,14 +35,16 @@
         "loguru",
         "numpy>=1.21",
         "packaging>=17.0",
         "pooch",
         "pydantic-settings",
         "pydantic>=2.6.3",
         "python-dateutil",
+        "python-dotenv",
+        "rich",
         "ruyaml",
         "tqdm",
         "typing-extensions",
     ],
     extras_require={
         "dev": [
             "black",
```

### Comparing `bioimageio.spec-0.5.1/tests/test_bioimageio_collection.py` & `bioimageio.spec-0.5.1.post1/tests/test_bioimageio_collection.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_description.py` & `bioimageio.spec-0.5.1.post1/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_example_specs.py` & `bioimageio.spec-0.5.1.post1/tests/test_example_specs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_generic/test_v0_2.py` & `bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_generic/test_v0_3.py` & `bioimageio.spec-0.5.1.post1/tests/test_generic/test_v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_constants.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_file_source.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_file_source.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_license_id.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_node.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_types.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_types.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_utils.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_validate.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_validate.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_internal/test_validated_string.py` & `bioimageio.spec-0.5.1.post1/tests/test_internal/test_validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_model/test_v0_4.py` & `bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_model/test_v0_5.py` & `bioimageio.spec-0.5.1.post1/tests/test_model/test_v0_5.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,23 +375,23 @@
     with pytest.raises(ValueError):
         _ = model.get_axis_sizes(
             ns={(output_tensor_id, output_axis_id): 1}, batch_size=1
         )
 
 
 def test_get_axis_sizes_raises_with_missing_n(model_data: Dict[str, Any]):
-    model_data["outputs"][0]["axes"][2] = {
+    model_data["inputs"][0]["axes"][2] = {
         "type": "space",
         "id": "x",
-        "size": {"tensor_id": "input_1", "axis_id": "x"},
-        "halo": 0,
+        "size": {"min": 10, "step": 5},
     }
 
     with ValidationContext(perform_io_checks=False):
         model = ModelDescr(**model_data)
+
     with pytest.raises(ValueError):
         _ = model.get_axis_sizes(ns={}, batch_size=1)
 
 
 def test_output_ref_shape_mismatch(model_data: Dict[str, Any]):
     model_data["outputs"][0]["axes"][2] = {
         "type": "space",
```

### Comparing `bioimageio.spec-0.5.1/tests/test_package.py` & `bioimageio.spec-0.5.1.post1/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.1/tests/test_specific_reexports_generics.py` & `bioimageio.spec-0.5.1.post1/tests/test_specific_reexports_generics.py`

 * *Files identical despite different names*

