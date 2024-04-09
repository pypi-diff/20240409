# Comparing `tmp/avis_client-0.6.0.tar.gz` & `tmp/avis_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avis_client-0.6.0.tar", max compression
+gzip compressed data, was "avis_client-0.7.0.tar", max compression
```

## Comparing `avis_client-0.6.0.tar` & `avis_client-0.7.0.tar`

### file list

```diff
@@ -1,88 +1,113 @@
--rw-r--r--   0        0        0    11364 2024-03-07 03:22:14.745539 avis_client-0.6.0/LICENSE
--rw-r--r--   0        0        0    18583 2024-03-07 03:22:12.077504 avis_client-0.6.0/README.md
--rw-r--r--   0        0        0     5857 2024-03-07 03:22:12.085504 avis_client-0.6.0/avis_client/__init__.py
--rw-r--r--   0        0        0      959 2024-03-07 03:22:12.089504 avis_client-0.6.0/avis_client/api/__init__.py
--rw-r--r--   0        0        0    22842 2024-03-07 03:22:11.905502 avis_client-0.6.0/avis_client/api/api_keys_api.py
--rw-r--r--   0        0        0    72889 2024-03-07 03:22:11.917502 avis_client-0.6.0/avis_client/api/configuration_api.py
--rw-r--r--   0        0        0    97960 2024-03-07 03:22:11.929502 avis_client-0.6.0/avis_client/api/image_api.py
--rw-r--r--   0        0        0    72761 2024-03-07 03:22:11.941502 avis_client-0.6.0/avis_client/api/image_attribute_api.py
--rw-r--r--   0        0        0    74460 2024-03-07 03:22:11.953502 avis_client-0.6.0/avis_client/api/image_attribute_category_api.py
--rw-r--r--   0        0        0   105894 2024-03-07 03:22:11.965502 avis_client-0.6.0/avis_client/api/inspection_api.py
--rw-r--r--   0        0        0    61222 2024-03-07 03:22:11.973502 avis_client-0.6.0/avis_client/api/membership_api.py
--rw-r--r--   0        0        0    71450 2024-03-07 03:22:11.985503 avis_client-0.6.0/avis_client/api/metadata_api.py
--rw-r--r--   0        0        0    72761 2024-03-07 03:22:11.993503 avis_client-0.6.0/avis_client/api/metadata_schema_api.py
--rw-r--r--   0        0        0   140002 2024-03-07 03:22:12.001503 avis_client-0.6.0/avis_client/api/ml_api.py
--rw-r--r--   0        0        0    73204 2024-03-07 03:22:12.013503 avis_client-0.6.0/avis_client/api/product_api.py
--rw-r--r--   0        0        0    72955 2024-03-07 03:22:12.025503 avis_client-0.6.0/avis_client/api/product_category_api.py
--rw-r--r--   0        0        0    72955 2024-03-07 03:22:12.037503 avis_client-0.6.0/avis_client/api/quality_criteria_api.py
--rw-r--r--   0        0        0    71062 2024-03-07 03:22:12.049503 avis_client-0.6.0/avis_client/api/result_api.py
--rw-r--r--   0        0        0    60346 2024-03-07 03:22:12.061504 avis_client-0.6.0/avis_client/api/team_api.py
--rw-r--r--   0        0        0    19541 2024-03-07 03:22:12.069504 avis_client-0.6.0/avis_client/api/user_api.py
--rw-r--r--   0        0        0    24532 2024-03-07 03:22:12.093504 avis_client-0.6.0/avis_client/api_client.py
--rw-r--r--   0        0        0      674 2024-03-07 03:22:12.093504 avis_client-0.6.0/avis_client/api_response.py
--rw-r--r--   0        0        0    15666 2024-03-07 03:22:12.085504 avis_client-0.6.0/avis_client/configuration.py
--rw-r--r--   0        0        0     5910 2024-03-07 03:22:12.089504 avis_client-0.6.0/avis_client/exceptions.py
--rw-r--r--   0        0        0     4429 2024-03-07 03:22:12.089504 avis_client-0.6.0/avis_client/models/__init__.py
--rw-r--r--   0        0        0     3135 2024-03-07 03:22:11.249493 avis_client-0.6.0/avis_client/models/azure_ml_inference_request.py
--rw-r--r--   0        0        0      746 2024-03-07 03:22:11.257493 avis_client-0.6.0/avis_client/models/blank_enum.py
--rw-r--r--   0        0        0     4794 2024-03-07 03:22:11.273493 avis_client-0.6.0/avis_client/models/configuration_type.py
--rw-r--r--   0        0        0     3968 2024-03-07 03:22:11.289493 avis_client-0.6.0/avis_client/models/configuration_type_request.py
--rw-r--r--   0        0        0     2869 2024-03-07 03:22:11.301494 avis_client-0.6.0/avis_client/models/custom_user.py
--rw-r--r--   0        0        0     2757 2024-03-07 03:22:11.309494 avis_client-0.6.0/avis_client/models/custom_user_request.py
--rw-r--r--   0        0        0     2841 2024-03-07 03:22:11.317494 avis_client-0.6.0/avis_client/models/email_address.py
--rw-r--r--   0        0        0      947 2024-03-07 03:22:11.329494 avis_client-0.6.0/avis_client/models/format_enum.py
--rw-r--r--   0        0        0     4782 2024-03-07 03:22:11.337494 avis_client-0.6.0/avis_client/models/image.py
--rw-r--r--   0        0        0     3897 2024-03-07 03:22:11.349494 avis_client-0.6.0/avis_client/models/image_attribute.py
--rw-r--r--   0        0        0     3953 2024-03-07 03:22:11.357494 avis_client-0.6.0/avis_client/models/image_attribute_category.py
--rw-r--r--   0        0        0     3021 2024-03-07 03:22:11.365494 avis_client-0.6.0/avis_client/models/image_attribute_category_request.py
--rw-r--r--   0        0        0     2965 2024-03-07 03:22:11.369495 avis_client-0.6.0/avis_client/models/image_attribute_request.py
--rw-r--r--   0        0        0     3919 2024-03-07 03:22:11.377495 avis_client-0.6.0/avis_client/models/image_request.py
--rw-r--r--   0        0        0     5778 2024-03-07 03:22:11.385495 avis_client-0.6.0/avis_client/models/inspection.py
--rw-r--r--   0        0        0     4447 2024-03-07 03:22:11.389495 avis_client-0.6.0/avis_client/models/inspection_request.py
--rw-r--r--   0        0        0     2530 2024-03-07 03:22:11.397495 avis_client-0.6.0/avis_client/models/inspection_status.py
--rw-r--r--   0        0        0      845 2024-03-07 03:22:11.401495 avis_client-0.6.0/avis_client/models/inspection_status_enum.py
--rw-r--r--   0        0        0     2570 2024-03-07 03:22:11.405495 avis_client-0.6.0/avis_client/models/inspection_validation_status.py
--rw-r--r--   0        0        0     3841 2024-03-07 03:22:11.437495 avis_client-0.6.0/avis_client/models/membership.py
--rw-r--r--   0        0        0     2434 2024-03-07 03:22:11.445495 avis_client-0.6.0/avis_client/models/membership_request.py
--rw-r--r--   0        0        0     3804 2024-03-07 03:22:11.453496 avis_client-0.6.0/avis_client/models/metadata.py
--rw-r--r--   0        0        0     2872 2024-03-07 03:22:11.457496 avis_client-0.6.0/avis_client/models/metadata_request.py
--rw-r--r--   0        0        0     3630 2024-03-07 03:22:11.465496 avis_client-0.6.0/avis_client/models/metadata_schema.py
--rw-r--r--   0        0        0     2698 2024-03-07 03:22:11.477496 avis_client-0.6.0/avis_client/models/metadata_schema_request.py
--rw-r--r--   0        0        0     4120 2024-03-07 03:22:11.413495 avis_client-0.6.0/avis_client/models/ml_model.py
--rw-r--r--   0        0        0     3330 2024-03-07 03:22:11.417495 avis_client-0.6.0/avis_client/models/ml_model_request.py
--rw-r--r--   0        0        0     4641 2024-03-07 03:22:11.425495 avis_client-0.6.0/avis_client/models/ml_model_type.py
--rw-r--r--   0        0        0     3698 2024-03-07 03:22:11.433495 avis_client-0.6.0/avis_client/models/ml_model_type_request.py
--rw-r--r--   0        0        0     4030 2024-03-07 03:22:11.481496 avis_client-0.6.0/avis_client/models/patched_configuration_type_request.py
--rw-r--r--   0        0        0     3066 2024-03-07 03:22:11.489496 avis_client-0.6.0/avis_client/models/patched_image_attribute_category_request.py
--rw-r--r--   0        0        0     3017 2024-03-07 03:22:11.493496 avis_client-0.6.0/avis_client/models/patched_image_attribute_request.py
--rw-r--r--   0        0        0     3998 2024-03-07 03:22:11.501496 avis_client-0.6.0/avis_client/models/patched_image_request.py
--rw-r--r--   0        0        0     4492 2024-03-07 03:22:11.509496 avis_client-0.6.0/avis_client/models/patched_inspection_request.py
--rw-r--r--   0        0        0     2941 2024-03-07 03:22:11.525497 avis_client-0.6.0/avis_client/models/patched_metadata_request.py
--rw-r--r--   0        0        0     2757 2024-03-07 03:22:11.533497 avis_client-0.6.0/avis_client/models/patched_metadata_schema_request.py
--rw-r--r--   0        0        0     3382 2024-03-07 03:22:11.513496 avis_client-0.6.0/avis_client/models/patched_ml_model_request.py
--rw-r--r--   0        0        0     3726 2024-03-07 03:22:11.521496 avis_client-0.6.0/avis_client/models/patched_ml_model_type_request.py
--rw-r--r--   0        0        0     3219 2024-03-07 03:22:11.541497 avis_client-0.6.0/avis_client/models/patched_product_category_request.py
--rw-r--r--   0        0        0     3532 2024-03-07 03:22:11.545497 avis_client-0.6.0/avis_client/models/patched_product_request.py
--rw-r--r--   0        0        0     3198 2024-03-07 03:22:11.553497 avis_client-0.6.0/avis_client/models/patched_quality_criteria_request.py
--rw-r--r--   0        0        0     4141 2024-03-07 03:22:11.557497 avis_client-0.6.0/avis_client/models/patched_result_request.py
--rw-r--r--   0        0        0     5266 2024-03-07 03:22:11.565497 avis_client-0.6.0/avis_client/models/patched_result_request_status.py
--rw-r--r--   0        0        0     4402 2024-03-07 03:22:11.573497 avis_client-0.6.0/avis_client/models/product.py
--rw-r--r--   0        0        0     4106 2024-03-07 03:22:11.577497 avis_client-0.6.0/avis_client/models/product_category.py
--rw-r--r--   0        0        0     3174 2024-03-07 03:22:11.585497 avis_client-0.6.0/avis_client/models/product_category_request.py
--rw-r--r--   0        0        0     3470 2024-03-07 03:22:11.589497 avis_client-0.6.0/avis_client/models/product_request.py
--rw-r--r--   0        0        0     3861 2024-03-07 03:22:11.593497 avis_client-0.6.0/avis_client/models/quality_criteria.py
--rw-r--r--   0        0        0     3102 2024-03-07 03:22:11.601498 avis_client-0.6.0/avis_client/models/quality_criteria_request.py
--rw-r--r--   0        0        0     2595 2024-03-07 03:22:11.605498 avis_client-0.6.0/avis_client/models/quality_criteria_result.py
--rw-r--r--   0        0        0      843 2024-03-07 03:22:11.609498 avis_client-0.6.0/avis_client/models/quality_enum.py
--rw-r--r--   0        0        0     5028 2024-03-07 03:22:11.613498 avis_client-0.6.0/avis_client/models/result.py
--rw-r--r--   0        0        0     4096 2024-03-07 03:22:11.617498 avis_client-0.6.0/avis_client/models/result_request.py
--rw-r--r--   0        0        0      857 2024-03-07 03:22:11.621498 avis_client-0.6.0/avis_client/models/status_enum.py
--rw-r--r--   0        0        0     4599 2024-03-07 03:22:11.625498 avis_client-0.6.0/avis_client/models/team.py
--rw-r--r--   0        0        0     3535 2024-03-07 03:22:11.633498 avis_client-0.6.0/avis_client/models/team_request.py
--rw-r--r--   0        0        0     3528 2024-03-07 03:22:11.637498 avis_client-0.6.0/avis_client/models/user_api_key_create.py
--rw-r--r--   0        0        0     2603 2024-03-07 03:22:11.641498 avis_client-0.6.0/avis_client/models/user_api_key_create_request.py
--rw-r--r--   0        0        0      896 2024-03-07 03:22:11.645498 avis_client-0.6.0/avis_client/models/validation_status_enum.py
--rw-r--r--   0        0        0        0 2024-03-07 03:22:12.085504 avis_client-0.6.0/avis_client/py.typed
--rw-r--r--   0        0        0     9749 2024-03-07 03:22:12.093504 avis_client-0.6.0/avis_client/rest.py
--rw-r--r--   0        0        0      904 2024-03-07 03:22:14.733539 avis_client-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    19569 1970-01-01 00:00:00.000000 avis_client-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11364 2024-03-07 03:22:14.745539 avis_client-0.7.0/LICENSE
+-rw-r--r--   0        0        0    21680 2024-04-09 13:30:25.744450 avis_client-0.7.0/README.md
+-rw-r--r--   0        0        0     8054 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/__init__.py
+-rw-r--r--   0        0        0     1018 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/api/__init__.py
+-rw-r--r--   0        0        0    22842 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/api/api_keys_api.py
+-rw-r--r--   0        0        0    75618 2024-04-09 13:30:25.744450 avis_client-0.7.0/avis_client/api/configuration_api.py
+-rw-r--r--   0        0        0   105986 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/image_api.py
+-rw-r--r--   0        0        0    75484 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/image_attribute_api.py
+-rw-r--r--   0        0        0    77200 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/image_attribute_category_api.py
+-rw-r--r--   0        0        0   113930 2024-04-09 13:30:25.748450 avis_client-0.7.0/avis_client/api/inspection_api.py
+-rw-r--r--   0        0        0    63041 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/membership_api.py
+-rw-r--r--   0        0        0    74160 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/metadata_api.py
+-rw-r--r--   0        0        0    75484 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/metadata_schema_api.py
+-rw-r--r--   0        0        0   143687 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/ml_api.py
+-rw-r--r--   0        0        0    75912 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/product_api.py
+-rw-r--r--   0        0        0    75680 2024-04-09 13:30:25.752450 avis_client-0.7.0/avis_client/api/product_category_api.py
+-rw-r--r--   0        0        0    75680 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/quality_criteria_api.py
+-rw-r--r--   0        0        0    73768 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/result_api.py
+-rw-r--r--   0        0        0   109694 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/statistics_api.py
+-rw-r--r--   0        0        0    62209 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/teams_api.py
+-rw-r--r--   0        0        0    19541 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api/user_api.py
+-rw-r--r--   0        0        0    24532 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/api_client.py
+-rw-r--r--   0        0        0      674 2024-03-07 03:22:12.093504 avis_client-0.7.0/avis_client/api_response.py
+-rw-r--r--   0        0        0    15507 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/configuration.py
+-rw-r--r--   0        0        0     5910 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/exceptions.py
+-rw-r--r--   0        0        0     6567 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/__init__.py
+-rw-r--r--   0        0        0     3135 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/azure_ml_inference_request.py
+-rw-r--r--   0        0        0      746 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/blank_enum.py
+-rw-r--r--   0        0        0     4794 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/configuration_type.py
+-rw-r--r--   0        0        0     3968 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/configuration_type_request.py
+-rw-r--r--   0        0        0     2869 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/custom_user.py
+-rw-r--r--   0        0        0     2757 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/custom_user_request.py
+-rw-r--r--   0        0        0     2841 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/email_address.py
+-rw-r--r--   0        0        0      947 2024-04-09 13:30:25.756450 avis_client-0.7.0/avis_client/models/format_enum.py
+-rw-r--r--   0        0        0     4782 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image.py
+-rw-r--r--   0        0        0     3897 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute.py
+-rw-r--r--   0        0        0     3953 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute_category.py
+-rw-r--r--   0        0        0     3021 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute_category_request.py
+-rw-r--r--   0        0        0     2965 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_attribute_request.py
+-rw-r--r--   0        0        0     3919 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/image_request.py
+-rw-r--r--   0        0        0     5778 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection.py
+-rw-r--r--   0        0        0     2524 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_images_statistics.py
+-rw-r--r--   0        0        0     2552 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_images_statistics_request.py
+-rw-r--r--   0        0        0     4447 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_request.py
+-rw-r--r--   0        0        0     2770 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_statistics.py
+-rw-r--r--   0        0        0     2798 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_statistics_request.py
+-rw-r--r--   0        0        0     2530 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_status.py
+-rw-r--r--   0        0        0      845 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_status_enum.py
+-rw-r--r--   0        0        0     2570 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/inspection_validation_status.py
+-rw-r--r--   0        0        0     3841 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/membership.py
+-rw-r--r--   0        0        0     2434 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/membership_request.py
+-rw-r--r--   0        0        0     3804 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata.py
+-rw-r--r--   0        0        0     2872 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata_request.py
+-rw-r--r--   0        0        0     3630 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata_schema.py
+-rw-r--r--   0        0        0     2698 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/metadata_schema_request.py
+-rw-r--r--   0        0        0     4120 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model.py
+-rw-r--r--   0        0        0     3330 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model_request.py
+-rw-r--r--   0        0        0     4641 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model_type.py
+-rw-r--r--   0        0        0     3698 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/ml_model_type_request.py
+-rw-r--r--   0        0        0     3602 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_configuration_type_list.py
+-rw-r--r--   0        0        0     3643 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_image_attribute_category_list.py
+-rw-r--r--   0        0        0     3578 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_image_attribute_list.py
+-rw-r--r--   0        0        0     3505 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_image_list.py
+-rw-r--r--   0        0        0     3675 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_images_statistics_list.py
+-rw-r--r--   0        0        0     3545 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_list.py
+-rw-r--r--   0        0        0     3626 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_statistics_list.py
+-rw-r--r--   0        0        0     3594 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_status_list.py
+-rw-r--r--   0        0        0     3675 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_inspection_validation_status_list.py
+-rw-r--r--   0        0        0     3545 2024-04-09 13:30:25.760450 avis_client-0.7.0/avis_client/models/paginated_membership_list.py
+-rw-r--r--   0        0        0     3529 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_metadata_list.py
+-rw-r--r--   0        0        0     3578 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_metadata_schema_list.py
+-rw-r--r--   0        0        0     3522 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_ml_model_list.py
+-rw-r--r--   0        0        0     3555 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_ml_model_type_list.py
+-rw-r--r--   0        0        0     3586 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_product_category_list.py
+-rw-r--r--   0        0        0     3521 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_product_list.py
+-rw-r--r--   0        0        0     3586 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_quality_criteria_list.py
+-rw-r--r--   0        0        0     3635 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_quality_criteria_result_list.py
+-rw-r--r--   0        0        0     3513 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_result_list.py
+-rw-r--r--   0        0        0     3497 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/paginated_team_list.py
+-rw-r--r--   0        0        0     4030 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_configuration_type_request.py
+-rw-r--r--   0        0        0     3066 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_image_attribute_category_request.py
+-rw-r--r--   0        0        0     3017 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_image_attribute_request.py
+-rw-r--r--   0        0        0     3998 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_image_request.py
+-rw-r--r--   0        0        0     4492 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_inspection_request.py
+-rw-r--r--   0        0        0     2941 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_metadata_request.py
+-rw-r--r--   0        0        0     2757 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_metadata_schema_request.py
+-rw-r--r--   0        0        0     3382 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_ml_model_request.py
+-rw-r--r--   0        0        0     3726 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_ml_model_type_request.py
+-rw-r--r--   0        0        0     3219 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_product_category_request.py
+-rw-r--r--   0        0        0     3532 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_product_request.py
+-rw-r--r--   0        0        0     3198 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_quality_criteria_request.py
+-rw-r--r--   0        0        0     4141 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_result_request.py
+-rw-r--r--   0        0        0     5266 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/patched_result_request_status.py
+-rw-r--r--   0        0        0     4402 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product.py
+-rw-r--r--   0        0        0     4106 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product_category.py
+-rw-r--r--   0        0        0     3174 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product_category_request.py
+-rw-r--r--   0        0        0     3470 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/product_request.py
+-rw-r--r--   0        0        0     3861 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_criteria.py
+-rw-r--r--   0        0        0     3102 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_criteria_request.py
+-rw-r--r--   0        0        0     2595 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_criteria_result.py
+-rw-r--r--   0        0        0      843 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/quality_enum.py
+-rw-r--r--   0        0        0     5028 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/result.py
+-rw-r--r--   0        0        0     4096 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/result_request.py
+-rw-r--r--   0        0        0      857 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/status_enum.py
+-rw-r--r--   0        0        0     4599 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/team.py
+-rw-r--r--   0        0        0     3535 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/team_request.py
+-rw-r--r--   0        0        0     3528 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/user_api_key_create.py
+-rw-r--r--   0        0        0     2603 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/user_api_key_create_request.py
+-rw-r--r--   0        0        0      896 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/models/validation_status_enum.py
+-rw-r--r--   0        0        0        0 2024-03-07 03:22:12.085504 avis_client-0.7.0/avis_client/py.typed
+-rw-r--r--   0        0        0     9749 2024-04-09 13:30:25.764449 avis_client-0.7.0/avis_client/rest.py
+-rw-r--r--   0        0        0      904 2024-04-09 13:30:25.768449 avis_client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    22666 1970-01-01 00:00:00.000000 avis_client-0.7.0/PKG-INFO
```

### Comparing `avis_client-0.6.0/LICENSE` & `avis_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avis_client-0.6.0/README.md` & `avis_client-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,40 @@
+Metadata-Version: 2.1
+Name: avis_client
+Version: 0.7.0
+Summary: AVIS Python client
+Home-page: https://docs.vu.engineering/api/clients/python/avis_client/
+License: Apache-2.0
+Keywords: OpenAPI,avis,api client
+Author: VUEngineering
+Author-email: tech@vu.engineering
+Maintainer: Adriano Pagano
+Maintainer-email: adriano.pagano@vu.engineering
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=2)
+Requires-Dist: python-dateutil (>=2.8.2)
+Requires-Dist: typing-extensions (>=4.7.1)
+Requires-Dist: urllib3 (>=1.25.3)
+Project-URL: Repository, https://github.com/vuengineering/public/
+Description-Content-Type: text/markdown
+
 # avis-client
 VUE Autonomous Visual Inspection System (AVIS)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.6.0
-- Package version: 0.6.0
+- API version: 0.7.0
+- Package version: 0.7.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -51,18 +77,18 @@
 ```python
 
 import time
 import avis_client
 from avis_client.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to https://avis.vu.engineering
+# Defining the host is optional and defaults to http://localhost:8000
 # See configuration.py for a list of all supported configuration parameters.
 configuration = avis_client.Configuration(
-    host = "https://avis.vu.engineering"
+    host = "http://localhost:8000"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
@@ -92,15 +118,15 @@
     except ApiException as e:
         print("Exception when calling ApiKeysApi->keys_create: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://avis.vu.engineering*
+All URIs are relative to *http://localhost:8000*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApiKeysApi* | [**keys_create**](docs/ApiKeysApi.md#keys_create) | **POST** /api/keys/ | 
 *ApiKeysApi* | [**keys_revoke_create**](docs/ApiKeysApi.md#keys_revoke_create) | **POST** /api/keys/revoke/ | 
 *ConfigurationApi* | [**configuration_create**](docs/ConfigurationApi.md#configuration_create) | **POST** /api/configuration/ | 
 *ConfigurationApi* | [**configuration_destroy**](docs/ConfigurationApi.md#configuration_destroy) | **DELETE** /api/configuration/{id}/ | 
@@ -152,25 +178,25 @@
 *MetadataSchemaApi* | [**metadata_schema_destroy**](docs/MetadataSchemaApi.md#metadata_schema_destroy) | **DELETE** /api/metadata-schema/{id}/ | 
 *MetadataSchemaApi* | [**metadata_schema_list**](docs/MetadataSchemaApi.md#metadata_schema_list) | **GET** /api/metadata-schema/ | 
 *MetadataSchemaApi* | [**metadata_schema_partial_update**](docs/MetadataSchemaApi.md#metadata_schema_partial_update) | **PATCH** /api/metadata-schema/{id}/ | 
 *MetadataSchemaApi* | [**metadata_schema_retrieve**](docs/MetadataSchemaApi.md#metadata_schema_retrieve) | **GET** /api/metadata-schema/{id}/ | 
 *MetadataSchemaApi* | [**metadata_schema_update**](docs/MetadataSchemaApi.md#metadata_schema_update) | **PUT** /api/metadata-schema/{id}/ | 
 *MlApi* | [**ml_model_create**](docs/MlApi.md#ml_model_create) | **POST** /api/ml/model/ | 
 *MlApi* | [**ml_model_destroy**](docs/MlApi.md#ml_model_destroy) | **DELETE** /api/ml/model/{id}/ | 
-*MlApi* | [**ml_model_inference**](docs/MlApi.md#ml_model_inference) | **POST** /api/ml/model/{id}/inference/ | 
+*MlApi* | [**ml_model_inference**](docs/MlApi.md#ml_model_inference) | **POST** /api/ml/model/{id}/infer/ | 
 *MlApi* | [**ml_model_list**](docs/MlApi.md#ml_model_list) | **GET** /api/ml/model/ | 
 *MlApi* | [**ml_model_partial_update**](docs/MlApi.md#ml_model_partial_update) | **PATCH** /api/ml/model/{id}/ | 
 *MlApi* | [**ml_model_retrieve**](docs/MlApi.md#ml_model_retrieve) | **GET** /api/ml/model/{id}/ | 
+*MlApi* | [**ml_model_type_create**](docs/MlApi.md#ml_model_type_create) | **POST** /api/ml/model-type/ | 
+*MlApi* | [**ml_model_type_destroy**](docs/MlApi.md#ml_model_type_destroy) | **DELETE** /api/ml/model-type/{id}/ | 
+*MlApi* | [**ml_model_type_list**](docs/MlApi.md#ml_model_type_list) | **GET** /api/ml/model-type/ | 
+*MlApi* | [**ml_model_type_partial_update**](docs/MlApi.md#ml_model_type_partial_update) | **PATCH** /api/ml/model-type/{id}/ | 
+*MlApi* | [**ml_model_type_retrieve**](docs/MlApi.md#ml_model_type_retrieve) | **GET** /api/ml/model-type/{id}/ | 
+*MlApi* | [**ml_model_type_update**](docs/MlApi.md#ml_model_type_update) | **PUT** /api/ml/model-type/{id}/ | 
 *MlApi* | [**ml_model_update**](docs/MlApi.md#ml_model_update) | **PUT** /api/ml/model/{id}/ | 
-*MlApi* | [**ml_modeltype_create**](docs/MlApi.md#ml_modeltype_create) | **POST** /api/ml/modeltype/ | 
-*MlApi* | [**ml_modeltype_destroy**](docs/MlApi.md#ml_modeltype_destroy) | **DELETE** /api/ml/modeltype/{id}/ | 
-*MlApi* | [**ml_modeltype_list**](docs/MlApi.md#ml_modeltype_list) | **GET** /api/ml/modeltype/ | 
-*MlApi* | [**ml_modeltype_partial_update**](docs/MlApi.md#ml_modeltype_partial_update) | **PATCH** /api/ml/modeltype/{id}/ | 
-*MlApi* | [**ml_modeltype_retrieve**](docs/MlApi.md#ml_modeltype_retrieve) | **GET** /api/ml/modeltype/{id}/ | 
-*MlApi* | [**ml_modeltype_update**](docs/MlApi.md#ml_modeltype_update) | **PUT** /api/ml/modeltype/{id}/ | 
 *ProductApi* | [**product_create**](docs/ProductApi.md#product_create) | **POST** /api/product/ | 
 *ProductApi* | [**product_destroy**](docs/ProductApi.md#product_destroy) | **DELETE** /api/product/{id}/ | 
 *ProductApi* | [**product_list**](docs/ProductApi.md#product_list) | **GET** /api/product/ | 
 *ProductApi* | [**product_partial_update**](docs/ProductApi.md#product_partial_update) | **PATCH** /api/product/{id}/ | 
 *ProductApi* | [**product_retrieve**](docs/ProductApi.md#product_retrieve) | **GET** /api/product/{id}/ | 
 *ProductApi* | [**product_update**](docs/ProductApi.md#product_update) | **PUT** /api/product/{id}/ | 
 *ProductCategoryApi* | [**product_category_create**](docs/ProductCategoryApi.md#product_category_create) | **POST** /api/product-category/ | 
@@ -187,19 +213,29 @@
 *QualityCriteriaApi* | [**quality_criteria_update**](docs/QualityCriteriaApi.md#quality_criteria_update) | **PUT** /api/quality-criteria/{id}/ | 
 *ResultApi* | [**result_create**](docs/ResultApi.md#result_create) | **POST** /api/result/ | 
 *ResultApi* | [**result_destroy**](docs/ResultApi.md#result_destroy) | **DELETE** /api/result/{id}/ | 
 *ResultApi* | [**result_list**](docs/ResultApi.md#result_list) | **GET** /api/result/ | 
 *ResultApi* | [**result_partial_update**](docs/ResultApi.md#result_partial_update) | **PATCH** /api/result/{id}/ | 
 *ResultApi* | [**result_retrieve**](docs/ResultApi.md#result_retrieve) | **GET** /api/result/{id}/ | 
 *ResultApi* | [**result_update**](docs/ResultApi.md#result_update) | **PUT** /api/result/{id}/ | 
-*TeamApi* | [**team_create**](docs/TeamApi.md#team_create) | **POST** /api/team/ | 
-*TeamApi* | [**team_destroy**](docs/TeamApi.md#team_destroy) | **DELETE** /api/team/{id}/ | 
-*TeamApi* | [**team_list**](docs/TeamApi.md#team_list) | **GET** /api/team/ | 
-*TeamApi* | [**team_retrieve**](docs/TeamApi.md#team_retrieve) | **GET** /api/team/{id}/ | 
-*TeamApi* | [**team_update**](docs/TeamApi.md#team_update) | **PUT** /api/team/{id}/ | 
+*StatisticsApi* | [**statistics_inspection_create**](docs/StatisticsApi.md#statistics_inspection_create) | **POST** /api/statistics/inspection/ | 
+*StatisticsApi* | [**statistics_inspection_destroy**](docs/StatisticsApi.md#statistics_inspection_destroy) | **DELETE** /api/statistics/inspection/{id}/ | 
+*StatisticsApi* | [**statistics_inspection_list**](docs/StatisticsApi.md#statistics_inspection_list) | **GET** /api/statistics/inspection/ | 
+*StatisticsApi* | [**statistics_inspection_retrieve**](docs/StatisticsApi.md#statistics_inspection_retrieve) | **GET** /api/statistics/inspection/{id}/ | 
+*StatisticsApi* | [**statistics_inspection_update**](docs/StatisticsApi.md#statistics_inspection_update) | **PUT** /api/statistics/inspection/{id}/ | 
+*StatisticsApi* | [**statistics_team_create**](docs/StatisticsApi.md#statistics_team_create) | **POST** /api/statistics/team/ | 
+*StatisticsApi* | [**statistics_team_destroy**](docs/StatisticsApi.md#statistics_team_destroy) | **DELETE** /api/statistics/team/{id}/ | 
+*StatisticsApi* | [**statistics_team_list**](docs/StatisticsApi.md#statistics_team_list) | **GET** /api/statistics/team/ | 
+*StatisticsApi* | [**statistics_team_retrieve**](docs/StatisticsApi.md#statistics_team_retrieve) | **GET** /api/statistics/team/{id}/ | 
+*StatisticsApi* | [**statistics_team_update**](docs/StatisticsApi.md#statistics_team_update) | **PUT** /api/statistics/team/{id}/ | 
+*TeamsApi* | [**teams_create**](docs/TeamsApi.md#teams_create) | **POST** /api/teams/ | 
+*TeamsApi* | [**teams_destroy**](docs/TeamsApi.md#teams_destroy) | **DELETE** /api/teams/{id}/ | 
+*TeamsApi* | [**teams_list**](docs/TeamsApi.md#teams_list) | **GET** /api/teams/ | 
+*TeamsApi* | [**teams_retrieve**](docs/TeamsApi.md#teams_retrieve) | **GET** /api/teams/{id}/ | 
+*TeamsApi* | [**teams_update**](docs/TeamsApi.md#teams_update) | **PUT** /api/teams/{id}/ | 
 *UserApi* | [**user_email_list**](docs/UserApi.md#user_email_list) | **GET** /api/user/email/ | 
 *UserApi* | [**user_whoami_retrieve**](docs/UserApi.md#user_whoami_retrieve) | **GET** /api/user/whoami/ | 
 
 
 ## Documentation For Models
 
  - [AzureMLInferenceRequest](docs/AzureMLInferenceRequest.md)
@@ -213,28 +249,52 @@
  - [Image](docs/Image.md)
  - [ImageAttribute](docs/ImageAttribute.md)
  - [ImageAttributeCategory](docs/ImageAttributeCategory.md)
  - [ImageAttributeCategoryRequest](docs/ImageAttributeCategoryRequest.md)
  - [ImageAttributeRequest](docs/ImageAttributeRequest.md)
  - [ImageRequest](docs/ImageRequest.md)
  - [Inspection](docs/Inspection.md)
+ - [InspectionImagesStatistics](docs/InspectionImagesStatistics.md)
+ - [InspectionImagesStatisticsRequest](docs/InspectionImagesStatisticsRequest.md)
  - [InspectionRequest](docs/InspectionRequest.md)
+ - [InspectionStatistics](docs/InspectionStatistics.md)
+ - [InspectionStatisticsRequest](docs/InspectionStatisticsRequest.md)
  - [InspectionStatus](docs/InspectionStatus.md)
  - [InspectionStatusEnum](docs/InspectionStatusEnum.md)
  - [InspectionValidationStatus](docs/InspectionValidationStatus.md)
  - [MLModel](docs/MLModel.md)
  - [MLModelRequest](docs/MLModelRequest.md)
  - [MLModelType](docs/MLModelType.md)
  - [MLModelTypeRequest](docs/MLModelTypeRequest.md)
  - [Membership](docs/Membership.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [Metadata](docs/Metadata.md)
  - [MetadataRequest](docs/MetadataRequest.md)
  - [MetadataSchema](docs/MetadataSchema.md)
  - [MetadataSchemaRequest](docs/MetadataSchemaRequest.md)
+ - [PaginatedConfigurationTypeList](docs/PaginatedConfigurationTypeList.md)
+ - [PaginatedImageAttributeCategoryList](docs/PaginatedImageAttributeCategoryList.md)
+ - [PaginatedImageAttributeList](docs/PaginatedImageAttributeList.md)
+ - [PaginatedImageList](docs/PaginatedImageList.md)
+ - [PaginatedInspectionImagesStatisticsList](docs/PaginatedInspectionImagesStatisticsList.md)
+ - [PaginatedInspectionList](docs/PaginatedInspectionList.md)
+ - [PaginatedInspectionStatisticsList](docs/PaginatedInspectionStatisticsList.md)
+ - [PaginatedInspectionStatusList](docs/PaginatedInspectionStatusList.md)
+ - [PaginatedInspectionValidationStatusList](docs/PaginatedInspectionValidationStatusList.md)
+ - [PaginatedMLModelList](docs/PaginatedMLModelList.md)
+ - [PaginatedMLModelTypeList](docs/PaginatedMLModelTypeList.md)
+ - [PaginatedMembershipList](docs/PaginatedMembershipList.md)
+ - [PaginatedMetadataList](docs/PaginatedMetadataList.md)
+ - [PaginatedMetadataSchemaList](docs/PaginatedMetadataSchemaList.md)
+ - [PaginatedProductCategoryList](docs/PaginatedProductCategoryList.md)
+ - [PaginatedProductList](docs/PaginatedProductList.md)
+ - [PaginatedQualityCriteriaList](docs/PaginatedQualityCriteriaList.md)
+ - [PaginatedQualityCriteriaResultList](docs/PaginatedQualityCriteriaResultList.md)
+ - [PaginatedResultList](docs/PaginatedResultList.md)
+ - [PaginatedTeamList](docs/PaginatedTeamList.md)
  - [PatchedConfigurationTypeRequest](docs/PatchedConfigurationTypeRequest.md)
  - [PatchedImageAttributeCategoryRequest](docs/PatchedImageAttributeCategoryRequest.md)
  - [PatchedImageAttributeRequest](docs/PatchedImageAttributeRequest.md)
  - [PatchedImageRequest](docs/PatchedImageRequest.md)
  - [PatchedInspectionRequest](docs/PatchedInspectionRequest.md)
  - [PatchedMLModelRequest](docs/PatchedMLModelRequest.md)
  - [PatchedMLModelTypeRequest](docs/PatchedMLModelTypeRequest.md)
@@ -284,7 +344,8 @@
 
 
 ## Author
 
 
 
 
+
```

### Comparing `avis_client-0.6.0/avis_client/__init__.py` & `avis_client-0.7.0/avis_client/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,23 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.6.0"
-
-# import apis into sdk package
-from avis_client.api.api_keys_api import ApiKeysApi
-from avis_client.api.configuration_api import ConfigurationApi
-from avis_client.api.image_api import ImageApi
-from avis_client.api.image_attribute_api import ImageAttributeApi
-from avis_client.api.image_attribute_category_api import ImageAttributeCategoryApi
-from avis_client.api.inspection_api import InspectionApi
-from avis_client.api.membership_api import MembershipApi
-from avis_client.api.metadata_api import MetadataApi
-from avis_client.api.metadata_schema_api import MetadataSchemaApi
-from avis_client.api.ml_api import MlApi
-from avis_client.api.product_api import ProductApi
-from avis_client.api.product_category_api import ProductCategoryApi
-from avis_client.api.quality_criteria_api import QualityCriteriaApi
-from avis_client.api.result_api import ResultApi
-from avis_client.api.team_api import TeamApi
-from avis_client.api.user_api import UserApi
-
-# import ApiClient
-from avis_client.api_response import ApiResponse
-from avis_client.api_client import ApiClient
-from avis_client.configuration import Configuration
-from avis_client.exceptions import OpenApiException
-from avis_client.exceptions import ApiTypeError
-from avis_client.exceptions import ApiValueError
-from avis_client.exceptions import ApiKeyError
-from avis_client.exceptions import ApiAttributeError
-from avis_client.exceptions import ApiException
-
-# import models into sdk package
+# import models into model package
 from avis_client.models.azure_ml_inference_request import AzureMLInferenceRequest
 from avis_client.models.blank_enum import BlankEnum
 from avis_client.models.configuration_type import ConfigurationType
 from avis_client.models.configuration_type_request import ConfigurationTypeRequest
 from avis_client.models.custom_user import CustomUser
 from avis_client.models.custom_user_request import CustomUserRequest
 from avis_client.models.email_address import EmailAddress
@@ -57,28 +25,52 @@
 from avis_client.models.image import Image
 from avis_client.models.image_attribute import ImageAttribute
 from avis_client.models.image_attribute_category import ImageAttributeCategory
 from avis_client.models.image_attribute_category_request import ImageAttributeCategoryRequest
 from avis_client.models.image_attribute_request import ImageAttributeRequest
 from avis_client.models.image_request import ImageRequest
 from avis_client.models.inspection import Inspection
+from avis_client.models.inspection_images_statistics import InspectionImagesStatistics
+from avis_client.models.inspection_images_statistics_request import InspectionImagesStatisticsRequest
 from avis_client.models.inspection_request import InspectionRequest
+from avis_client.models.inspection_statistics import InspectionStatistics
+from avis_client.models.inspection_statistics_request import InspectionStatisticsRequest
 from avis_client.models.inspection_status import InspectionStatus
 from avis_client.models.inspection_status_enum import InspectionStatusEnum
 from avis_client.models.inspection_validation_status import InspectionValidationStatus
 from avis_client.models.ml_model import MLModel
 from avis_client.models.ml_model_request import MLModelRequest
 from avis_client.models.ml_model_type import MLModelType
 from avis_client.models.ml_model_type_request import MLModelTypeRequest
 from avis_client.models.membership import Membership
 from avis_client.models.membership_request import MembershipRequest
 from avis_client.models.metadata import Metadata
 from avis_client.models.metadata_request import MetadataRequest
 from avis_client.models.metadata_schema import MetadataSchema
 from avis_client.models.metadata_schema_request import MetadataSchemaRequest
+from avis_client.models.paginated_configuration_type_list import PaginatedConfigurationTypeList
+from avis_client.models.paginated_image_attribute_category_list import PaginatedImageAttributeCategoryList
+from avis_client.models.paginated_image_attribute_list import PaginatedImageAttributeList
+from avis_client.models.paginated_image_list import PaginatedImageList
+from avis_client.models.paginated_inspection_images_statistics_list import PaginatedInspectionImagesStatisticsList
+from avis_client.models.paginated_inspection_list import PaginatedInspectionList
+from avis_client.models.paginated_inspection_statistics_list import PaginatedInspectionStatisticsList
+from avis_client.models.paginated_inspection_status_list import PaginatedInspectionStatusList
+from avis_client.models.paginated_inspection_validation_status_list import PaginatedInspectionValidationStatusList
+from avis_client.models.paginated_ml_model_list import PaginatedMLModelList
+from avis_client.models.paginated_ml_model_type_list import PaginatedMLModelTypeList
+from avis_client.models.paginated_membership_list import PaginatedMembershipList
+from avis_client.models.paginated_metadata_list import PaginatedMetadataList
+from avis_client.models.paginated_metadata_schema_list import PaginatedMetadataSchemaList
+from avis_client.models.paginated_product_category_list import PaginatedProductCategoryList
+from avis_client.models.paginated_product_list import PaginatedProductList
+from avis_client.models.paginated_quality_criteria_list import PaginatedQualityCriteriaList
+from avis_client.models.paginated_quality_criteria_result_list import PaginatedQualityCriteriaResultList
+from avis_client.models.paginated_result_list import PaginatedResultList
+from avis_client.models.paginated_team_list import PaginatedTeamList
 from avis_client.models.patched_configuration_type_request import PatchedConfigurationTypeRequest
 from avis_client.models.patched_image_attribute_category_request import PatchedImageAttributeCategoryRequest
 from avis_client.models.patched_image_attribute_request import PatchedImageAttributeRequest
 from avis_client.models.patched_image_request import PatchedImageRequest
 from avis_client.models.patched_inspection_request import PatchedInspectionRequest
 from avis_client.models.patched_ml_model_request import PatchedMLModelRequest
 from avis_client.models.patched_ml_model_type_request import PatchedMLModelTypeRequest
```

### Comparing `avis_client-0.6.0/avis_client/api/__init__.py` & `avis_client-0.7.0/avis_client/api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 from avis_client.api.metadata_api import MetadataApi
 from avis_client.api.metadata_schema_api import MetadataSchemaApi
 from avis_client.api.ml_api import MlApi
 from avis_client.api.product_api import ProductApi
 from avis_client.api.product_category_api import ProductCategoryApi
 from avis_client.api.quality_criteria_api import QualityCriteriaApi
 from avis_client.api.result_api import ResultApi
-from avis_client.api.team_api import TeamApi
+from avis_client.api.statistics_api import StatisticsApi
+from avis_client.api.teams_api import TeamsApi
 from avis_client.api.user_api import UserApi
```

### Comparing `avis_client-0.6.0/avis_client/api/api_keys_api.py` & `avis_client-0.7.0/avis_client/api/api_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.6.0/avis_client/api/configuration_api.py` & `avis_client-0.7.0/avis_client/api/configuration_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -27,14 +27,15 @@
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from avis_client.models.configuration_type import ConfigurationType
 from avis_client.models.configuration_type_request import ConfigurationTypeRequest
+from avis_client.models.paginated_configuration_type_list import PaginatedConfigurationTypeList
 from avis_client.models.patched_configuration_type_request import PatchedConfigurationTypeRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def configuration_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ConfigurationType]:
+    ) -> PaginatedConfigurationTypeList:
         """configuration_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._configuration_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ConfigurationType]",
+            '200': "PaginatedConfigurationTypeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def configuration_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ConfigurationType]]:
+    ) -> ApiResponse[PaginatedConfigurationTypeList]:
         """configuration_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._configuration_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ConfigurationType]",
+            '200': "PaginatedConfigurationTypeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def configuration_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._configuration_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ConfigurationType]",
+            '200': "PaginatedConfigurationTypeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _configuration_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/image_api.py` & `avis_client-0.7.0/avis_client/api/inspection_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -21,93 +21,66 @@
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from datetime import datetime
+from pydantic import StrictInt, StrictStr
 
-from pydantic import StrictBytes, StrictInt, StrictStr
+from typing import List, Optional
 
-from typing import List, Optional, Union
-
-from avis_client.models.format_enum import FormatEnum
-from avis_client.models.image import Image
-from avis_client.models.image_request import ImageRequest
-from avis_client.models.inspection_status import InspectionStatus
-from avis_client.models.patched_image_request import PatchedImageRequest
-from avis_client.models.quality_criteria_result import QualityCriteriaResult
-from avis_client.models.validation_status_enum import ValidationStatusEnum
+from avis_client.models.inspection import Inspection
+from avis_client.models.inspection_request import InspectionRequest
+from avis_client.models.paginated_inspection_list import PaginatedInspectionList
+from avis_client.models.paginated_inspection_status_list import PaginatedInspectionStatusList
+from avis_client.models.paginated_inspection_validation_status_list import PaginatedInspectionValidationStatusList
+from avis_client.models.patched_inspection_request import PatchedInspectionRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
-class ImageApi:
+class InspectionApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def image_create(
+    def inspection_create(
         self,
-        team: StrictInt,
-        capture_datetime: datetime,
-        file: Union[StrictBytes, StrictStr],
-        inspection: Optional[StrictInt] = None,
-        uploaded_by: Optional[StrictInt] = None,
-        results: Optional[List[StrictInt]] = None,
-        format: Optional[FormatEnum] = None,
-        part_id: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None,
-        validation_status: Optional[ValidationStatusEnum] = None,
+        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Image:
-        """image_create
+    ) -> Inspection:
+        """inspection_create
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param team: (required)
-        :type team: int
-        :param capture_datetime: (required)
-        :type capture_datetime: datetime
-        :param file: (required)
-        :type file: bytearray
-        :param inspection:
-        :type inspection: int
-        :param uploaded_by:
-        :type uploaded_by: int
-        :param results:
-        :type results: List[int]
-        :param format:
-        :type format: FormatEnum
-        :param part_id:
-        :type part_id: str
-        :param validation_status:
-        :type validation_status: ValidationStatusEnum
+        :param inspection_request: (required)
+        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -122,91 +95,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_create_serialize(
-            team=team,
-            capture_datetime=capture_datetime,
-            file=file,
-            inspection=inspection,
-            uploaded_by=uploaded_by,
-            results=results,
-            format=format,
-            part_id=part_id,
-            validation_status=validation_status,
+        _param = self._inspection_create_serialize(
+            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Image",
+            '201': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_create_with_http_info(
+    def inspection_create_with_http_info(
         self,
-        team: StrictInt,
-        capture_datetime: datetime,
-        file: Union[StrictBytes, StrictStr],
-        inspection: Optional[StrictInt] = None,
-        uploaded_by: Optional[StrictInt] = None,
-        results: Optional[List[StrictInt]] = None,
-        format: Optional[FormatEnum] = None,
-        part_id: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None,
-        validation_status: Optional[ValidationStatusEnum] = None,
+        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Image]:
-        """image_create
+    ) -> ApiResponse[Inspection]:
+        """inspection_create
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param team: (required)
-        :type team: int
-        :param capture_datetime: (required)
-        :type capture_datetime: datetime
-        :param file: (required)
-        :type file: bytearray
-        :param inspection:
-        :type inspection: int
-        :param uploaded_by:
-        :type uploaded_by: int
-        :param results:
-        :type results: List[int]
-        :param format:
-        :type format: FormatEnum
-        :param part_id:
-        :type part_id: str
-        :param validation_status:
-        :type validation_status: ValidationStatusEnum
+        :param inspection_request: (required)
+        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -221,91 +162,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_create_serialize(
-            team=team,
-            capture_datetime=capture_datetime,
-            file=file,
-            inspection=inspection,
-            uploaded_by=uploaded_by,
-            results=results,
-            format=format,
-            part_id=part_id,
-            validation_status=validation_status,
+        _param = self._inspection_create_serialize(
+            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Image",
+            '201': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_create_without_preload_content(
+    def inspection_create_without_preload_content(
         self,
-        team: StrictInt,
-        capture_datetime: datetime,
-        file: Union[StrictBytes, StrictStr],
-        inspection: Optional[StrictInt] = None,
-        uploaded_by: Optional[StrictInt] = None,
-        results: Optional[List[StrictInt]] = None,
-        format: Optional[FormatEnum] = None,
-        part_id: Optional[Annotated[str, Field(strict=True, max_length=255)]] = None,
-        validation_status: Optional[ValidationStatusEnum] = None,
+        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_create
+        """inspection_create
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param team: (required)
-        :type team: int
-        :param capture_datetime: (required)
-        :type capture_datetime: datetime
-        :param file: (required)
-        :type file: bytearray
-        :param inspection:
-        :type inspection: int
-        :param uploaded_by:
-        :type uploaded_by: int
-        :param results:
-        :type results: List[int]
-        :param format:
-        :type format: FormatEnum
-        :param part_id:
-        :type part_id: str
-        :param validation_status:
-        :type validation_status: ValidationStatusEnum
+        :param inspection_request: (required)
+        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -320,93 +229,60 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_create_serialize(
-            team=team,
-            capture_datetime=capture_datetime,
-            file=file,
-            inspection=inspection,
-            uploaded_by=uploaded_by,
-            results=results,
-            format=format,
-            part_id=part_id,
-            validation_status=validation_status,
+        _param = self._inspection_create_serialize(
+            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Image",
+            '201': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_create_serialize(
+    def _inspection_create_serialize(
         self,
-        team,
-        capture_datetime,
-        file,
-        inspection,
-        uploaded_by,
-        results,
-        format,
-        part_id,
-        validation_status,
+        inspection_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'results': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
-        if team is not None:
-            _form_params.append(('team', team))
-        if inspection is not None:
-            _form_params.append(('inspection', inspection))
-        if uploaded_by is not None:
-            _form_params.append(('uploaded_by', uploaded_by))
-        if results is not None:
-            _form_params.append(('results', results))
-        if format is not None:
-            _form_params.append(('format', format))
-        if capture_datetime is not None:
-            _form_params.append(('capture_datetime', capture_datetime))
-        if file is not None:
-            _files['file'] = file
-        if part_id is not None:
-            _form_params.append(('part_id', part_id))
-        if validation_status is not None:
-            _form_params.append(('validation_status', validation_status))
         # process the body parameter
+        if inspection_request is not None:
+            _body_params = inspection_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -415,14 +291,16 @@
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
             _default_content_type = (
                 self.api_client.select_header_content_type(
                     [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
                         'multipart/form-data'
                     ]
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
@@ -430,15 +308,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/api/image/',
+            resource_path='/api/inspection/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -447,35 +325,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_destroy(
+    def inspection_destroy(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """image_destroy
+        """inspection_destroy
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -491,15 +369,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_destroy_serialize(
+        _param = self._inspection_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -514,35 +392,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_destroy_with_http_info(
+    def inspection_destroy_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """image_destroy
+        """inspection_destroy
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -558,15 +436,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_destroy_serialize(
+        _param = self._inspection_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -581,35 +459,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_destroy_without_preload_content(
+    def inspection_destroy_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_destroy
+        """inspection_destroy
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -625,15 +503,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_destroy_serialize(
+        _param = self._inspection_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -643,15 +521,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_destroy_serialize(
+    def _inspection_destroy_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -683,15 +561,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/api/image/{id}/',
+            resource_path='/api/inspection/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -700,36 +578,48 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_inspection_status_list(
+    def inspection_list(
         self,
+        fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[InspectionStatus]:
-        """image_inspection_status_list
+    ) -> PaginatedInspectionList:
+        """inspection_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param fields:
+        :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -744,59 +634,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_inspection_status_list_serialize(
+        _param = self._inspection_list_serialize(
+            fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionStatus]",
+            '200': "PaginatedInspectionList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_inspection_status_list_with_http_info(
+    def inspection_list_with_http_info(
         self,
+        fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[InspectionStatus]]:
-        """image_inspection_status_list
+    ) -> ApiResponse[PaginatedInspectionList]:
+        """inspection_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param fields:
+        :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -811,59 +717,75 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_inspection_status_list_serialize(
+        _param = self._inspection_list_serialize(
+            fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionStatus]",
+            '200': "PaginatedInspectionList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_inspection_status_list_without_preload_content(
+    def inspection_list_without_preload_content(
         self,
+        fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_inspection_status_list
+        """inspection_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param fields:
+        :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -878,35 +800,43 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_inspection_status_list_serialize(
+        _param = self._inspection_list_serialize(
+            fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionStatus]",
+            '200': "PaginatedInspectionList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_inspection_status_list_serialize(
+    def _inspection_list_serialize(
         self,
+        fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -920,18 +850,34 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if fields is not None:
+            
+            _query_params.append(('fields', fields))
+            
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -945,15 +891,304 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/image/inspection_status/',
+            resource_path='/api/inspection/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def inspection_partial_update(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        patched_inspection_request: Optional[PatchedInspectionRequest] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> Inspection:
+        """inspection_partial_update
+
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
+        :param patched_inspection_request:
+        :type patched_inspection_request: PatchedInspectionRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._inspection_partial_update_serialize(
+            id=id,
+            patched_inspection_request=patched_inspection_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Inspection",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def inspection_partial_update_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        patched_inspection_request: Optional[PatchedInspectionRequest] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[Inspection]:
+        """inspection_partial_update
+
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
+        :param patched_inspection_request:
+        :type patched_inspection_request: PatchedInspectionRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._inspection_partial_update_serialize(
+            id=id,
+            patched_inspection_request=patched_inspection_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Inspection",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def inspection_partial_update_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        patched_inspection_request: Optional[PatchedInspectionRequest] = None,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """inspection_partial_update
+
+        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
+        :param patched_inspection_request:
+        :type patched_inspection_request: PatchedInspectionRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._inspection_partial_update_serialize(
+            id=id,
+            patched_inspection_request=patched_inspection_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "Inspection",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _inspection_partial_update_serialize(
+        self,
+        id,
+        patched_inspection_request,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+        if patched_inspection_request is not None:
+            _body_params = patched_inspection_request
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='PATCH',
+            resource_path='/api/inspection/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -962,39 +1197,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_list(
+    def inspection_retrieve(
         self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         fields: Optional[StrictStr] = None,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Image]:
-        """image_list
+    ) -> Inspection:
+        """inspection_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
         :param fields:
         :type fields: str
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1009,63 +1244,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_list_serialize(
-            fields=fields,
+        _param = self._inspection_retrieve_serialize(
             id=id,
+            fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Image]",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_list_with_http_info(
+    def inspection_retrieve_with_http_info(
         self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         fields: Optional[StrictStr] = None,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Image]]:
-        """image_list
+    ) -> ApiResponse[Inspection]:
+        """inspection_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
         :param fields:
         :type fields: str
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1080,63 +1315,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_list_serialize(
-            fields=fields,
+        _param = self._inspection_retrieve_serialize(
             id=id,
+            fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Image]",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_list_without_preload_content(
+    def inspection_retrieve_without_preload_content(
         self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         fields: Optional[StrictStr] = None,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_list
+        """inspection_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
         :param fields:
         :type fields: str
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1151,66 +1386,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_list_serialize(
-            fields=fields,
+        _param = self._inspection_retrieve_serialize(
             id=id,
+            fields=fields,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Image]",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_list_serialize(
+    def _inspection_retrieve_serialize(
         self,
-        fields,
         id,
+        fields,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'id': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         if fields is not None:
             
             _query_params.append(('fields', fields))
             
-        if id is not None:
-            
-            _query_params.append(('id', id))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1224,15 +1456,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/image/',
+            resource_path='/api/inspection/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1241,39 +1473,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_partial_update(
+    def inspection_send_validation_email_retrieve(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        patched_image_request: Optional[PatchedImageRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Image:
-        """image_partial_update
+    ) -> Inspection:
+        """inspection_send_validation_email_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param patched_image_request:
-        :type patched_image_request: PatchedImageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1288,63 +1517,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_partial_update_serialize(
+        _param = self._inspection_send_validation_email_retrieve_serialize(
             id=id,
-            patched_image_request=patched_image_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_partial_update_with_http_info(
+    def inspection_send_validation_email_retrieve_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        patched_image_request: Optional[PatchedImageRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Image]:
-        """image_partial_update
+    ) -> ApiResponse[Inspection]:
+        """inspection_send_validation_email_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param patched_image_request:
-        :type patched_image_request: PatchedImageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1359,63 +1584,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_partial_update_serialize(
+        _param = self._inspection_send_validation_email_retrieve_serialize(
             id=id,
-            patched_image_request=patched_image_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_partial_update_without_preload_content(
+    def inspection_send_validation_email_retrieve_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        patched_image_request: Optional[PatchedImageRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_partial_update
+        """inspection_send_validation_email_retrieve
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param patched_image_request:
-        :type patched_image_request: PatchedImageRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1430,37 +1651,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_partial_update_serialize(
+        _param = self._inspection_send_validation_email_retrieve_serialize(
             id=id,
-            patched_image_request=patched_image_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_partial_update_serialize(
+    def _inspection_send_validation_email_retrieve_serialize(
         self,
         id,
-        patched_image_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1478,50 +1697,33 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if patched_image_request is not None:
-            _body_params = patched_image_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json', 
-                        'application/x-www-form-urlencoded', 
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/api/image/{id}/',
+            method='GET',
+            resource_path='/api/inspection/{id}/send_validation_email/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1530,36 +1732,45 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_quality_list(
+    def inspection_status_list(
         self,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[QualityCriteriaResult]:
-        """image_quality_list
+    ) -> PaginatedInspectionStatusList:
+        """inspection_status_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1574,59 +1785,71 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_quality_list_serialize(
+        _param = self._inspection_status_list_serialize(
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[QualityCriteriaResult]",
+            '200': "PaginatedInspectionStatusList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_quality_list_with_http_info(
+    def inspection_status_list_with_http_info(
         self,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[QualityCriteriaResult]]:
-        """image_quality_list
+    ) -> ApiResponse[PaginatedInspectionStatusList]:
+        """inspection_status_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1641,59 +1864,71 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_quality_list_serialize(
+        _param = self._inspection_status_list_serialize(
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[QualityCriteriaResult]",
+            '200': "PaginatedInspectionStatusList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_quality_list_without_preload_content(
+    def inspection_status_list_without_preload_content(
         self,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_quality_list
+        """inspection_status_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1708,35 +1943,41 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_quality_list_serialize(
+        _param = self._inspection_status_list_serialize(
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[QualityCriteriaResult]",
+            '200': "PaginatedInspectionStatusList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_quality_list_serialize(
+    def _inspection_status_list_serialize(
         self,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1754,14 +1995,26 @@
 
         # process the path parameters
         # process the query parameters
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1775,15 +2028,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/image/quality/',
+            resource_path='/api/inspection/status/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1792,39 +2045,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_retrieve(
+    def inspection_update(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        fields: Optional[StrictStr] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Image:
-        """image_retrieve
+    ) -> Inspection:
+        """inspection_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param fields:
-        :type fields: str
+        :param inspection_request: (required)
+        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1839,63 +2092,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_retrieve_serialize(
+        _param = self._inspection_update_serialize(
             id=id,
-            fields=fields,
+            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_retrieve_with_http_info(
+    def inspection_update_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        fields: Optional[StrictStr] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Image]:
-        """image_retrieve
+    ) -> ApiResponse[Inspection]:
+        """inspection_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param fields:
-        :type fields: str
+        :param inspection_request: (required)
+        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1910,63 +2163,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_retrieve_serialize(
+        _param = self._inspection_update_serialize(
             id=id,
-            fields=fields,
+            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_retrieve_without_preload_content(
+    def inspection_update_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        fields: Optional[StrictStr] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_retrieve
+        """inspection_update
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
+        :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param fields:
-        :type fields: str
+        :param inspection_request: (required)
+        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1981,37 +2234,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_retrieve_serialize(
+        _param = self._inspection_update_serialize(
             id=id,
-            fields=fields,
+            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "Inspection",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_retrieve_serialize(
+    def _inspection_update_serialize(
         self,
         id,
-        fields,
+        inspection_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -2026,40 +2279,53 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
-        if fields is not None:
-            
-            _query_params.append(('fields', fields))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if inspection_request is not None:
+            _body_params = inspection_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/image/{id}/',
+            method='PUT',
+            resource_path='/api/inspection/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2068,39 +2334,45 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def image_update(
+    def inspection_validation_status_list(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        image_request: ImageRequest,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Image:
-        """image_update
+    ) -> PaginatedInspectionValidationStatusList:
+        """inspection_validation_status_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
-        :type id: int
-        :param image_request: (required)
-        :type image_request: ImageRequest
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2115,63 +2387,71 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_update_serialize(
+        _param = self._inspection_validation_status_list_serialize(
             id=id,
-            image_request=image_request,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "PaginatedInspectionValidationStatusList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def image_update_with_http_info(
+    def inspection_validation_status_list_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        image_request: ImageRequest,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Image]:
-        """image_update
+    ) -> ApiResponse[PaginatedInspectionValidationStatusList]:
+        """inspection_validation_status_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
-        :type id: int
-        :param image_request: (required)
-        :type image_request: ImageRequest
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2186,63 +2466,71 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_update_serialize(
+        _param = self._inspection_validation_status_list_serialize(
             id=id,
-            image_request=image_request,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "PaginatedInspectionValidationStatusList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def image_update_without_preload_content(
+    def inspection_validation_status_list_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
-        image_request: ImageRequest,
+        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """image_update
+        """inspection_validation_status_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
-        :param id: A unique integer value identifying this image. (required)
-        :type id: int
-        :param image_request: (required)
-        :type image_request: ImageRequest
+        :param id: Multiple values may be separated by commas.
+        :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2257,98 +2545,100 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._image_update_serialize(
+        _param = self._inspection_validation_status_list_serialize(
             id=id,
-            image_request=image_request,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Image",
+            '200': "PaginatedInspectionValidationStatusList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _image_update_serialize(
+    def _inspection_validation_status_list_serialize(
         self,
         id,
-        image_request,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
+            'id': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
         # process the query parameters
+        if id is not None:
+            
+            _query_params.append(('id', id))
+            
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if image_request is not None:
-            _body_params = image_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json', 
-                        'application/x-www-form-urlencoded', 
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/api/image/{id}/',
+            method='GET',
+            resource_path='/api/inspection/validation_status/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `avis_client-0.6.0/avis_client/api/image_attribute_api.py` & `avis_client-0.7.0/avis_client/api/image_attribute_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -27,14 +27,15 @@
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from avis_client.models.image_attribute import ImageAttribute
 from avis_client.models.image_attribute_request import ImageAttributeRequest
+from avis_client.models.paginated_image_attribute_list import PaginatedImageAttributeList
 from avis_client.models.patched_image_attribute_request import PatchedImageAttributeRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def image_attribute_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ImageAttribute]:
+    ) -> PaginatedImageAttributeList:
         """image_attribute_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._image_attribute_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ImageAttribute]",
+            '200': "PaginatedImageAttributeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def image_attribute_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ImageAttribute]]:
+    ) -> ApiResponse[PaginatedImageAttributeList]:
         """image_attribute_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._image_attribute_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ImageAttribute]",
+            '200': "PaginatedImageAttributeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def image_attribute_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._image_attribute_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ImageAttribute]",
+            '200': "PaginatedImageAttributeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _image_attribute_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/image_attribute_category_api.py` & `avis_client-0.7.0/avis_client/api/image_attribute_category_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -27,14 +27,15 @@
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from avis_client.models.image_attribute_category import ImageAttributeCategory
 from avis_client.models.image_attribute_category_request import ImageAttributeCategoryRequest
+from avis_client.models.paginated_image_attribute_category_list import PaginatedImageAttributeCategoryList
 from avis_client.models.patched_image_attribute_category_request import PatchedImageAttributeCategoryRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def image_attribute_category_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ImageAttributeCategory]:
+    ) -> PaginatedImageAttributeCategoryList:
         """image_attribute_category_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._image_attribute_category_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ImageAttributeCategory]",
+            '200': "PaginatedImageAttributeCategoryList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def image_attribute_category_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ImageAttributeCategory]]:
+    ) -> ApiResponse[PaginatedImageAttributeCategoryList]:
         """image_attribute_category_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._image_attribute_category_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ImageAttributeCategory]",
+            '200': "PaginatedImageAttributeCategoryList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def image_attribute_category_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._image_attribute_category_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ImageAttributeCategory]",
+            '200': "PaginatedImageAttributeCategoryList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _image_attribute_category_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/inspection_api.py` & `avis_client-0.7.0/avis_client/api/statistics_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -21,65 +21,66 @@
 try:
     from typing import Annotated
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictInt
 
-from typing import List, Optional
+from typing import Optional
 
-from avis_client.models.inspection import Inspection
-from avis_client.models.inspection_request import InspectionRequest
-from avis_client.models.inspection_status import InspectionStatus
-from avis_client.models.inspection_validation_status import InspectionValidationStatus
-from avis_client.models.patched_inspection_request import PatchedInspectionRequest
+from avis_client.models.inspection_images_statistics import InspectionImagesStatistics
+from avis_client.models.inspection_images_statistics_request import InspectionImagesStatisticsRequest
+from avis_client.models.inspection_statistics import InspectionStatistics
+from avis_client.models.inspection_statistics_request import InspectionStatisticsRequest
+from avis_client.models.paginated_inspection_images_statistics_list import PaginatedInspectionImagesStatisticsList
+from avis_client.models.paginated_inspection_statistics_list import PaginatedInspectionStatisticsList
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
-class InspectionApi:
+class StatisticsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def inspection_create(
+    def statistics_inspection_create(
         self,
-        inspection_request: InspectionRequest,
+        inspection_images_statistics_request: InspectionImagesStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Inspection:
-        """inspection_create
+    ) -> InspectionImagesStatistics:
+        """statistics_inspection_create
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param inspection_request: (required)
-        :type inspection_request: InspectionRequest
+        :param inspection_images_statistics_request: (required)
+        :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -94,59 +95,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_create_serialize(
-            inspection_request=inspection_request,
+        _param = self._statistics_inspection_create_serialize(
+            inspection_images_statistics_request=inspection_images_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Inspection",
+            '201': "InspectionImagesStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_create_with_http_info(
+    def statistics_inspection_create_with_http_info(
         self,
-        inspection_request: InspectionRequest,
+        inspection_images_statistics_request: InspectionImagesStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Inspection]:
-        """inspection_create
+    ) -> ApiResponse[InspectionImagesStatistics]:
+        """statistics_inspection_create
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param inspection_request: (required)
-        :type inspection_request: InspectionRequest
+        :param inspection_images_statistics_request: (required)
+        :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -161,59 +162,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_create_serialize(
-            inspection_request=inspection_request,
+        _param = self._statistics_inspection_create_serialize(
+            inspection_images_statistics_request=inspection_images_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Inspection",
+            '201': "InspectionImagesStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_create_without_preload_content(
+    def statistics_inspection_create_without_preload_content(
         self,
-        inspection_request: InspectionRequest,
+        inspection_images_statistics_request: InspectionImagesStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_create
+        """statistics_inspection_create
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param inspection_request: (required)
-        :type inspection_request: InspectionRequest
+        :param inspection_images_statistics_request: (required)
+        :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -228,35 +229,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_create_serialize(
-            inspection_request=inspection_request,
+        _param = self._statistics_inspection_create_serialize(
+            inspection_images_statistics_request=inspection_images_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "Inspection",
+            '201': "InspectionImagesStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_create_serialize(
+    def _statistics_inspection_create_serialize(
         self,
-        inspection_request,
+        inspection_images_statistics_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -272,16 +273,16 @@
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if inspection_request is not None:
-            _body_params = inspection_request
+        if inspection_images_statistics_request is not None:
+            _body_params = inspection_images_statistics_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -307,15 +308,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/api/inspection/',
+            resource_path='/api/statistics/inspection/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -324,35 +325,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_destroy(
+    def statistics_inspection_destroy(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """inspection_destroy
+        """statistics_inspection_destroy
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
+        :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -368,15 +369,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_destroy_serialize(
+        _param = self._statistics_inspection_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -391,35 +392,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_destroy_with_http_info(
+    def statistics_inspection_destroy_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """inspection_destroy
+        """statistics_inspection_destroy
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
+        :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -435,15 +436,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_destroy_serialize(
+        _param = self._statistics_inspection_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -458,35 +459,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_destroy_without_preload_content(
+    def statistics_inspection_destroy_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_destroy
+        """statistics_inspection_destroy
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
+        :param id: A unique integer value identifying this image. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
@@ -502,15 +503,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_destroy_serialize(
+        _param = self._statistics_inspection_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -520,15 +521,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_destroy_serialize(
+    def _statistics_inspection_destroy_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -560,15 +561,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/api/inspection/{id}/',
+            resource_path='/api/statistics/inspection/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -577,39 +578,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_list(
+    def statistics_inspection_list(
         self,
-        fields: Optional[StrictStr] = None,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Inspection]:
-        """inspection_list
+    ) -> PaginatedInspectionImagesStatisticsList:
+        """statistics_inspection_list
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param fields:
-        :type fields: str
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -624,63 +625,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_list_serialize(
-            fields=fields,
-            id=id,
+        _param = self._statistics_inspection_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Inspection]",
+            '200': "PaginatedInspectionImagesStatisticsList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_list_with_http_info(
+    def statistics_inspection_list_with_http_info(
         self,
-        fields: Optional[StrictStr] = None,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Inspection]]:
-        """inspection_list
+    ) -> ApiResponse[PaginatedInspectionImagesStatisticsList]:
+        """statistics_inspection_list
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param fields:
-        :type fields: str
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -695,63 +696,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_list_serialize(
-            fields=fields,
-            id=id,
+        _param = self._statistics_inspection_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Inspection]",
+            '200': "PaginatedInspectionImagesStatisticsList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_list_without_preload_content(
+    def statistics_inspection_list_without_preload_content(
         self,
-        fields: Optional[StrictStr] = None,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_list
+        """statistics_inspection_list
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param fields:
-        :type fields: str
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -766,65 +767,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_list_serialize(
-            fields=fields,
-            id=id,
+        _param = self._statistics_inspection_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Inspection]",
+            '200': "PaginatedInspectionImagesStatisticsList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_list_serialize(
+    def _statistics_inspection_list_serialize(
         self,
-        fields,
-        id,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'id': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if fields is not None:
+        if page is not None:
             
-            _query_params.append(('fields', fields))
+            _query_params.append(('page', page))
             
-        if id is not None:
+        if page_size is not None:
             
-            _query_params.append(('id', id))
+            _query_params.append(('page_size', page_size))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -839,15 +839,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/inspection/',
+            resource_path='/api/statistics/inspection/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -856,39 +856,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_partial_update(
+    def statistics_inspection_retrieve(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        patched_inspection_request: Optional[PatchedInspectionRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Inspection:
-        """inspection_partial_update
+    ) -> InspectionImagesStatistics:
+        """statistics_inspection_retrieve
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
+        :param id: A unique integer value identifying this image. (required)
         :type id: int
-        :param patched_inspection_request:
-        :type patched_inspection_request: PatchedInspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -903,63 +900,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_partial_update_serialize(
+        _param = self._statistics_inspection_retrieve_serialize(
             id=id,
-            patched_inspection_request=patched_inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '200': "InspectionImagesStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_partial_update_with_http_info(
+    def statistics_inspection_retrieve_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        patched_inspection_request: Optional[PatchedInspectionRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Inspection]:
-        """inspection_partial_update
+    ) -> ApiResponse[InspectionImagesStatistics]:
+        """statistics_inspection_retrieve
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
+        :param id: A unique integer value identifying this image. (required)
         :type id: int
-        :param patched_inspection_request:
-        :type patched_inspection_request: PatchedInspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -974,63 +967,258 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_partial_update_serialize(
+        _param = self._statistics_inspection_retrieve_serialize(
             id=id,
-            patched_inspection_request=patched_inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '200': "InspectionImagesStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_partial_update_without_preload_content(
+    def statistics_inspection_retrieve_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        patched_inspection_request: Optional[PatchedInspectionRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_partial_update
+        """statistics_inspection_retrieve
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
+        :param id: A unique integer value identifying this image. (required)
+        :type id: int
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_inspection_retrieve_serialize(
+            id=id,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "InspectionImagesStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        return response_data.response
+
+
+    def _statistics_inspection_retrieve_serialize(
+        self,
+        id,
+        _request_auth,
+        _content_type,
+        _headers,
+        _host_index,
+    ) -> Tuple:
+
+        _host = None
+
+        _collection_formats: Dict[str, str] = {
+        }
+
+        _path_params: Dict[str, str] = {}
+        _query_params: List[Tuple[str, str]] = []
+        _header_params: Dict[str, Optional[str]] = _headers or {}
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        _body_params: Optional[bytes] = None
+
+        # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
+        # process the query parameters
+        # process the header parameters
+        # process the form parameters
+        # process the body parameter
+
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
+
+
+        # authentication setting
+        _auth_settings: List[str] = [
+            'cookieAuth', 
+            'ApiKeyAuth'
+        ]
+
+        return self.api_client.param_serialize(
+            method='GET',
+            resource_path='/api/statistics/inspection/{id}/',
+            path_params=_path_params,
+            query_params=_query_params,
+            header_params=_header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            auth_settings=_auth_settings,
+            collection_formats=_collection_formats,
+            _host=_host,
+            _request_auth=_request_auth
+        )
+
+
+
+
+    @validate_call
+    def statistics_inspection_update(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
+        inspection_images_statistics_request: InspectionImagesStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> InspectionImagesStatistics:
+        """statistics_inspection_update
+
+        Allows a Google Partial Response query param like to prune results
+
+        :param id: A unique integer value identifying this image. (required)
+        :type id: int
+        :param inspection_images_statistics_request: (required)
+        :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_inspection_update_serialize(
+            id=id,
+            inspection_images_statistics_request=inspection_images_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "InspectionImagesStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        ).data
+
+
+    @validate_call
+    def statistics_inspection_update_with_http_info(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
+        inspection_images_statistics_request: InspectionImagesStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> ApiResponse[InspectionImagesStatistics]:
+        """statistics_inspection_update
+
+        Allows a Google Partial Response query param like to prune results
+
+        :param id: A unique integer value identifying this image. (required)
         :type id: int
-        :param patched_inspection_request:
-        :type patched_inspection_request: PatchedInspectionRequest
+        :param inspection_images_statistics_request: (required)
+        :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1045,37 +1233,108 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_partial_update_serialize(
+        _param = self._statistics_inspection_update_serialize(
             id=id,
-            patched_inspection_request=patched_inspection_request,
+            inspection_images_statistics_request=inspection_images_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '200': "InspectionImagesStatistics",
+        }
+        response_data = self.api_client.call_api(
+            *_param,
+            _request_timeout=_request_timeout
+        )
+        response_data.read()
+        return self.api_client.response_deserialize(
+            response_data=response_data,
+            response_types_map=_response_types_map,
+        )
+
+
+    @validate_call
+    def statistics_inspection_update_without_preload_content(
+        self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this image.")],
+        inspection_images_statistics_request: InspectionImagesStatisticsRequest,
+        _request_timeout: Union[
+            None,
+            Annotated[StrictFloat, Field(gt=0)],
+            Tuple[
+                Annotated[StrictFloat, Field(gt=0)],
+                Annotated[StrictFloat, Field(gt=0)]
+            ]
+        ] = None,
+        _request_auth: Optional[Dict[StrictStr, Any]] = None,
+        _content_type: Optional[StrictStr] = None,
+        _headers: Optional[Dict[StrictStr, Any]] = None,
+        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
+    ) -> RESTResponseType:
+        """statistics_inspection_update
+
+        Allows a Google Partial Response query param like to prune results
+
+        :param id: A unique integer value identifying this image. (required)
+        :type id: int
+        :param inspection_images_statistics_request: (required)
+        :type inspection_images_statistics_request: InspectionImagesStatisticsRequest
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :type _request_timeout: int, tuple(int, int), optional
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the
+                              authentication in the spec for a single request.
+        :type _request_auth: dict, optional
+        :param _content_type: force content-type for the request.
+        :type _content_type: str, Optional
+        :param _headers: set to override the headers for a single
+                         request; this effectively ignores the headers
+                         in the spec for a single request.
+        :type _headers: dict, optional
+        :param _host_index: set to override the host_index for a single
+                            request; this effectively ignores the host_index
+                            in the spec for a single request.
+        :type _host_index: int, optional
+        :return: Returns the result object.
+        """ # noqa: E501
+
+        _param = self._statistics_inspection_update_serialize(
+            id=id,
+            inspection_images_statistics_request=inspection_images_statistics_request,
+            _request_auth=_request_auth,
+            _content_type=_content_type,
+            _headers=_headers,
+            _host_index=_host_index
+        )
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "InspectionImagesStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_partial_update_serialize(
+    def _statistics_inspection_update_serialize(
         self,
         id,
-        patched_inspection_request,
+        inspection_images_statistics_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1093,16 +1352,16 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if patched_inspection_request is not None:
-            _body_params = patched_inspection_request
+        if inspection_images_statistics_request is not None:
+            _body_params = inspection_images_statistics_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1127,16 +1386,16 @@
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/api/inspection/{id}/',
+            method='PUT',
+            resource_path='/api/statistics/inspection/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1145,39 +1404,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_retrieve(
+    def statistics_team_create(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        fields: Optional[StrictStr] = None,
+        inspection_statistics_request: InspectionStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Inspection:
-        """inspection_retrieve
+    ) -> InspectionStatistics:
+        """statistics_team_create
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
-        :type id: int
-        :param fields:
-        :type fields: str
+        :param inspection_statistics_request: (required)
+        :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1192,63 +1448,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_retrieve_serialize(
-            id=id,
-            fields=fields,
+        _param = self._statistics_team_create_serialize(
+            inspection_statistics_request=inspection_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '201': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_retrieve_with_http_info(
+    def statistics_team_create_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        fields: Optional[StrictStr] = None,
+        inspection_statistics_request: InspectionStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Inspection]:
-        """inspection_retrieve
+    ) -> ApiResponse[InspectionStatistics]:
+        """statistics_team_create
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
-        :type id: int
-        :param fields:
-        :type fields: str
+        :param inspection_statistics_request: (required)
+        :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1263,63 +1515,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_retrieve_serialize(
-            id=id,
-            fields=fields,
+        _param = self._statistics_team_create_serialize(
+            inspection_statistics_request=inspection_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '201': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_retrieve_without_preload_content(
+    def statistics_team_create_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        fields: Optional[StrictStr] = None,
+        inspection_statistics_request: InspectionStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_retrieve
+        """statistics_team_create
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: A unique integer value identifying this inspection. (required)
-        :type id: int
-        :param fields:
-        :type fields: str
+        :param inspection_statistics_request: (required)
+        :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1334,37 +1582,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_retrieve_serialize(
-            id=id,
-            fields=fields,
+        _param = self._statistics_team_create_serialize(
+            inspection_statistics_request=inspection_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '201': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_retrieve_serialize(
+    def _statistics_team_create_serialize(
         self,
-        id,
-        fields,
+        inspection_statistics_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1376,43 +1622,54 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
         # process the query parameters
-        if fields is not None:
-            
-            _query_params.append(('fields', fields))
-            
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if inspection_statistics_request is not None:
+            _body_params = inspection_statistics_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/inspection/{id}/',
+            method='POST',
+            resource_path='/api/statistics/team/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1421,33 +1678,33 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_send_validation_email_retrieve(
+    def statistics_team_destroy(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Inspection:
-        """inspection_send_validation_email_retrieve
+    ) -> None:
+        """statistics_team_destroy
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1465,56 +1722,56 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_send_validation_email_retrieve_serialize(
+        _param = self._statistics_team_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_send_validation_email_retrieve_with_http_info(
+    def statistics_team_destroy_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Inspection]:
-        """inspection_send_validation_email_retrieve
+    ) -> ApiResponse[None]:
+        """statistics_team_destroy
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1532,38 +1789,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_send_validation_email_retrieve_serialize(
+        _param = self._statistics_team_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_send_validation_email_retrieve_without_preload_content(
+    def statistics_team_destroy_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -1571,17 +1828,17 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_send_validation_email_retrieve
+        """statistics_team_destroy
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1599,33 +1856,33 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_send_validation_email_retrieve_serialize(
+        _param = self._statistics_team_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_send_validation_email_retrieve_serialize(
+    def _statistics_team_destroy_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -1647,31 +1904,25 @@
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/inspection/{id}/send_validation_email/',
+            method='DELETE',
+            resource_path='/api/statistics/team/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1680,36 +1931,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_status_list(
+    def statistics_team_list(
         self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[InspectionStatus]:
-        """inspection_status_list
+    ) -> PaginatedInspectionStatisticsList:
+        """statistics_team_list
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1724,59 +1978,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_status_list_serialize(
-            id=id,
+        _param = self._statistics_team_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionStatus]",
+            '200': "PaginatedInspectionStatisticsList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_status_list_with_http_info(
+    def statistics_team_list_with_http_info(
         self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[InspectionStatus]]:
-        """inspection_status_list
+    ) -> ApiResponse[PaginatedInspectionStatisticsList]:
+        """statistics_team_list
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1791,59 +2049,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_status_list_serialize(
-            id=id,
+        _param = self._statistics_team_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionStatus]",
+            '200': "PaginatedInspectionStatisticsList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_status_list_without_preload_content(
+    def statistics_team_list_without_preload_content(
         self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_status_list
+        """statistics_team_list
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1858,59 +2120,64 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_status_list_serialize(
-            id=id,
+        _param = self._statistics_team_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionStatus]",
+            '200': "PaginatedInspectionStatisticsList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_status_list_serialize(
+    def _statistics_team_list_serialize(
         self,
-        id,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'id': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if id is not None:
+        if page is not None:
+            
+            _query_params.append(('page', page))
             
-            _query_params.append(('id', id))
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
@@ -1925,15 +2192,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/inspection/status/',
+            resource_path='/api/statistics/team/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1942,39 +2209,36 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_update(
+    def statistics_team_retrieve(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> Inspection:
-        """inspection_update
+    ) -> InspectionStatistics:
+        """statistics_team_retrieve
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param inspection_request: (required)
-        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1989,63 +2253,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_update_serialize(
+        _param = self._statistics_team_retrieve_serialize(
             id=id,
-            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '200': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_update_with_http_info(
+    def statistics_team_retrieve_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[Inspection]:
-        """inspection_update
+    ) -> ApiResponse[InspectionStatistics]:
+        """statistics_team_retrieve
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param inspection_request: (required)
-        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2060,63 +2320,59 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_update_serialize(
+        _param = self._statistics_team_retrieve_serialize(
             id=id,
-            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '200': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_update_without_preload_content(
+    def statistics_team_retrieve_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
-        inspection_request: InspectionRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_update
+        """statistics_team_retrieve
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
         :param id: A unique integer value identifying this inspection. (required)
         :type id: int
-        :param inspection_request: (required)
-        :type inspection_request: InspectionRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2131,37 +2387,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_update_serialize(
+        _param = self._statistics_team_retrieve_serialize(
             id=id,
-            inspection_request=inspection_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "Inspection",
+            '200': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_update_serialize(
+    def _statistics_team_retrieve_serialize(
         self,
         id,
-        inspection_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -2179,50 +2433,33 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if inspection_request is not None:
-            _body_params = inspection_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json', 
-                        'application/x-www-form-urlencoded', 
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/api/inspection/{id}/',
+            method='GET',
+            resource_path='/api/statistics/team/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2231,36 +2468,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def inspection_validation_status_list(
+    def statistics_team_update(
         self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        inspection_statistics_request: InspectionStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[InspectionValidationStatus]:
-        """inspection_validation_status_list
+    ) -> InspectionStatistics:
+        """statistics_team_update
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
+        :param inspection_statistics_request: (required)
+        :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2275,59 +2515,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_validation_status_list_serialize(
+        _param = self._statistics_team_update_serialize(
             id=id,
+            inspection_statistics_request=inspection_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionValidationStatus]",
+            '200': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def inspection_validation_status_list_with_http_info(
+    def statistics_team_update_with_http_info(
         self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        inspection_statistics_request: InspectionStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[InspectionValidationStatus]]:
-        """inspection_validation_status_list
+    ) -> ApiResponse[InspectionStatistics]:
+        """statistics_team_update
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
+        :param inspection_statistics_request: (required)
+        :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2342,59 +2586,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_validation_status_list_serialize(
+        _param = self._statistics_team_update_serialize(
             id=id,
+            inspection_statistics_request=inspection_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionValidationStatus]",
+            '200': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def inspection_validation_status_list_without_preload_content(
+    def statistics_team_update_without_preload_content(
         self,
-        id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this inspection.")],
+        inspection_statistics_request: InspectionStatisticsRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """inspection_validation_status_list
+        """statistics_team_update
 
-        A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
+        Allows a Google Partial Response query param like to prune results
 
-        :param id: Multiple values may be separated by commas.
-        :type id: List[int]
+        :param id: A unique integer value identifying this inspection. (required)
+        :type id: int
+        :param inspection_statistics_request: (required)
+        :type inspection_statistics_request: InspectionStatisticsRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2409,82 +2657,98 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._inspection_validation_status_list_serialize(
+        _param = self._statistics_team_update_serialize(
             id=id,
+            inspection_statistics_request=inspection_statistics_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[InspectionValidationStatus]",
+            '200': "InspectionStatistics",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _inspection_validation_status_list_serialize(
+    def _statistics_team_update_serialize(
         self,
         id,
+        inspection_statistics_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
 
         _collection_formats: Dict[str, str] = {
-            'id': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        # process the query parameters
         if id is not None:
-            
-            _query_params.append(('id', id))
-            
+            _path_params['id'] = id
+        # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if inspection_statistics_request is not None:
+            _body_params = inspection_statistics_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/inspection/validation_status/',
+            method='PUT',
+            resource_path='/api/statistics/team/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `avis_client-0.6.0/avis_client/api/membership_api.py` & `avis_client-0.7.0/avis_client/api/membership_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -23,18 +23,19 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt
 
-from typing import List
+from typing import Optional
 
 from avis_client.models.membership import Membership
 from avis_client.models.membership_request import MembershipRequest
+from avis_client.models.paginated_membership_list import PaginatedMembershipList
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
 class MembershipApi:
@@ -576,31 +577,37 @@
 
 
 
 
     @validate_call
     def membership_list(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Membership]:
+    ) -> PaginatedMembershipList:
         """membership_list
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -616,22 +623,24 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._membership_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Membership]",
+            '200': "PaginatedMembershipList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -639,31 +648,37 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def membership_list_with_http_info(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Membership]]:
+    ) -> ApiResponse[PaginatedMembershipList]:
         """membership_list
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -679,22 +694,24 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._membership_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Membership]",
+            '200': "PaginatedMembershipList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -702,14 +719,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def membership_list_without_preload_content(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -719,14 +738,18 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """membership_list
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -742,32 +765,36 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._membership_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Membership]",
+            '200': "PaginatedMembershipList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _membership_list_serialize(
         self,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -780,14 +807,22 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/metadata_api.py` & `avis_client-0.7.0/avis_client/api/metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -27,14 +27,15 @@
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from avis_client.models.metadata import Metadata
 from avis_client.models.metadata_request import MetadataRequest
+from avis_client.models.paginated_metadata_list import PaginatedMetadataList
 from avis_client.models.patched_metadata_request import PatchedMetadataRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def metadata_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Metadata]:
+    ) -> PaginatedMetadataList:
         """metadata_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._metadata_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Metadata]",
+            '200': "PaginatedMetadataList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def metadata_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Metadata]]:
+    ) -> ApiResponse[PaginatedMetadataList]:
         """metadata_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._metadata_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Metadata]",
+            '200': "PaginatedMetadataList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def metadata_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._metadata_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Metadata]",
+            '200': "PaginatedMetadataList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _metadata_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/metadata_schema_api.py` & `avis_client-0.7.0/avis_client/api/metadata_schema_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -27,14 +27,15 @@
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from avis_client.models.metadata_schema import MetadataSchema
 from avis_client.models.metadata_schema_request import MetadataSchemaRequest
+from avis_client.models.paginated_metadata_schema_list import PaginatedMetadataSchemaList
 from avis_client.models.patched_metadata_schema_request import PatchedMetadataSchemaRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def metadata_schema_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[MetadataSchema]:
+    ) -> PaginatedMetadataSchemaList:
         """metadata_schema_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._metadata_schema_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MetadataSchema]",
+            '200': "PaginatedMetadataSchemaList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def metadata_schema_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[MetadataSchema]]:
+    ) -> ApiResponse[PaginatedMetadataSchemaList]:
         """metadata_schema_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._metadata_schema_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MetadataSchema]",
+            '200': "PaginatedMetadataSchemaList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def metadata_schema_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._metadata_schema_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MetadataSchema]",
+            '200': "PaginatedMetadataSchemaList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _metadata_schema_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/ml_api.py` & `avis_client-0.7.0/avis_client/api/ml_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -23,21 +23,23 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt
 
-from typing import List, Optional
+from typing import Optional
 
 from avis_client.models.azure_ml_inference_request import AzureMLInferenceRequest
 from avis_client.models.ml_model import MLModel
 from avis_client.models.ml_model_request import MLModelRequest
 from avis_client.models.ml_model_type import MLModelType
 from avis_client.models.ml_model_type_request import MLModelTypeRequest
+from avis_client.models.paginated_ml_model_list import PaginatedMLModelList
+from avis_client.models.paginated_ml_model_type_list import PaginatedMLModelTypeList
 from avis_client.models.patched_ml_model_request import PatchedMLModelRequest
 from avis_client.models.patched_ml_model_type_request import PatchedMLModelTypeRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
@@ -851,15 +853,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/api/ml/model/{id}/inference/',
+            resource_path='/api/ml/model/{id}/infer/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -870,31 +872,37 @@
 
 
 
 
     @validate_call
     def ml_model_list(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[MLModel]:
+    ) -> PaginatedMLModelList:
         """ml_model_list
 
         A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -910,22 +918,24 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._ml_model_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MLModel]",
+            '200': "PaginatedMLModelList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -933,31 +943,37 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def ml_model_list_with_http_info(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[MLModel]]:
+    ) -> ApiResponse[PaginatedMLModelList]:
         """ml_model_list
 
         A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -973,22 +989,24 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._ml_model_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MLModel]",
+            '200': "PaginatedMLModelList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -996,14 +1014,16 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def ml_model_list_without_preload_content(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -1013,14 +1033,18 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """ml_model_list
 
         A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1036,32 +1060,36 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._ml_model_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MLModel]",
+            '200': "PaginatedMLModelList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _ml_model_list_serialize(
         self,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1074,14 +1102,22 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1660,39 +1696,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_model_update(
+    def ml_model_type_create(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model.")],
-        ml_model_request: MLModelRequest,
+        ml_model_type_request: Optional[MLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MLModel:
-        """ml_model_update
+    ) -> MLModelType:
+        """ml_model_type_create
 
-        A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
-        :param id: A unique integer value identifying this ml model. (required)
-        :type id: int
-        :param ml_model_request: (required)
-        :type ml_model_request: MLModelRequest
+        :param ml_model_type_request:
+        :type ml_model_type_request: MLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1707,63 +1739,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_model_update_serialize(
-            id=id,
-            ml_model_request=ml_model_request,
+        _param = self._ml_model_type_create_serialize(
+            ml_model_type_request=ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MLModel",
+            '201': "MLModelType",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_model_update_with_http_info(
+    def ml_model_type_create_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model.")],
-        ml_model_request: MLModelRequest,
+        ml_model_type_request: Optional[MLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MLModel]:
-        """ml_model_update
+    ) -> ApiResponse[MLModelType]:
+        """ml_model_type_create
 
-        A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
-        :param id: A unique integer value identifying this ml model. (required)
-        :type id: int
-        :param ml_model_request: (required)
-        :type ml_model_request: MLModelRequest
+        :param ml_model_type_request:
+        :type ml_model_type_request: MLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1778,63 +1805,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_model_update_serialize(
-            id=id,
-            ml_model_request=ml_model_request,
+        _param = self._ml_model_type_create_serialize(
+            ml_model_type_request=ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MLModel",
+            '201': "MLModelType",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_model_update_without_preload_content(
+    def ml_model_type_create_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model.")],
-        ml_model_request: MLModelRequest,
+        ml_model_type_request: Optional[MLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_model_update
+        """ml_model_type_create
 
-        A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
-        :param id: A unique integer value identifying this ml model. (required)
-        :type id: int
-        :param ml_model_request: (required)
-        :type ml_model_request: MLModelRequest
+        :param ml_model_type_request:
+        :type ml_model_type_request: MLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1849,37 +1871,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_model_update_serialize(
-            id=id,
-            ml_model_request=ml_model_request,
+        _param = self._ml_model_type_create_serialize(
+            ml_model_type_request=ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MLModel",
+            '201': "MLModelType",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_model_update_serialize(
+    def _ml_model_type_create_serialize(
         self,
-        id,
-        ml_model_request,
+        ml_model_type_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1891,22 +1911,20 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if ml_model_request is not None:
-            _body_params = ml_model_request
+        if ml_model_type_request is not None:
+            _body_params = ml_model_type_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -1931,16 +1949,16 @@
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/api/ml/model/{id}/',
+            method='POST',
+            resource_path='/api/ml/model-type/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1949,35 +1967,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_modeltype_create(
+    def ml_model_type_destroy(
         self,
-        ml_model_type_request: Optional[MLModelTypeRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MLModelType:
-        """ml_modeltype_create
+    ) -> None:
+        """ml_model_type_destroy
 
 
-        :param ml_model_type_request:
-        :type ml_model_type_request: MLModelTypeRequest
+        :param id: A unique integer value identifying this ml model type. (required)
+        :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1992,58 +2010,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_create_serialize(
-            ml_model_type_request=ml_model_type_request,
+        _param = self._ml_model_type_destroy_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "MLModelType",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_modeltype_create_with_http_info(
+    def ml_model_type_destroy_with_http_info(
         self,
-        ml_model_type_request: Optional[MLModelTypeRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MLModelType]:
-        """ml_modeltype_create
+    ) -> ApiResponse[None]:
+        """ml_model_type_destroy
 
 
-        :param ml_model_type_request:
-        :type ml_model_type_request: MLModelTypeRequest
+        :param id: A unique integer value identifying this ml model type. (required)
+        :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2058,58 +2076,58 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_create_serialize(
-            ml_model_type_request=ml_model_type_request,
+        _param = self._ml_model_type_destroy_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "MLModelType",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_modeltype_create_without_preload_content(
+    def ml_model_type_destroy_without_preload_content(
         self,
-        ml_model_type_request: Optional[MLModelTypeRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_modeltype_create
+        """ml_model_type_destroy
 
 
-        :param ml_model_type_request:
-        :type ml_model_type_request: MLModelTypeRequest
+        :param id: A unique integer value identifying this ml model type. (required)
+        :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2124,35 +2142,35 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_create_serialize(
-            ml_model_type_request=ml_model_type_request,
+        _param = self._ml_model_type_destroy_serialize(
+            id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '201': "MLModelType",
+            '204': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_modeltype_create_serialize(
+    def _ml_model_type_destroy_serialize(
         self,
-        ml_model_type_request,
+        id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -2164,54 +2182,33 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if ml_model_type_request is not None:
-            _body_params = ml_model_type_request
 
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json', 
-                        'application/x-www-form-urlencoded', 
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/api/ml/modeltype/',
+            method='DELETE',
+            resource_path='/api/ml/model-type/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2220,35 +2217,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_modeltype_destroy(
+    def ml_model_type_list(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> None:
-        """ml_modeltype_destroy
+    ) -> PaginatedMLModelTypeList:
+        """ml_model_type_list
 
 
-        :param id: A unique integer value identifying this ml model type. (required)
-        :type id: int
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2263,58 +2263,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_destroy_serialize(
-            id=id,
+        _param = self._ml_model_type_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': None,
+            '200': "PaginatedMLModelTypeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_modeltype_destroy_with_http_info(
+    def ml_model_type_list_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[None]:
-        """ml_modeltype_destroy
+    ) -> ApiResponse[PaginatedMLModelTypeList]:
+        """ml_model_type_list
 
 
-        :param id: A unique integer value identifying this ml model type. (required)
-        :type id: int
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2329,58 +2333,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_destroy_serialize(
-            id=id,
+        _param = self._ml_model_type_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': None,
+            '200': "PaginatedMLModelTypeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_modeltype_destroy_without_preload_content(
+    def ml_model_type_list_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_modeltype_destroy
+        """ml_model_type_list
 
 
-        :param id: A unique integer value identifying this ml model type. (required)
-        :type id: int
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2395,35 +2403,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_destroy_serialize(
-            id=id,
+        _param = self._ml_model_type_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '204': None,
+            '200': "PaginatedMLModelTypeList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_modeltype_destroy_serialize(
+    def _ml_model_type_list_serialize(
         self,
-        id,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -2435,33 +2445,45 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if id is not None:
-            _path_params['id'] = id
         # process the query parameters
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            [
+                'application/json'
+            ]
+        )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/api/ml/modeltype/{id}/',
+            method='GET',
+            resource_path='/api/ml/model-type/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2470,32 +2492,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_modeltype_list(
+    def ml_model_type_partial_update(
         self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        patched_ml_model_type_request: Optional[PatchedMLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[MLModelType]:
-        """ml_modeltype_list
+    ) -> MLModelType:
+        """ml_model_type_partial_update
 
 
+        :param id: A unique integer value identifying this ml model type. (required)
+        :type id: int
+        :param patched_ml_model_type_request:
+        :type patched_ml_model_type_request: PatchedMLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2510,54 +2538,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_list_serialize(
+        _param = self._ml_model_type_partial_update_serialize(
+            id=id,
+            patched_ml_model_type_request=patched_ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MLModelType]",
+            '200': "MLModelType",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_modeltype_list_with_http_info(
+    def ml_model_type_partial_update_with_http_info(
         self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        patched_ml_model_type_request: Optional[PatchedMLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[MLModelType]]:
-        """ml_modeltype_list
+    ) -> ApiResponse[MLModelType]:
+        """ml_model_type_partial_update
 
 
+        :param id: A unique integer value identifying this ml model type. (required)
+        :type id: int
+        :param patched_ml_model_type_request:
+        :type patched_ml_model_type_request: PatchedMLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2572,54 +2608,62 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_list_serialize(
+        _param = self._ml_model_type_partial_update_serialize(
+            id=id,
+            patched_ml_model_type_request=patched_ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MLModelType]",
+            '200': "MLModelType",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_modeltype_list_without_preload_content(
+    def ml_model_type_partial_update_without_preload_content(
         self,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        patched_ml_model_type_request: Optional[PatchedMLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_modeltype_list
+        """ml_model_type_partial_update
 
 
+        :param id: A unique integer value identifying this ml model type. (required)
+        :type id: int
+        :param patched_ml_model_type_request:
+        :type patched_ml_model_type_request: PatchedMLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2634,33 +2678,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_list_serialize(
+        _param = self._ml_model_type_partial_update_serialize(
+            id=id,
+            patched_ml_model_type_request=patched_ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[MLModelType]",
+            '200': "MLModelType",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_modeltype_list_serialize(
+    def _ml_model_type_partial_update_serialize(
         self,
+        id,
+        patched_ml_model_type_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -2672,37 +2720,56 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if id is not None:
+            _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if patched_ml_model_type_request is not None:
+            _body_params = patched_ml_model_type_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/ml/modeltype/',
+            method='PATCH',
+            resource_path='/api/ml/model-type/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2711,38 +2778,35 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_modeltype_partial_update(
+    def ml_model_type_retrieve(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
-        patched_ml_model_type_request: Optional[PatchedMLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> MLModelType:
-        """ml_modeltype_partial_update
+        """ml_model_type_retrieve
 
 
         :param id: A unique integer value identifying this ml model type. (required)
         :type id: int
-        :param patched_ml_model_type_request:
-        :type patched_ml_model_type_request: PatchedMLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2757,17 +2821,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_partial_update_serialize(
+        _param = self._ml_model_type_retrieve_serialize(
             id=id,
-            patched_ml_model_type_request=patched_ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -2781,38 +2844,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_modeltype_partial_update_with_http_info(
+    def ml_model_type_retrieve_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
-        patched_ml_model_type_request: Optional[PatchedMLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[MLModelType]:
-        """ml_modeltype_partial_update
+        """ml_model_type_retrieve
 
 
         :param id: A unique integer value identifying this ml model type. (required)
         :type id: int
-        :param patched_ml_model_type_request:
-        :type patched_ml_model_type_request: PatchedMLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2827,17 +2887,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_partial_update_serialize(
+        _param = self._ml_model_type_retrieve_serialize(
             id=id,
-            patched_ml_model_type_request=patched_ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -2851,38 +2910,35 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_modeltype_partial_update_without_preload_content(
+    def ml_model_type_retrieve_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
-        patched_ml_model_type_request: Optional[PatchedMLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_modeltype_partial_update
+        """ml_model_type_retrieve
 
 
         :param id: A unique integer value identifying this ml model type. (required)
         :type id: int
-        :param patched_ml_model_type_request:
-        :type patched_ml_model_type_request: PatchedMLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -2897,17 +2953,16 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_partial_update_serialize(
+        _param = self._ml_model_type_retrieve_serialize(
             id=id,
-            patched_ml_model_type_request=patched_ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -2916,18 +2971,17 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_modeltype_partial_update_serialize(
+    def _ml_model_type_retrieve_serialize(
         self,
         id,
-        patched_ml_model_type_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -2945,50 +2999,33 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if patched_ml_model_type_request is not None:
-            _body_params = patched_ml_model_type_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json', 
-                        'application/x-www-form-urlencoded', 
-                        'multipart/form-data'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='PATCH',
-            resource_path='/api/ml/modeltype/{id}/',
+            method='GET',
+            resource_path='/api/ml/model-type/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -2997,35 +3034,38 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_modeltype_retrieve(
+    def ml_model_type_update(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        ml_model_type_request: Optional[MLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> MLModelType:
-        """ml_modeltype_retrieve
+        """ml_model_type_update
 
 
         :param id: A unique integer value identifying this ml model type. (required)
         :type id: int
+        :param ml_model_type_request:
+        :type ml_model_type_request: MLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3040,16 +3080,17 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_retrieve_serialize(
+        _param = self._ml_model_type_update_serialize(
             id=id,
+            ml_model_type_request=ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3063,35 +3104,38 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_modeltype_retrieve_with_http_info(
+    def ml_model_type_update_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        ml_model_type_request: Optional[MLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[MLModelType]:
-        """ml_modeltype_retrieve
+        """ml_model_type_update
 
 
         :param id: A unique integer value identifying this ml model type. (required)
         :type id: int
+        :param ml_model_type_request:
+        :type ml_model_type_request: MLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3106,16 +3150,17 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_retrieve_serialize(
+        _param = self._ml_model_type_update_serialize(
             id=id,
+            ml_model_type_request=ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3129,35 +3174,38 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_modeltype_retrieve_without_preload_content(
+    def ml_model_type_update_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
+        ml_model_type_request: Optional[MLModelTypeRequest] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_modeltype_retrieve
+        """ml_model_type_update
 
 
         :param id: A unique integer value identifying this ml model type. (required)
         :type id: int
+        :param ml_model_type_request:
+        :type ml_model_type_request: MLModelTypeRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3172,16 +3220,17 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_retrieve_serialize(
+        _param = self._ml_model_type_update_serialize(
             id=id,
+            ml_model_type_request=ml_model_type_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -3190,17 +3239,18 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_modeltype_retrieve_serialize(
+    def _ml_model_type_update_serialize(
         self,
         id,
+        ml_model_type_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -3218,33 +3268,50 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if ml_model_type_request is not None:
+            _body_params = ml_model_type_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json', 
+                        'application/x-www-form-urlencoded', 
+                        'multipart/form-data'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/ml/modeltype/{id}/',
+            method='PUT',
+            resource_path='/api/ml/model-type/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -3253,38 +3320,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def ml_modeltype_update(
+    def ml_model_update(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
-        ml_model_type_request: Optional[MLModelTypeRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model.")],
+        ml_model_request: MLModelRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> MLModelType:
-        """ml_modeltype_update
+    ) -> MLModel:
+        """ml_model_update
 
+        A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
-        :param id: A unique integer value identifying this ml model type. (required)
+        :param id: A unique integer value identifying this ml model. (required)
         :type id: int
-        :param ml_model_type_request:
-        :type ml_model_type_request: MLModelTypeRequest
+        :param ml_model_request: (required)
+        :type ml_model_request: MLModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3299,62 +3367,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_update_serialize(
+        _param = self._ml_model_update_serialize(
             id=id,
-            ml_model_type_request=ml_model_type_request,
+            ml_model_request=ml_model_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MLModelType",
+            '200': "MLModel",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def ml_modeltype_update_with_http_info(
+    def ml_model_update_with_http_info(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
-        ml_model_type_request: Optional[MLModelTypeRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model.")],
+        ml_model_request: MLModelRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[MLModelType]:
-        """ml_modeltype_update
+    ) -> ApiResponse[MLModel]:
+        """ml_model_update
 
+        A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
-        :param id: A unique integer value identifying this ml model type. (required)
+        :param id: A unique integer value identifying this ml model. (required)
         :type id: int
-        :param ml_model_type_request:
-        :type ml_model_type_request: MLModelTypeRequest
+        :param ml_model_request: (required)
+        :type ml_model_request: MLModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3369,62 +3438,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_update_serialize(
+        _param = self._ml_model_update_serialize(
             id=id,
-            ml_model_type_request=ml_model_type_request,
+            ml_model_request=ml_model_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MLModelType",
+            '200': "MLModel",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def ml_modeltype_update_without_preload_content(
+    def ml_model_update_without_preload_content(
         self,
-        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model type.")],
-        ml_model_type_request: Optional[MLModelTypeRequest] = None,
+        id: Annotated[StrictInt, Field(description="A unique integer value identifying this ml model.")],
+        ml_model_request: MLModelRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """ml_modeltype_update
+        """ml_model_update
 
+        A viewset for ML models. It filters results based on the permissions granted to all the user's team(s).  A user will only be able to interact with an ML models if at least one of the teams they are a member of has access to it.
 
-        :param id: A unique integer value identifying this ml model type. (required)
+        :param id: A unique integer value identifying this ml model. (required)
         :type id: int
-        :param ml_model_type_request:
-        :type ml_model_type_request: MLModelTypeRequest
+        :param ml_model_request: (required)
+        :type ml_model_request: MLModelRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -3439,37 +3509,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._ml_modeltype_update_serialize(
+        _param = self._ml_model_update_serialize(
             id=id,
-            ml_model_type_request=ml_model_type_request,
+            ml_model_request=ml_model_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "MLModelType",
+            '200': "MLModel",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _ml_modeltype_update_serialize(
+    def _ml_model_update_serialize(
         self,
         id,
-        ml_model_type_request,
+        ml_model_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -3487,16 +3557,16 @@
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if ml_model_type_request is not None:
-            _body_params = ml_model_type_request
+        if ml_model_request is not None:
+            _body_params = ml_model_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
@@ -3522,15 +3592,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
-            resource_path='/api/ml/modeltype/{id}/',
+            resource_path='/api/ml/model/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `avis_client-0.6.0/avis_client/api/product_api.py` & `avis_client-0.7.0/avis_client/api/product_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -25,14 +25,15 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
+from avis_client.models.paginated_product_list import PaginatedProductList
 from avis_client.models.patched_product_request import PatchedProductRequest
 from avis_client.models.product import Product
 from avis_client.models.product_request import ProductRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
@@ -581,39 +582,48 @@
     @validate_call
     def product_list(
         self,
         category: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         identifier: Annotated[Optional[List[StrictStr]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Product]:
+    ) -> PaginatedProductList:
         """product_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param category: Multiple values may be separated by commas.
         :type category: List[int]
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
         :param identifier: Multiple values may be separated by commas.
         :type identifier: List[str]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -633,22 +643,25 @@
         """ # noqa: E501
 
         _param = self._product_list_serialize(
             category=category,
             fields=fields,
             id=id,
             identifier=identifier,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Product]",
+            '200': "PaginatedProductList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -660,39 +673,48 @@
     @validate_call
     def product_list_with_http_info(
         self,
         category: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         identifier: Annotated[Optional[List[StrictStr]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Product]]:
+    ) -> ApiResponse[PaginatedProductList]:
         """product_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param category: Multiple values may be separated by commas.
         :type category: List[int]
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
         :param identifier: Multiple values may be separated by commas.
         :type identifier: List[str]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -712,22 +734,25 @@
         """ # noqa: E501
 
         _param = self._product_list_serialize(
             category=category,
             fields=fields,
             id=id,
             identifier=identifier,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Product]",
+            '200': "PaginatedProductList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -739,14 +764,17 @@
     @validate_call
     def product_list_without_preload_content(
         self,
         category: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
         identifier: Annotated[Optional[List[StrictStr]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -764,14 +792,20 @@
         :type category: List[int]
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
         :param identifier: Multiple values may be separated by commas.
         :type identifier: List[str]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -791,36 +825,42 @@
         """ # noqa: E501
 
         _param = self._product_list_serialize(
             category=category,
             fields=fields,
             id=id,
             identifier=identifier,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Product]",
+            '200': "PaginatedProductList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _product_list_serialize(
         self,
         category,
         fields,
         id,
         identifier,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -852,14 +892,26 @@
             
             _query_params.append(('id', id))
             
         if identifier is not None:
             
             _query_params.append(('identifier', identifier))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/product_category_api.py` & `avis_client-0.7.0/avis_client/api/product_category_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -25,14 +25,15 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
+from avis_client.models.paginated_product_category_list import PaginatedProductCategoryList
 from avis_client.models.patched_product_category_request import PatchedProductCategoryRequest
 from avis_client.models.product_category import ProductCategory
 from avis_client.models.product_category_request import ProductCategoryRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def product_category_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[ProductCategory]:
+    ) -> PaginatedProductCategoryList:
         """product_category_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._product_category_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ProductCategory]",
+            '200': "PaginatedProductCategoryList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def product_category_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[ProductCategory]]:
+    ) -> ApiResponse[PaginatedProductCategoryList]:
         """product_category_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._product_category_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ProductCategory]",
+            '200': "PaginatedProductCategoryList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def product_category_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._product_category_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[ProductCategory]",
+            '200': "PaginatedProductCategoryList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _product_category_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/quality_criteria_api.py` & `avis_client-0.7.0/avis_client/api/quality_criteria_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -25,14 +25,15 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
+from avis_client.models.paginated_quality_criteria_list import PaginatedQualityCriteriaList
 from avis_client.models.patched_quality_criteria_request import PatchedQualityCriteriaRequest
 from avis_client.models.quality_criteria import QualityCriteria
 from avis_client.models.quality_criteria_request import QualityCriteriaRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def quality_criteria_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[QualityCriteria]:
+    ) -> PaginatedQualityCriteriaList:
         """quality_criteria_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._quality_criteria_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[QualityCriteria]",
+            '200': "PaginatedQualityCriteriaList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def quality_criteria_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[QualityCriteria]]:
+    ) -> ApiResponse[PaginatedQualityCriteriaList]:
         """quality_criteria_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._quality_criteria_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[QualityCriteria]",
+            '200': "PaginatedQualityCriteriaList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def quality_criteria_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._quality_criteria_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[QualityCriteria]",
+            '200': "PaginatedQualityCriteriaList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _quality_criteria_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/result_api.py` & `avis_client-0.7.0/avis_client/api/result_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -25,14 +25,15 @@
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
+from avis_client.models.paginated_result_list import PaginatedResultList
 from avis_client.models.patched_result_request import PatchedResultRequest
 from avis_client.models.result import Result
 from avis_client.models.result_request import ResultRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
@@ -579,35 +580,44 @@
 
 
     @validate_call
     def result_list(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Result]:
+    ) -> PaginatedResultList:
         """result_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -625,22 +635,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._result_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Result]",
+            '200': "PaginatedResultList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -650,35 +663,44 @@
 
 
     @validate_call
     def result_list_with_http_info(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Result]]:
+    ) -> ApiResponse[PaginatedResultList]:
         """result_list
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -696,22 +718,25 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._result_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Result]",
+            '200': "PaginatedResultList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -721,14 +746,17 @@
 
 
     @validate_call
     def result_list_without_preload_content(
         self,
         fields: Optional[StrictStr] = None,
         id: Annotated[Optional[List[StrictInt]], Field(description="Multiple values may be separated by commas.")] = None,
+        ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -742,14 +770,20 @@
 
         A base viewset that allows reading, creating and updating objects. The following functionalities are added by the mixins:  * CreateModelMixin: allows creating objects * UpdateModelMixin: allows updating objects * DestroyModelMixin: allows deleting objects * OptimizedReadOnlyTracedViewSet: allows reading objects and adds tracing and optimized queryset fetching (with the use of the `fields` query parameter)
 
         :param fields:
         :type fields: str
         :param id: Multiple values may be separated by commas.
         :type id: List[int]
+        :param ordering: Which field to use when ordering the results.
+        :type ordering: str
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -767,34 +801,40 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._result_list_serialize(
             fields=fields,
             id=id,
+            ordering=ordering,
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Result]",
+            '200': "PaginatedResultList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _result_list_serialize(
         self,
         fields,
         id,
+        ordering,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -816,14 +856,26 @@
             
             _query_params.append(('fields', fields))
             
         if id is not None:
             
             _query_params.append(('id', id))
             
+        if ordering is not None:
+            
+            _query_params.append(('ordering', ordering))
+            
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `avis_client-0.6.0/avis_client/api/team_api.py` & `avis_client-0.7.0/avis_client/api/teams_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -23,39 +23,40 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictInt
 
-from typing import List
+from typing import Optional
 
+from avis_client.models.paginated_team_list import PaginatedTeamList
 from avis_client.models.team import Team
 from avis_client.models.team_request import TeamRequest
 
 from avis_client.api_client import ApiClient
 from avis_client.api_response import ApiResponse
 from avis_client.rest import RESTResponseType
 
 
-class TeamApi:
+class TeamsApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def team_create(
+    def teams_create(
         self,
         team_request: TeamRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -63,15 +64,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Team:
-        """team_create
+        """teams_create
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -91,15 +92,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_create_serialize(
+        _param = self._teams_create_serialize(
             team_request=team_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -114,15 +115,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def team_create_with_http_info(
+    def teams_create_with_http_info(
         self,
         team_request: TeamRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -130,15 +131,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Team]:
-        """team_create
+        """teams_create
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -158,15 +159,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_create_serialize(
+        _param = self._teams_create_serialize(
             team_request=team_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -181,15 +182,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def team_create_without_preload_content(
+    def teams_create_without_preload_content(
         self,
         team_request: TeamRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -197,15 +198,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """team_create
+        """teams_create
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param team_request: (required)
         :type team_request: TeamRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -225,15 +226,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_create_serialize(
+        _param = self._teams_create_serialize(
             team_request=team_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -243,15 +244,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _team_create_serialize(
+    def _teams_create_serialize(
         self,
         team_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -304,15 +305,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='POST',
-            resource_path='/api/team/',
+            resource_path='/api/teams/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -321,15 +322,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def team_destroy(
+    def teams_destroy(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -337,15 +338,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """team_destroy
+        """teams_destroy
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -365,15 +366,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_destroy_serialize(
+        _param = self._teams_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -388,15 +389,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def team_destroy_with_http_info(
+    def teams_destroy_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -404,15 +405,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """team_destroy
+        """teams_destroy
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -432,15 +433,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_destroy_serialize(
+        _param = self._teams_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -455,15 +456,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def team_destroy_without_preload_content(
+    def teams_destroy_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -471,15 +472,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """team_destroy
+        """teams_destroy
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -499,15 +500,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_destroy_serialize(
+        _param = self._teams_destroy_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -517,15 +518,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _team_destroy_serialize(
+    def _teams_destroy_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -557,15 +558,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='DELETE',
-            resource_path='/api/team/{id}/',
+            resource_path='/api/teams/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -574,33 +575,39 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def team_list(
+    def teams_list(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Team]:
-        """team_list
+    ) -> PaginatedTeamList:
+        """teams_list
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -615,55 +622,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_list_serialize(
+        _param = self._teams_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Team]",
+            '200': "PaginatedTeamList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def team_list_with_http_info(
+    def teams_list_with_http_info(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Team]]:
-        """team_list
+    ) -> ApiResponse[PaginatedTeamList]:
+        """teams_list
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -678,55 +693,63 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_list_serialize(
+        _param = self._teams_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Team]",
+            '200': "PaginatedTeamList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def team_list_without_preload_content(
+    def teams_list_without_preload_content(
         self,
+        page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
+        page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """team_list
+        """teams_list
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
+        :param page: A page number within the paginated result set.
+        :type page: int
+        :param page_size: Number of results to return per page.
+        :type page_size: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -741,33 +764,37 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_list_serialize(
+        _param = self._teams_list_serialize(
+            page=page,
+            page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "List[Team]",
+            '200': "PaginatedTeamList",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _team_list_serialize(
+    def _teams_list_serialize(
         self,
+        page,
+        page_size,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -780,14 +807,22 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if page is not None:
+            
+            _query_params.append(('page', page))
+            
+        if page_size is not None:
+            
+            _query_params.append(('page_size', page_size))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -801,15 +836,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/team/',
+            resource_path='/api/teams/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -818,15 +853,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def team_retrieve(
+    def teams_retrieve(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -834,15 +869,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Team:
-        """team_retrieve
+        """teams_retrieve
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -862,15 +897,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_retrieve_serialize(
+        _param = self._teams_retrieve_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -885,15 +920,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def team_retrieve_with_http_info(
+    def teams_retrieve_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -901,15 +936,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Team]:
-        """team_retrieve
+        """teams_retrieve
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -929,15 +964,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_retrieve_serialize(
+        _param = self._teams_retrieve_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -952,15 +987,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def team_retrieve_without_preload_content(
+    def teams_retrieve_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -968,15 +1003,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """team_retrieve
+        """teams_retrieve
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -996,15 +1031,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_retrieve_serialize(
+        _param = self._teams_retrieve_serialize(
             id=id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
@@ -1014,15 +1049,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _team_retrieve_serialize(
+    def _teams_retrieve_serialize(
         self,
         id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
@@ -1060,15 +1095,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='GET',
-            resource_path='/api/team/{id}/',
+            resource_path='/api/teams/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -1077,15 +1112,15 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def team_update(
+    def teams_update(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         team_request: TeamRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -1094,15 +1129,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> Team:
-        """team_update
+        """teams_update
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param team_request: (required)
         :type team_request: TeamRequest
@@ -1124,15 +1159,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_update_serialize(
+        _param = self._teams_update_serialize(
             id=id,
             team_request=team_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
@@ -1148,15 +1183,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def team_update_with_http_info(
+    def teams_update_with_http_info(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         team_request: TeamRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -1165,15 +1200,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[Team]:
-        """team_update
+        """teams_update
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param team_request: (required)
         :type team_request: TeamRequest
@@ -1195,15 +1230,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_update_serialize(
+        _param = self._teams_update_serialize(
             id=id,
             team_request=team_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
@@ -1219,15 +1254,15 @@
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def team_update_without_preload_content(
+    def teams_update_without_preload_content(
         self,
         id: Annotated[StrictInt, Field(description="A unique integer value identifying this team.")],
         team_request: TeamRequest,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
@@ -1236,15 +1271,15 @@
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """team_update
+        """teams_update
 
         A base read-only viewset that enables optimized queryset fetching and tracing.  This is a combination of the following mixins: * OptimizedQuerySetMixin (from drf_jsonmask): allows the client to specify which fields to return by exposing a `fields` query parameter. If this parameter is not specified, all fields are returned. If it is specified, only the specified fields are returned and the other fields are not fetched from the database. * TracedModelViewSetMixin (from vue_instrumentation): adds tracing to the viewset's methods. * ListModelMixin, RetrieveModelMixin  (from django-rest-framework): adds a list and retrieve method to the viewset making it read-only.
 
         :param id: A unique integer value identifying this team. (required)
         :type id: int
         :param team_request: (required)
         :type team_request: TeamRequest
@@ -1266,15 +1301,15 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._team_update_serialize(
+        _param = self._teams_update_serialize(
             id=id,
             team_request=team_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
@@ -1285,15 +1320,15 @@
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _team_update_serialize(
+    def _teams_update_serialize(
         self,
         id,
         team_request,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
@@ -1349,15 +1384,15 @@
         _auth_settings: List[str] = [
             'cookieAuth', 
             'ApiKeyAuth'
         ]
 
         return self.api_client.param_serialize(
             method='PUT',
-            resource_path='/api/team/{id}/',
+            resource_path='/api/teams/{id}/',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `avis_client-0.6.0/avis_client/api/user_api.py` & `avis_client-0.7.0/avis_client/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.6.0/avis_client/api_client.py` & `avis_client-0.7.0/avis_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -82,15 +82,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.6.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.7.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `avis_client-0.6.0/avis_client/api_response.py` & `avis_client-0.7.0/avis_client/api_response.py`

 * *Files identical despite different names*

### Comparing `avis_client-0.6.0/avis_client/configuration.py` & `avis_client-0.7.0/avis_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -83,15 +83,15 @@
                  access_token=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ) -> None:
         """Constructor
         """
-        self._base_path = "https://avis.vu.engineering" if host is None else host
+        self._base_path = "http://localhost:8000" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -401,31 +401,27 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.6.0\n"\
-               "SDK Package Version: 0.6.0".\
+               "Version of the API: 0.7.0\n"\
+               "SDK Package Version: 0.7.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "https://avis.vu.engineering",
-                'description': "Production server (uses live data)",
-            },
-            {
                 'url': "http://localhost:8000",
-                'description': "Local development server",
+                'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
         :param variables: hash of variable and the corresponding value
```

### Comparing `avis_client-0.6.0/avis_client/exceptions.py` & `avis_client-0.7.0/avis_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `avis_client-0.6.0/avis_client/models/azure_ml_inference_request.py` & `avis_client-0.7.0/avis_client/models/azure_ml_inference_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/blank_enum.py` & `avis_client-0.7.0/avis_client/models/blank_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/configuration_type.py` & `avis_client-0.7.0/avis_client/models/configuration_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/configuration_type_request.py` & `avis_client-0.7.0/avis_client/models/configuration_type_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/custom_user.py` & `avis_client-0.7.0/avis_client/models/custom_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/custom_user_request.py` & `avis_client-0.7.0/avis_client/models/custom_user_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/email_address.py` & `avis_client-0.7.0/avis_client/models/email_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/format_enum.py` & `avis_client-0.7.0/avis_client/models/format_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/image.py` & `avis_client-0.7.0/avis_client/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/image_attribute.py` & `avis_client-0.7.0/avis_client/models/image_attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/image_attribute_category.py` & `avis_client-0.7.0/avis_client/models/image_attribute_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/image_attribute_category_request.py` & `avis_client-0.7.0/avis_client/models/image_attribute_category_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/image_attribute_request.py` & `avis_client-0.7.0/avis_client/models/image_attribute_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/image_request.py` & `avis_client-0.7.0/avis_client/models/image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/inspection.py` & `avis_client-0.7.0/avis_client/models/inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/inspection_request.py` & `avis_client-0.7.0/avis_client/models/inspection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/inspection_status.py` & `avis_client-0.7.0/avis_client/models/inspection_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/inspection_status_enum.py` & `avis_client-0.7.0/avis_client/models/inspection_status_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/inspection_validation_status.py` & `avis_client-0.7.0/avis_client/models/inspection_validation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/membership.py` & `avis_client-0.7.0/avis_client/models/membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/membership_request.py` & `avis_client-0.7.0/avis_client/models/membership_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/metadata.py` & `avis_client-0.7.0/avis_client/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/metadata_request.py` & `avis_client-0.7.0/avis_client/models/metadata_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/metadata_schema.py` & `avis_client-0.7.0/avis_client/models/metadata_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/metadata_schema_request.py` & `avis_client-0.7.0/avis_client/models/metadata_schema_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/ml_model.py` & `avis_client-0.7.0/avis_client/models/ml_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/ml_model_request.py` & `avis_client-0.7.0/avis_client/models/ml_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/ml_model_type.py` & `avis_client-0.7.0/avis_client/models/ml_model_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/ml_model_type_request.py` & `avis_client-0.7.0/avis_client/models/ml_model_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_configuration_type_request.py` & `avis_client-0.7.0/avis_client/models/patched_configuration_type_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_image_attribute_category_request.py` & `avis_client-0.7.0/avis_client/models/patched_image_attribute_category_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_image_attribute_request.py` & `avis_client-0.7.0/avis_client/models/patched_image_attribute_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_image_request.py` & `avis_client-0.7.0/avis_client/models/patched_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_inspection_request.py` & `avis_client-0.7.0/avis_client/models/patched_inspection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_metadata_request.py` & `avis_client-0.7.0/avis_client/models/patched_metadata_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_metadata_schema_request.py` & `avis_client-0.7.0/avis_client/models/patched_metadata_schema_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_ml_model_request.py` & `avis_client-0.7.0/avis_client/models/patched_ml_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_ml_model_type_request.py` & `avis_client-0.7.0/avis_client/models/patched_ml_model_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_product_category_request.py` & `avis_client-0.7.0/avis_client/models/patched_product_category_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_product_request.py` & `avis_client-0.7.0/avis_client/models/patched_product_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_quality_criteria_request.py` & `avis_client-0.7.0/avis_client/models/patched_quality_criteria_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_result_request.py` & `avis_client-0.7.0/avis_client/models/patched_result_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/patched_result_request_status.py` & `avis_client-0.7.0/avis_client/models/patched_result_request_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/product.py` & `avis_client-0.7.0/avis_client/models/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/product_category.py` & `avis_client-0.7.0/avis_client/models/product_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/product_category_request.py` & `avis_client-0.7.0/avis_client/models/product_category_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/product_request.py` & `avis_client-0.7.0/avis_client/models/product_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/quality_criteria.py` & `avis_client-0.7.0/avis_client/models/quality_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/quality_criteria_request.py` & `avis_client-0.7.0/avis_client/models/quality_criteria_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/quality_criteria_result.py` & `avis_client-0.7.0/avis_client/models/quality_criteria_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/quality_enum.py` & `avis_client-0.7.0/avis_client/models/quality_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/result.py` & `avis_client-0.7.0/avis_client/models/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/result_request.py` & `avis_client-0.7.0/avis_client/models/result_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/status_enum.py` & `avis_client-0.7.0/avis_client/models/status_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/team.py` & `avis_client-0.7.0/avis_client/models/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/team_request.py` & `avis_client-0.7.0/avis_client/models/team_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/user_api_key_create.py` & `avis_client-0.7.0/avis_client/models/user_api_key_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/user_api_key_create_request.py` & `avis_client-0.7.0/avis_client/models/user_api_key_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/models/validation_status_enum.py` & `avis_client-0.7.0/avis_client/models/validation_status_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

### Comparing `avis_client-0.6.0/avis_client/rest.py` & `avis_client-0.7.0/avis_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     avis
 
     VUE Autonomous Visual Inspection System (AVIS)
 
-    The version of the OpenAPI document: 0.6.0
+    The version of the OpenAPI document: 0.7.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

### Comparing `avis_client-0.6.0/pyproject.toml` & `avis_client-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools",]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "avis_client"
-version = "0.6.0"
+version = "0.7.0"
 description = "AVIS Python client"
 authors = [ "VUEngineering <tech@vu.engineering>",]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/vuengineering/public/"
 keywords = [ "OpenAPI", "avis", "api client",]
 include = [ "avis_client/py.typed",]
```

### Comparing `avis_client-0.6.0/PKG-INFO` & `avis_client-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,14 @@
-Metadata-Version: 2.1
-Name: avis_client
-Version: 0.6.0
-Summary: AVIS Python client
-Home-page: https://docs.vu.engineering/api/clients/python/avis_client/
-License: Apache-2.0
-Keywords: OpenAPI,avis,api client
-Author: VUEngineering
-Author-email: tech@vu.engineering
-Maintainer: Adriano Pagano
-Maintainer-email: adriano.pagano@vu.engineering
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=2)
-Requires-Dist: python-dateutil (>=2.8.2)
-Requires-Dist: typing-extensions (>=4.7.1)
-Requires-Dist: urllib3 (>=1.25.3)
-Project-URL: Repository, https://github.com/vuengineering/public/
-Description-Content-Type: text/markdown
-
 # avis-client
 VUE Autonomous Visual Inspection System (AVIS)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.6.0
-- Package version: 0.6.0
+- API version: 0.7.0
+- Package version: 0.7.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
@@ -77,18 +51,18 @@
 ```python
 
 import time
 import avis_client
 from avis_client.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to https://avis.vu.engineering
+# Defining the host is optional and defaults to http://localhost:8000
 # See configuration.py for a list of all supported configuration parameters.
 configuration = avis_client.Configuration(
-    host = "https://avis.vu.engineering"
+    host = "http://localhost:8000"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
@@ -118,15 +92,15 @@
     except ApiException as e:
         print("Exception when calling ApiKeysApi->keys_create: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://avis.vu.engineering*
+All URIs are relative to *http://localhost:8000*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApiKeysApi* | [**keys_create**](docs/ApiKeysApi.md#keys_create) | **POST** /api/keys/ | 
 *ApiKeysApi* | [**keys_revoke_create**](docs/ApiKeysApi.md#keys_revoke_create) | **POST** /api/keys/revoke/ | 
 *ConfigurationApi* | [**configuration_create**](docs/ConfigurationApi.md#configuration_create) | **POST** /api/configuration/ | 
 *ConfigurationApi* | [**configuration_destroy**](docs/ConfigurationApi.md#configuration_destroy) | **DELETE** /api/configuration/{id}/ | 
@@ -178,25 +152,25 @@
 *MetadataSchemaApi* | [**metadata_schema_destroy**](docs/MetadataSchemaApi.md#metadata_schema_destroy) | **DELETE** /api/metadata-schema/{id}/ | 
 *MetadataSchemaApi* | [**metadata_schema_list**](docs/MetadataSchemaApi.md#metadata_schema_list) | **GET** /api/metadata-schema/ | 
 *MetadataSchemaApi* | [**metadata_schema_partial_update**](docs/MetadataSchemaApi.md#metadata_schema_partial_update) | **PATCH** /api/metadata-schema/{id}/ | 
 *MetadataSchemaApi* | [**metadata_schema_retrieve**](docs/MetadataSchemaApi.md#metadata_schema_retrieve) | **GET** /api/metadata-schema/{id}/ | 
 *MetadataSchemaApi* | [**metadata_schema_update**](docs/MetadataSchemaApi.md#metadata_schema_update) | **PUT** /api/metadata-schema/{id}/ | 
 *MlApi* | [**ml_model_create**](docs/MlApi.md#ml_model_create) | **POST** /api/ml/model/ | 
 *MlApi* | [**ml_model_destroy**](docs/MlApi.md#ml_model_destroy) | **DELETE** /api/ml/model/{id}/ | 
-*MlApi* | [**ml_model_inference**](docs/MlApi.md#ml_model_inference) | **POST** /api/ml/model/{id}/inference/ | 
+*MlApi* | [**ml_model_inference**](docs/MlApi.md#ml_model_inference) | **POST** /api/ml/model/{id}/infer/ | 
 *MlApi* | [**ml_model_list**](docs/MlApi.md#ml_model_list) | **GET** /api/ml/model/ | 
 *MlApi* | [**ml_model_partial_update**](docs/MlApi.md#ml_model_partial_update) | **PATCH** /api/ml/model/{id}/ | 
 *MlApi* | [**ml_model_retrieve**](docs/MlApi.md#ml_model_retrieve) | **GET** /api/ml/model/{id}/ | 
+*MlApi* | [**ml_model_type_create**](docs/MlApi.md#ml_model_type_create) | **POST** /api/ml/model-type/ | 
+*MlApi* | [**ml_model_type_destroy**](docs/MlApi.md#ml_model_type_destroy) | **DELETE** /api/ml/model-type/{id}/ | 
+*MlApi* | [**ml_model_type_list**](docs/MlApi.md#ml_model_type_list) | **GET** /api/ml/model-type/ | 
+*MlApi* | [**ml_model_type_partial_update**](docs/MlApi.md#ml_model_type_partial_update) | **PATCH** /api/ml/model-type/{id}/ | 
+*MlApi* | [**ml_model_type_retrieve**](docs/MlApi.md#ml_model_type_retrieve) | **GET** /api/ml/model-type/{id}/ | 
+*MlApi* | [**ml_model_type_update**](docs/MlApi.md#ml_model_type_update) | **PUT** /api/ml/model-type/{id}/ | 
 *MlApi* | [**ml_model_update**](docs/MlApi.md#ml_model_update) | **PUT** /api/ml/model/{id}/ | 
-*MlApi* | [**ml_modeltype_create**](docs/MlApi.md#ml_modeltype_create) | **POST** /api/ml/modeltype/ | 
-*MlApi* | [**ml_modeltype_destroy**](docs/MlApi.md#ml_modeltype_destroy) | **DELETE** /api/ml/modeltype/{id}/ | 
-*MlApi* | [**ml_modeltype_list**](docs/MlApi.md#ml_modeltype_list) | **GET** /api/ml/modeltype/ | 
-*MlApi* | [**ml_modeltype_partial_update**](docs/MlApi.md#ml_modeltype_partial_update) | **PATCH** /api/ml/modeltype/{id}/ | 
-*MlApi* | [**ml_modeltype_retrieve**](docs/MlApi.md#ml_modeltype_retrieve) | **GET** /api/ml/modeltype/{id}/ | 
-*MlApi* | [**ml_modeltype_update**](docs/MlApi.md#ml_modeltype_update) | **PUT** /api/ml/modeltype/{id}/ | 
 *ProductApi* | [**product_create**](docs/ProductApi.md#product_create) | **POST** /api/product/ | 
 *ProductApi* | [**product_destroy**](docs/ProductApi.md#product_destroy) | **DELETE** /api/product/{id}/ | 
 *ProductApi* | [**product_list**](docs/ProductApi.md#product_list) | **GET** /api/product/ | 
 *ProductApi* | [**product_partial_update**](docs/ProductApi.md#product_partial_update) | **PATCH** /api/product/{id}/ | 
 *ProductApi* | [**product_retrieve**](docs/ProductApi.md#product_retrieve) | **GET** /api/product/{id}/ | 
 *ProductApi* | [**product_update**](docs/ProductApi.md#product_update) | **PUT** /api/product/{id}/ | 
 *ProductCategoryApi* | [**product_category_create**](docs/ProductCategoryApi.md#product_category_create) | **POST** /api/product-category/ | 
@@ -213,19 +187,29 @@
 *QualityCriteriaApi* | [**quality_criteria_update**](docs/QualityCriteriaApi.md#quality_criteria_update) | **PUT** /api/quality-criteria/{id}/ | 
 *ResultApi* | [**result_create**](docs/ResultApi.md#result_create) | **POST** /api/result/ | 
 *ResultApi* | [**result_destroy**](docs/ResultApi.md#result_destroy) | **DELETE** /api/result/{id}/ | 
 *ResultApi* | [**result_list**](docs/ResultApi.md#result_list) | **GET** /api/result/ | 
 *ResultApi* | [**result_partial_update**](docs/ResultApi.md#result_partial_update) | **PATCH** /api/result/{id}/ | 
 *ResultApi* | [**result_retrieve**](docs/ResultApi.md#result_retrieve) | **GET** /api/result/{id}/ | 
 *ResultApi* | [**result_update**](docs/ResultApi.md#result_update) | **PUT** /api/result/{id}/ | 
-*TeamApi* | [**team_create**](docs/TeamApi.md#team_create) | **POST** /api/team/ | 
-*TeamApi* | [**team_destroy**](docs/TeamApi.md#team_destroy) | **DELETE** /api/team/{id}/ | 
-*TeamApi* | [**team_list**](docs/TeamApi.md#team_list) | **GET** /api/team/ | 
-*TeamApi* | [**team_retrieve**](docs/TeamApi.md#team_retrieve) | **GET** /api/team/{id}/ | 
-*TeamApi* | [**team_update**](docs/TeamApi.md#team_update) | **PUT** /api/team/{id}/ | 
+*StatisticsApi* | [**statistics_inspection_create**](docs/StatisticsApi.md#statistics_inspection_create) | **POST** /api/statistics/inspection/ | 
+*StatisticsApi* | [**statistics_inspection_destroy**](docs/StatisticsApi.md#statistics_inspection_destroy) | **DELETE** /api/statistics/inspection/{id}/ | 
+*StatisticsApi* | [**statistics_inspection_list**](docs/StatisticsApi.md#statistics_inspection_list) | **GET** /api/statistics/inspection/ | 
+*StatisticsApi* | [**statistics_inspection_retrieve**](docs/StatisticsApi.md#statistics_inspection_retrieve) | **GET** /api/statistics/inspection/{id}/ | 
+*StatisticsApi* | [**statistics_inspection_update**](docs/StatisticsApi.md#statistics_inspection_update) | **PUT** /api/statistics/inspection/{id}/ | 
+*StatisticsApi* | [**statistics_team_create**](docs/StatisticsApi.md#statistics_team_create) | **POST** /api/statistics/team/ | 
+*StatisticsApi* | [**statistics_team_destroy**](docs/StatisticsApi.md#statistics_team_destroy) | **DELETE** /api/statistics/team/{id}/ | 
+*StatisticsApi* | [**statistics_team_list**](docs/StatisticsApi.md#statistics_team_list) | **GET** /api/statistics/team/ | 
+*StatisticsApi* | [**statistics_team_retrieve**](docs/StatisticsApi.md#statistics_team_retrieve) | **GET** /api/statistics/team/{id}/ | 
+*StatisticsApi* | [**statistics_team_update**](docs/StatisticsApi.md#statistics_team_update) | **PUT** /api/statistics/team/{id}/ | 
+*TeamsApi* | [**teams_create**](docs/TeamsApi.md#teams_create) | **POST** /api/teams/ | 
+*TeamsApi* | [**teams_destroy**](docs/TeamsApi.md#teams_destroy) | **DELETE** /api/teams/{id}/ | 
+*TeamsApi* | [**teams_list**](docs/TeamsApi.md#teams_list) | **GET** /api/teams/ | 
+*TeamsApi* | [**teams_retrieve**](docs/TeamsApi.md#teams_retrieve) | **GET** /api/teams/{id}/ | 
+*TeamsApi* | [**teams_update**](docs/TeamsApi.md#teams_update) | **PUT** /api/teams/{id}/ | 
 *UserApi* | [**user_email_list**](docs/UserApi.md#user_email_list) | **GET** /api/user/email/ | 
 *UserApi* | [**user_whoami_retrieve**](docs/UserApi.md#user_whoami_retrieve) | **GET** /api/user/whoami/ | 
 
 
 ## Documentation For Models
 
  - [AzureMLInferenceRequest](docs/AzureMLInferenceRequest.md)
@@ -239,28 +223,52 @@
  - [Image](docs/Image.md)
  - [ImageAttribute](docs/ImageAttribute.md)
  - [ImageAttributeCategory](docs/ImageAttributeCategory.md)
  - [ImageAttributeCategoryRequest](docs/ImageAttributeCategoryRequest.md)
  - [ImageAttributeRequest](docs/ImageAttributeRequest.md)
  - [ImageRequest](docs/ImageRequest.md)
  - [Inspection](docs/Inspection.md)
+ - [InspectionImagesStatistics](docs/InspectionImagesStatistics.md)
+ - [InspectionImagesStatisticsRequest](docs/InspectionImagesStatisticsRequest.md)
  - [InspectionRequest](docs/InspectionRequest.md)
+ - [InspectionStatistics](docs/InspectionStatistics.md)
+ - [InspectionStatisticsRequest](docs/InspectionStatisticsRequest.md)
  - [InspectionStatus](docs/InspectionStatus.md)
  - [InspectionStatusEnum](docs/InspectionStatusEnum.md)
  - [InspectionValidationStatus](docs/InspectionValidationStatus.md)
  - [MLModel](docs/MLModel.md)
  - [MLModelRequest](docs/MLModelRequest.md)
  - [MLModelType](docs/MLModelType.md)
  - [MLModelTypeRequest](docs/MLModelTypeRequest.md)
  - [Membership](docs/Membership.md)
  - [MembershipRequest](docs/MembershipRequest.md)
  - [Metadata](docs/Metadata.md)
  - [MetadataRequest](docs/MetadataRequest.md)
  - [MetadataSchema](docs/MetadataSchema.md)
  - [MetadataSchemaRequest](docs/MetadataSchemaRequest.md)
+ - [PaginatedConfigurationTypeList](docs/PaginatedConfigurationTypeList.md)
+ - [PaginatedImageAttributeCategoryList](docs/PaginatedImageAttributeCategoryList.md)
+ - [PaginatedImageAttributeList](docs/PaginatedImageAttributeList.md)
+ - [PaginatedImageList](docs/PaginatedImageList.md)
+ - [PaginatedInspectionImagesStatisticsList](docs/PaginatedInspectionImagesStatisticsList.md)
+ - [PaginatedInspectionList](docs/PaginatedInspectionList.md)
+ - [PaginatedInspectionStatisticsList](docs/PaginatedInspectionStatisticsList.md)
+ - [PaginatedInspectionStatusList](docs/PaginatedInspectionStatusList.md)
+ - [PaginatedInspectionValidationStatusList](docs/PaginatedInspectionValidationStatusList.md)
+ - [PaginatedMLModelList](docs/PaginatedMLModelList.md)
+ - [PaginatedMLModelTypeList](docs/PaginatedMLModelTypeList.md)
+ - [PaginatedMembershipList](docs/PaginatedMembershipList.md)
+ - [PaginatedMetadataList](docs/PaginatedMetadataList.md)
+ - [PaginatedMetadataSchemaList](docs/PaginatedMetadataSchemaList.md)
+ - [PaginatedProductCategoryList](docs/PaginatedProductCategoryList.md)
+ - [PaginatedProductList](docs/PaginatedProductList.md)
+ - [PaginatedQualityCriteriaList](docs/PaginatedQualityCriteriaList.md)
+ - [PaginatedQualityCriteriaResultList](docs/PaginatedQualityCriteriaResultList.md)
+ - [PaginatedResultList](docs/PaginatedResultList.md)
+ - [PaginatedTeamList](docs/PaginatedTeamList.md)
  - [PatchedConfigurationTypeRequest](docs/PatchedConfigurationTypeRequest.md)
  - [PatchedImageAttributeCategoryRequest](docs/PatchedImageAttributeCategoryRequest.md)
  - [PatchedImageAttributeRequest](docs/PatchedImageAttributeRequest.md)
  - [PatchedImageRequest](docs/PatchedImageRequest.md)
  - [PatchedInspectionRequest](docs/PatchedInspectionRequest.md)
  - [PatchedMLModelRequest](docs/PatchedMLModelRequest.md)
  - [PatchedMLModelTypeRequest](docs/PatchedMLModelTypeRequest.md)
@@ -310,8 +318,7 @@
 
 
 ## Author
 
 
 
 
-
```

