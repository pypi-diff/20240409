# Comparing `tmp/graphene-django-3.2.0.tar.gz` & `tmp/graphene-django-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-3.2.0.tar", last modified: Wed Dec 20 10:25:18 2023, max compression
+gzip compressed data, was "graphene-django-3.2.1.tar", last modified: Tue Apr  9 00:41:34 2024, max compression
```

## Comparing `graphene-django-3.2.0.tar` & `graphene-django-3.2.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.194355 graphene-django-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-12-20 10:25:15.000000 graphene-django-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-20 10:25:15.000000 graphene-django-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-20 10:25:18.194355 graphene-django-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2023-12-20 10:25:15.000000 graphene-django-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/cookbook/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/cookbook/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.178355 graphene-django-3.2.0/examples/cookbook/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-20 10:25:15.000000 graphene-django-3.2.0/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/cookbook-plain/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/cookbook-plain/cookbook/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.174355 graphene-django-3.2.0/examples/cookbook-plain/cookbook/ingredients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.178355 graphene-django-3.2.0/examples/cookbook-plain/cookbook/ingredients/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-20 10:25:15.000000 graphene-django-3.2.0/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.178355 graphene-django-3.2.0/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18229 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.182355 graphene-django-3.2.0/graphene_django/debug/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.182355 graphene-django-3.2.0/graphene_django/debug/exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/exception/formating.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/exception/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.182355 graphene-django-3.2.0/graphene_django/debug/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/sql/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.182355 graphene-django-3.2.0/graphene_django/debug/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/debug/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.182355 graphene-django-3.2.0/graphene_django/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.186355 graphene-django-3.2.0/graphene_django/filter/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filters/array_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filters/global_id_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filters/list_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filters/range_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filters/typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/filterset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.186355 graphene-django-3.2.0/graphene_django/filter/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_contains_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_custom_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_exact_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_overlap_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_enum_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    37365 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_in_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_range_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/tests/test_typed_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.186355 graphene-django-3.2.0/graphene_django/forms/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/mutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.186355 graphene-django-3.2.0/graphene_django/forms/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/tests/test_djangoinputobject.py
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/forms/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.186355 graphene-django-3.2.0/graphene_django/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.186355 graphene-django-3.2.0/graphene_django/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/management/commands/graphql_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.190355 graphene-django-3.2.0/graphene_django/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/serializer_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.190355 graphene-django-3.2.0/graphene_django/rest_framework/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/tests/test_field_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/rest_framework/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.178355 graphene-django-3.2.0/graphene_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.190355 graphene-django-3.2.0/graphene_django/static/graphene_django/
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/static/graphene_django/graphiql.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.178355 graphene-django-3.2.0/graphene_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.190355 graphene-django-3.2.0/graphene_django/templates/graphene/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/templates/graphene/graphiql.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.194355 graphene-django-3.2.0/graphene_django/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.194355 graphene-django-3.2.0/graphene_django/tests/issues/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/issues/test_520.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/schema_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20313 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_get_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)    60107 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    20342 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26799 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/urls_inherited.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/urls_pretty.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/tests/urls_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10891 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.194355 graphene-django-3.2.0/graphene_django/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/str_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.194355 graphene-django-3.2.0/graphene_django/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/tests/test_str_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/tests/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2023-12-20 10:25:15.000000 graphene-django-3.2.0/graphene_django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 10:25:18.182355 graphene-django-3.2.0/graphene_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2023-12-20 10:25:18.000000 graphene-django-3.2.0/graphene_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2023-12-20 10:25:18.000000 graphene-django-3.2.0/graphene_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 10:25:18.000000 graphene-django-3.2.0/graphene_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 10:25:18.000000 graphene-django-3.2.0/graphene_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-20 10:25:18.000000 graphene-django-3.2.0/graphene_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-20 10:25:18.000000 graphene-django-3.2.0/graphene_django.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-20 10:25:18.194355 graphene-django-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2023-12-20 10:25:15.000000 graphene-django-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.209563 graphene-django-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 00:41:18.000000 graphene-django-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 00:41:18.000000 graphene-django-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-09 00:41:34.209563 graphene-django-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-09 00:41:18.000000 graphene-django-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 00:41:18.000000 graphene-django-3.2.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook-plain/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook-plain/cookbook/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook-plain/cookbook/ingredients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/examples/cookbook-plain/cookbook/ingredients/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 00:41:18.000000 graphene-django-3.2.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django/debug/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/exception/formating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/exception/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django/debug/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/sql/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django/debug/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/debug/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/filter/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filters/array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filters/global_id_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filters/list_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filters/range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filters/typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/filterset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/filter/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_contains_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_custom_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_exact_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_overlap_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_enum_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37365 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_in_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_range_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/tests/test_typed_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/mutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/tests/test_djangoinputobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/forms/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/management/commands/graphql_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.201563 graphene-django-3.2.1/graphene_django/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/serializer_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.205563 graphene-django-3.2.1/graphene_django/rest_framework/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/tests/test_field_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/rest_framework/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/graphene_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.205563 graphene-django-3.2.1/graphene_django/static/graphene_django/
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/static/graphene_django/graphiql.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.193563 graphene-django-3.2.1/graphene_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.205563 graphene-django-3.2.1/graphene_django/templates/graphene/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/templates/graphene/graphiql.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.205563 graphene-django-3.2.1/graphene_django/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.209563 graphene-django-3.2.1/graphene_django/tests/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/issues/test_520.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/schema_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_get_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60107 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26799 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/urls_inherited.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/urls_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/tests/urls_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.209563 graphene-django-3.2.1/graphene_django/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.209563 graphene-django-3.2.1/graphene_django/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/tests/test_str_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/tests/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-09 00:41:18.000000 graphene-django-3.2.1/graphene_django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:41:34.197563 graphene-django-3.2.1/graphene_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7065 2024-04-09 00:41:34.000000 graphene-django-3.2.1/graphene_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-09 00:41:34.000000 graphene-django-3.2.1/graphene_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:41:34.000000 graphene-django-3.2.1/graphene_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:41:34.000000 graphene-django-3.2.1/graphene_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 00:41:34.000000 graphene-django-3.2.1/graphene_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 00:41:34.000000 graphene-django-3.2.1/graphene_django.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 00:41:34.209563 graphene-django-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-09 00:41:18.000000 graphene-django-3.2.1/setup.py
```

### Comparing `graphene-django-3.2.0/LICENSE` & `graphene-django-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/PKG-INFO` & `graphene-django-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.2.0
+Version: 3.2.1
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
@@ -56,15 +56,15 @@
 * Compatible with Django's form and validation system
 * Extensive documentation and community support
 
 ## Installation
 
 To install Graphene-Django, run the following command:
 
-```
+```sh
 pip install graphene-django
 ```
 
 ## Configuration
 
 After installation, add 'graphene_django' to your Django project's `INSTALLED_APPS` list and define the GraphQL schema in your project's settings:
 
@@ -140,19 +140,19 @@
 
         self.assertResponseNoErrors(response)
         self.assertEqual(len(response.data['mymodels']), MyModel.objects.count())
 ```
 
 ## Contributing
 
-Contributions to Graphene-Django are always welcome! To get started, check the repository's [issue tracker](https://github.com/graphql-python/graphene-django/issues) and [contribution guidelines](https://github.com/graphql-python/graphene-django/blob/master/CONTRIBUTING.md).
+Contributions to Graphene-Django are always welcome! To get started, check the repository's [issue tracker](https://github.com/graphql-python/graphene-django/issues) and [contribution guidelines](https://github.com/graphql-python/graphene-django/blob/main/CONTRIBUTING.md).
 
 ## License
 
-Graphene-Django is released under the [MIT License](https://github.com/graphql-python/graphene-django/blob/master/LICENSE).
+Graphene-Django is released under the [MIT License](https://github.com/graphql-python/graphene-django/blob/main/LICENSE).
 
 ## Resources
 
 * [Official GitHub Repository](https://github.com/graphql-python/graphene-django)
 * [Graphene Documentation](http://docs.graphene-python.org/en/latest/)
 * [Django Documentation](https://docs.djangoproject.com/en/stable/)
 * [GraphQL Specification](https://spec.graphql.org/)
```

### Comparing `graphene-django-3.2.0/README.md` & `graphene-django-3.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 * Compatible with Django's form and validation system
 * Extensive documentation and community support
 
 ## Installation
 
 To install Graphene-Django, run the following command:
 
-```
+```sh
 pip install graphene-django
 ```
 
 ## Configuration
 
 After installation, add 'graphene_django' to your Django project's `INSTALLED_APPS` list and define the GraphQL schema in your project's settings:
 
@@ -110,19 +110,19 @@
 
         self.assertResponseNoErrors(response)
         self.assertEqual(len(response.data['mymodels']), MyModel.objects.count())
 ```
 
 ## Contributing
 
-Contributions to Graphene-Django are always welcome! To get started, check the repository's [issue tracker](https://github.com/graphql-python/graphene-django/issues) and [contribution guidelines](https://github.com/graphql-python/graphene-django/blob/master/CONTRIBUTING.md).
+Contributions to Graphene-Django are always welcome! To get started, check the repository's [issue tracker](https://github.com/graphql-python/graphene-django/issues) and [contribution guidelines](https://github.com/graphql-python/graphene-django/blob/main/CONTRIBUTING.md).
 
 ## License
 
-Graphene-Django is released under the [MIT License](https://github.com/graphql-python/graphene-django/blob/master/LICENSE).
+Graphene-Django is released under the [MIT License](https://github.com/graphql-python/graphene-django/blob/main/LICENSE).
 
 ## Resources
 
 * [Official GitHub Repository](https://github.com/graphql-python/graphene-django)
 * [Graphene Documentation](http://docs.graphene-python.org/en/latest/)
 * [Django Documentation](https://docs.djangoproject.com/en/stable/)
 * [GraphQL Specification](https://spec.graphql.org/)
```

### Comparing `graphene-django-3.2.0/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.2.1/examples/cookbook/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json` & `graphene-django-3.2.1/examples/cookbook-plain/cookbook/ingredients/fixtures/ingredients.json`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/compat.py` & `graphene-django-3.2.1/graphene_django/compat.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/converter.py` & `graphene-django-3.2.1/graphene_django/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import inspect
-from collections import OrderedDict
+from collections.abc import Callable
 from functools import partial, singledispatch, wraps
 
 from django.db import models
 from django.utils.encoding import force_str
 from django.utils.functional import Promise
 from django.utils.module_loading import import_string
 from graphql import GraphQLError
@@ -68,16 +68,23 @@
     except GraphQLError:
         name = "A_%s" % name
     return name
 
 
 def get_choices(choices):
     converted_names = []
-    if isinstance(choices, OrderedDict):
+    if isinstance(choices, Callable):
+        choices = choices()
+
+    # In restframework==3.15.0, choices are not passed
+    # as OrderedDict anymore, so it's safer to check
+    # for a dict
+    if isinstance(choices, dict):
         choices = choices.items()
+
     for value, help_text in choices:
         if isinstance(help_text, (tuple, list)):
             yield from get_choices(help_text)
         else:
             name = convert_choice_name(value)
             while name in converted_names:
                 name += "_" + str(len(converted_names))
```

### Comparing `graphene-django-3.2.0/graphene_django/debug/middleware.py` & `graphene-django-3.2.1/graphene_django/debug/middleware.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/debug/sql/tracking.py` & `graphene-django-3.2.1/graphene_django/debug/sql/tracking.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/debug/sql/types.py` & `graphene-django-3.2.1/graphene_django/debug/sql/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/debug/tests/test_query.py` & `graphene-django-3.2.1/graphene_django/debug/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/fields.py` & `graphene-django-3.2.1/graphene_django/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,28 @@
 
 from .settings import graphene_settings
 from .utils import maybe_queryset
 
 
 class DjangoListField(Field):
     def __init__(self, _type, *args, **kwargs):
-        from .types import DjangoObjectType
-
         if isinstance(_type, NonNull):
             _type = _type.of_type
 
         # Django would never return a Set of None  vvvvvvv
         super().__init__(List(NonNull(_type)), *args, **kwargs)
 
+    @property
+    def type(self):
+        from .types import DjangoObjectType
+
         assert issubclass(
             self._underlying_type, DjangoObjectType
-        ), "DjangoListField only accepts DjangoObjectType types"
+        ), "DjangoListField only accepts DjangoObjectType types as underlying type"
+        return super().type
 
     @property
     def _underlying_type(self):
         _type = self._type
         while hasattr(_type, "of_type"):
             _type = _type.of_type
         return _type
@@ -94,21 +97,27 @@
         _type = super(ConnectionField, self).type
         non_null = False
         if isinstance(_type, NonNull):
             _type = _type.of_type
             non_null = True
         assert issubclass(
             _type, DjangoObjectType
-        ), "DjangoConnectionField only accepts DjangoObjectType types"
+        ), "DjangoConnectionField only accepts DjangoObjectType types as underlying type"
         assert _type._meta.connection, "The type {} doesn't have a connection".format(
             _type.__name__
         )
         connection_type = _type._meta.connection
         if non_null:
             return NonNull(connection_type)
+        # Since Relay Connections require to have a predictible ordering for pagination,
+        # check on init that the Django model provided has a default ordering declared.
+        model = connection_type._meta.node._meta.model
+        assert (
+            len(getattr(model._meta, "ordering", [])) > 0
+        ), f"Django model {model._meta.app_label}.{model.__name__} has to have a default ordering to be used in a Connection."
         return connection_type
 
     @property
     def connection_type(self):
         type = self.type
         if isinstance(type, NonNull):
             return type.of_type
```

### Comparing `graphene-django-3.2.0/graphene_django/filter/__init__.py` & `graphene-django-3.2.1/graphene_django/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/fields.py` & `graphene-django-3.2.1/graphene_django/filter/fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filters/__init__.py` & `graphene-django-3.2.1/graphene_django/filter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filters/array_filter.py` & `graphene-django-3.2.1/graphene_django/filter/filters/array_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filters/global_id_filter.py` & `graphene-django-3.2.1/graphene_django/filter/filters/global_id_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filters/list_filter.py` & `graphene-django-3.2.1/graphene_django/filter/filters/list_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filters/range_filter.py` & `graphene-django-3.2.1/graphene_django/filter/filters/range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filters/typed_filter.py` & `graphene-django-3.2.1/graphene_django/filter/filters/typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/filterset.py` & `graphene-django-3.2.1/graphene_django/filter/filterset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/conftest.py` & `graphene-django-3.2.1/graphene_django/filter/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,17 @@
         pytest.mark.skipif(
             True, reason="django_filters not installed or not compatible"
         )
     )
 
 
 class Event(models.Model):
+    class Meta:
+        ordering = ["pk"]
+
     name = models.CharField(max_length=50)
     tags = ArrayField(models.CharField(max_length=50))
     tag_ids = ArrayField(models.IntegerField())
     random_field = ArrayField(models.BooleanField())
 
     def __repr__(self):
         return f"Event [{self.name}]"
```

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/filters.py` & `graphene-django-3.2.1/graphene_django/filter/tests/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_contains_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_contains_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_custom_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_custom_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_exact_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_exact_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_array_field_overlap_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_array_field_overlap_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_enum_filtering.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_enum_filtering.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_fields.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_in_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_in_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_range_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_range_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/tests/test_typed_filter.py` & `graphene-django-3.2.1/graphene_django/filter/tests/test_typed_filter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/filter/utils.py` & `graphene-django-3.2.1/graphene_django/filter/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/converter.py` & `graphene-django-3.2.1/graphene_django/forms/converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/forms.py` & `graphene-django-3.2.1/graphene_django/forms/forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/mutation.py` & `graphene-django-3.2.1/graphene_django/forms/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/tests/test_converter.py` & `graphene-django-3.2.1/graphene_django/forms/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/tests/test_djangoinputobject.py` & `graphene-django-3.2.1/graphene_django/forms/tests/test_djangoinputobject.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/tests/test_mutation.py` & `graphene-django-3.2.1/graphene_django/forms/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/forms/types.py` & `graphene-django-3.2.1/graphene_django/forms/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/management/commands/graphql_schema.py` & `graphene-django-3.2.1/graphene_django/management/commands/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/registry.py` & `graphene-django-3.2.1/graphene_django/registry.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/rest_framework/models.py` & `graphene-django-3.2.1/graphene_django/rest_framework/models.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/rest_framework/mutation.py` & `graphene-django-3.2.1/graphene_django/rest_framework/mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/rest_framework/serializer_converter.py` & `graphene-django-3.2.1/graphene_django/rest_framework/serializer_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/rest_framework/tests/test_field_converter.py` & `graphene-django-3.2.1/graphene_django/rest_framework/tests/test_field_converter.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/rest_framework/tests/test_multiple_model_serializers.py` & `graphene-django-3.2.1/graphene_django/rest_framework/tests/test_multiple_model_serializers.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/rest_framework/tests/test_mutation.py` & `graphene-django-3.2.1/graphene_django/rest_framework/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/settings.py` & `graphene-django-3.2.1/graphene_django/settings.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/static/graphene_django/graphiql.js` & `graphene-django-3.2.1/graphene_django/static/graphene_django/graphiql.js`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/templates/graphene/graphiql.html` & `graphene-django-3.2.1/graphene_django/templates/graphene/graphiql.html`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/issues/test_520.py` & `graphene-django-3.2.1/graphene_django/tests/issues/test_520.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/models.py` & `graphene-django-3.2.1/graphene_django/tests/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 CHOICES = ((1, "this"), (2, _("that")))
 
 
 class Person(models.Model):
+    class Meta:
+        ordering = ["pk"]
+
     name = models.CharField(max_length=30)
+    parent = models.ForeignKey(
+        "self", on_delete=models.CASCADE, null=True, blank=True, related_name="children"
+    )
 
 
 class Pet(models.Model):
+    class Meta:
+        ordering = ["pk"]
+
     name = models.CharField(max_length=30)
     age = models.PositiveIntegerField()
     owner = models.ForeignKey(
         "Person", on_delete=models.CASCADE, null=True, blank=True, related_name="pets"
     )
 
 
@@ -24,14 +33,17 @@
         related_name="details",
         null=True,
         blank=True,
     )
 
 
 class Film(models.Model):
+    class Meta:
+        ordering = ["pk"]
+
     genre = models.CharField(
         max_length=2,
         help_text="Genre",
         choices=[("do", "Documentary"), ("ac", "Action"), ("ot", "Other")],
         default="ot",
     )
     reporters = models.ManyToManyField("Reporter", related_name="films")
@@ -39,14 +51,17 @@
 
 class DoeReporterManager(models.Manager):
     def get_queryset(self):
         return super().get_queryset().filter(last_name="Doe")
 
 
 class Reporter(models.Model):
+    class Meta:
+        ordering = ["pk"]
+
     first_name = models.CharField(max_length=30)
     last_name = models.CharField(max_length=30)
     email = models.EmailField()
     pets = models.ManyToManyField("self")
     a_choice = models.IntegerField(choices=CHOICES, null=True, blank=True)
     objects = models.Manager()
     doe_objects = DoeReporterManager()
```

### Comparing `graphene-django-3.2.0/graphene_django/tests/schema.py` & `graphene-django-3.2.1/graphene_django/tests/schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/schema_view.py` & `graphene-django-3.2.1/graphene_django/tests/schema_view.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_command.py` & `graphene-django-3.2.1/graphene_django/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_converter.py` & `graphene-django-3.2.1/graphene_django/tests/test_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,14 +176,34 @@
     assert graphene_type._meta.name == "TestTranslatedModelLanguageChoices"
     assert graphene_type._meta.enum.__members__["ES"].value == "es"
     assert graphene_type._meta.enum.__members__["ES"].description == "Spanish"
     assert graphene_type._meta.enum.__members__["EN"].value == "en"
     assert graphene_type._meta.enum.__members__["EN"].description == "English"
 
 
+def test_field_with_callable_choices_convert_enum():
+    def get_choices():
+        return ("es", "Spanish"), ("en", "English")
+
+    field = models.CharField(help_text="Language", choices=get_choices)
+
+    class TranslatedModel(models.Model):
+        language = field
+
+        class Meta:
+            app_label = "test"
+
+    graphene_type = convert_django_field_with_choices(field).type.of_type
+    assert graphene_type._meta.name == "TestTranslatedModelLanguageChoices"
+    assert graphene_type._meta.enum.__members__["ES"].value == "es"
+    assert graphene_type._meta.enum.__members__["ES"].description == "Spanish"
+    assert graphene_type._meta.enum.__members__["EN"].value == "en"
+    assert graphene_type._meta.enum.__members__["EN"].description == "English"
+
+
 def test_field_with_grouped_choices():
     field = models.CharField(
         help_text="Language",
         choices=(("Europe", (("es", "Spanish"), ("en", "English"))),),
     )
 
     class GroupedChoicesModel(models.Model):
```

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_fields.py` & `graphene-django-3.2.1/graphene_django/tests/test_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import datetime
 import re
 
 import pytest
-from django.db.models import Count, Prefetch
+from django.db.models import Count, Model, Prefetch
 
 from graphene import List, NonNull, ObjectType, Schema, String
+from graphene.relay import Node
 
-from ..fields import DjangoListField
+from ..fields import DjangoConnectionField, DjangoListField
 from ..types import DjangoObjectType
 from .models import (
     Article as ArticleModel,
     Film as FilmModel,
     FilmDetails as FilmDetailsModel,
+    Person as PersonModel,
     Reporter as ReporterModel,
 )
 
 
 class TestDjangoListField:
     def test_only_django_object_types(self):
-        class TestType(ObjectType):
-            foo = String()
+        class Query(ObjectType):
+            something = DjangoListField(String)
+
+        with pytest.raises(TypeError) as excinfo:
+            Schema(query=Query)
 
-        with pytest.raises(AssertionError):
-            DjangoListField(TestType)
+        assert (
+            "Query fields cannot be resolved. DjangoListField only accepts DjangoObjectType types as underlying type"
+            in str(excinfo.value)
+        )
 
     def test_only_import_paths(self):
         list_field = DjangoListField("graphene_django.tests.schema.Human")
         from .schema import Human
 
         assert list_field._type.of_type.of_type is Human
 
@@ -258,14 +265,77 @@
         assert result.data == {
             "reporters": [
                 {"firstName": "Tara", "articles": [{"headline": "Amazing news"}]},
                 {"firstName": "Debra", "articles": []},
             ]
         }
 
+    def test_same_type_nested_list_field(self):
+        class Person(DjangoObjectType):
+            class Meta:
+                model = PersonModel
+                fields = ("name", "parent")
+
+            children = DjangoListField(lambda: Person)
+
+        class Query(ObjectType):
+            persons = DjangoListField(Person)
+
+        schema = Schema(query=Query)
+
+        query = """
+            query {
+                persons {
+                    name
+                    children {
+                        name
+                    }
+                }
+            }
+        """
+
+        p1 = PersonModel.objects.create(name="Tara")
+        PersonModel.objects.create(name="Debra")
+
+        PersonModel.objects.create(
+            name="Toto",
+            parent=p1,
+        )
+        PersonModel.objects.create(
+            name="Tata",
+            parent=p1,
+        )
+
+        result = schema.execute(query)
+
+        assert not result.errors
+        assert result.data == {
+            "persons": [
+                {
+                    "name": "Tara",
+                    "children": [
+                        {"name": "Toto"},
+                        {"name": "Tata"},
+                    ],
+                },
+                {
+                    "name": "Debra",
+                    "children": [],
+                },
+                {
+                    "name": "Toto",
+                    "children": [],
+                },
+                {
+                    "name": "Tata",
+                    "children": [],
+                },
+            ]
+        }
+
     def test_get_queryset_filter(self):
         class Reporter(DjangoObjectType):
             class Meta:
                 model = ReporterModel
                 fields = ("first_name", "articles")
 
             @classmethod
@@ -643,7 +713,38 @@
 
         # Then we should have queried for all of the films of all reporters, joined with the film
         # details for each film, using a single query
         assert re.match(
             r'SELECT .* FROM "tests_film" INNER JOIN "tests_film_reporters" .* LEFT OUTER JOIN "tests_filmdetails"',
             captured.captured_queries[1]["sql"],
         )
+
+
+class TestDjangoConnectionField:
+    def test_model_ordering_assertion(self):
+        class Chaos(Model):
+            class Meta:
+                app_label = "test"
+
+        class ChaosType(DjangoObjectType):
+            class Meta:
+                model = Chaos
+                interfaces = (Node,)
+
+        class Query(ObjectType):
+            chaos = DjangoConnectionField(ChaosType)
+
+        with pytest.raises(
+            TypeError,
+            match=r"Django model test\.Chaos has to have a default ordering to be used in a Connection\.",
+        ):
+            Schema(query=Query)
+
+    def test_only_django_object_types(self):
+        class Query(ObjectType):
+            something = DjangoConnectionField(String)
+
+        with pytest.raises(
+            TypeError,
+            match="DjangoConnectionField only accepts DjangoObjectType types as underlying type",
+        ):
+            Schema(query=Query)
```

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_forms.py` & `graphene-django-3.2.1/graphene_django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_get_queryset.py` & `graphene-django-3.2.1/graphene_django/tests/test_get_queryset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_query.py` & `graphene-django-3.2.1/graphene_django/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_schema.py` & `graphene-django-3.2.1/graphene_django/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_types.py` & `graphene-django-3.2.1/graphene_django/tests/test_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from collections import OrderedDict, defaultdict
 from textwrap import dedent
 from unittest.mock import patch
 
 import pytest
 from django.db import models
 
@@ -395,33 +396,32 @@
             class Meta:
                 model = ReporterModel
                 fields = ["first_name", "foo", "email"]
 
     with pytest.warns(
         UserWarning,
         match=r"Field name .* matches an attribute on Django model .* but it's not a model field",
-    ) as record:
+    ):
 
         class Reporter2(DjangoObjectType):
             class Meta:
                 model = ReporterModel
                 fields = ["first_name", "some_method", "email"]
 
     # Don't warn if selecting a custom field
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
 
         class Reporter3(DjangoObjectType):
             custom_field = String()
 
             class Meta:
                 model = ReporterModel
                 fields = ["first_name", "custom_field", "email"]
 
-    assert len(record) == 0
-
 
 @with_local_registry
 def test_django_objecttype_exclude_fields_exist_on_model():
     with pytest.warns(
         UserWarning,
         match=r"Django model .* does not have a field or attribute named .*",
     ):
@@ -441,54 +441,51 @@
             custom_field = String()
 
             class Meta:
                 model = ReporterModel
                 exclude = ["custom_field"]
 
     # Don't warn on exclude fields
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
 
         class Reporter4(DjangoObjectType):
             class Meta:
                 model = ReporterModel
                 exclude = ["email", "first_name"]
 
-    assert len(record) == 0
-
 
 @with_local_registry
 def test_django_objecttype_neither_fields_nor_exclude():
     with pytest.warns(
         DeprecationWarning,
         match=r"Creating a DjangoObjectType without either the `fields` "
         "or the `exclude` option is deprecated.",
     ):
 
         class Reporter(DjangoObjectType):
             class Meta:
                 model = ReporterModel
 
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
 
         class Reporter2(DjangoObjectType):
             class Meta:
                 model = ReporterModel
                 fields = ["email"]
 
-    assert len(record) == 0
-
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
 
         class Reporter3(DjangoObjectType):
             class Meta:
                 model = ReporterModel
                 exclude = ["email"]
 
-    assert len(record) == 0
-
 
 def custom_enum_name(field):
     return f"CustomEnum{field.name.title()}"
 
 
 class TestDjangoObjectType:
     @pytest.fixture
```

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_utils.py` & `graphene-django-3.2.1/graphene_django/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/test_views.py` & `graphene-django-3.2.1/graphene_django/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/tests/urls_validation.py` & `graphene-django-3.2.1/graphene_django/tests/urls_validation.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/types.py` & `graphene-django-3.2.1/graphene_django/types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/utils/testing.py` & `graphene-django-3.2.1/graphene_django/utils/testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/utils/tests/test_testing.py` & `graphene-django-3.2.1/graphene_django/utils/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/utils/utils.py` & `graphene-django-3.2.1/graphene_django/utils/utils.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django/views.py` & `graphene-django-3.2.1/graphene_django/views.py`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/graphene_django.egg-info/PKG-INFO` & `graphene-django-3.2.1/graphene_django.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django
-Version: 3.2.0
+Version: 3.2.1
 Summary: Graphene Django integration
 Home-page: https://github.com/graphql-python/graphene-django
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Keywords: api graphql protocol rest relay graphene
 Platform: any
@@ -56,15 +56,15 @@
 * Compatible with Django's form and validation system
 * Extensive documentation and community support
 
 ## Installation
 
 To install Graphene-Django, run the following command:
 
-```
+```sh
 pip install graphene-django
 ```
 
 ## Configuration
 
 After installation, add 'graphene_django' to your Django project's `INSTALLED_APPS` list and define the GraphQL schema in your project's settings:
 
@@ -140,19 +140,19 @@
 
         self.assertResponseNoErrors(response)
         self.assertEqual(len(response.data['mymodels']), MyModel.objects.count())
 ```
 
 ## Contributing
 
-Contributions to Graphene-Django are always welcome! To get started, check the repository's [issue tracker](https://github.com/graphql-python/graphene-django/issues) and [contribution guidelines](https://github.com/graphql-python/graphene-django/blob/master/CONTRIBUTING.md).
+Contributions to Graphene-Django are always welcome! To get started, check the repository's [issue tracker](https://github.com/graphql-python/graphene-django/issues) and [contribution guidelines](https://github.com/graphql-python/graphene-django/blob/main/CONTRIBUTING.md).
 
 ## License
 
-Graphene-Django is released under the [MIT License](https://github.com/graphql-python/graphene-django/blob/master/LICENSE).
+Graphene-Django is released under the [MIT License](https://github.com/graphql-python/graphene-django/blob/main/LICENSE).
 
 ## Resources
 
 * [Official GitHub Repository](https://github.com/graphql-python/graphene-django)
 * [Graphene Documentation](http://docs.graphene-python.org/en/latest/)
 * [Django Documentation](https://docs.djangoproject.com/en/stable/)
 * [GraphQL Specification](https://spec.graphql.org/)
```

### Comparing `graphene-django-3.2.0/graphene_django.egg-info/SOURCES.txt` & `graphene-django-3.2.1/graphene_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphene-django-3.2.0/setup.py` & `graphene-django-3.2.1/setup.py`

 * *Files identical despite different names*

