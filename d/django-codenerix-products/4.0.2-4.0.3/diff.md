# Comparing `tmp/django-codenerix-products-4.0.2.tar.gz` & `tmp/django-codenerix-products-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-products-4.0.2.tar", last modified: Sun Jan 29 13:00:45 2023, max compression
+gzip compressed data, was "django-codenerix-products-4.0.3.tar", last modified: Tue Apr  9 07:39:58 2024, max compression
```

## Comparing `django-codenerix-products-4.0.2.tar` & `django-codenerix-products-4.0.3.tar`

### file list

```diff
@@ -1,109 +1,124 @@
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.969864 django-codenerix-products-4.0.2/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11357 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/LICENSE
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      301 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/MANIFEST.in
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3233 2023-01-29 13:00:45.969864 django-codenerix-products-4.0.2/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2008 2022-08-14 19:57:03.000000 django-codenerix-products-4.0.2/README.rst
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2023-01-29 13:00:45.000000 django-codenerix-products-4.0.2/codenerix_products/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2440 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/admin.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      152 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/apps.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      892 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/exceptions.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    42432 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/forms.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/locale/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/locale/en/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/locale/en/LC_MESSAGES/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    34434 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/locale/es/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/locale/es/LC_MESSAGES/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13606 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    38346 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/migrations/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    61602 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    19768 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0002_auto_20180117_1628.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      846 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0003_auto_20180117_1655.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1936 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0004_auto_20180117_1745.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      834 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0005_auto_20180118_0739.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1715 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0006_auto_20180118_1126.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      929 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0007_auto_20180123_1316.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      493 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0007_product_caducable.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      527 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0008_auto_20180126_1711.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      814 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0009_auto_20180201_1137.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      359 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0010_merge_20180202_0726.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      424 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0011_auto_20180202_0826.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      516 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0012_productunique_caducity.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7108 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/0013_alter_attribute_public_alter_brand_outstanding_and_more.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.965864 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    23789 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    15355 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8782 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6753 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      963 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      915 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1371 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1202 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      848 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      788 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1187 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1027 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      936 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      864 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      718 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      696 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      661 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      644 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      992 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      942 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      577 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      564 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      636 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      624 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      749 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      719 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2542 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      150 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      171 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    78720 2023-01-29 13:00:13.000000 django-codenerix-products-4.0.2/codenerix_products/models.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/static/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.965864 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.965864 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      725 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/app.js
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1306 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/app_product.js
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3649 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/controllers.js
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.965864 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/partials/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    19360 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/partials/products_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1028 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/productfinals_sublist_rows.html
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.961864 django-codenerix-products-4.0.2/codenerix_products/templates/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.969864 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1260 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/attribute_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1642 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvalue_formmodal.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1642 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvalueattribute_formmodal_next_version.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1180 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvalueattribute_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1642 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvaluefeature_formmodal_next_version.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1180 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvaluefeature_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1180 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvaluefeaturespecial_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvalue_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvalueattribute_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvaluefeature_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvaluefeaturespecial_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1268 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/product_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2389 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productdocument_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2203 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfeature_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2382 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfeaturespecial_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1268 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfinal_list.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2207 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfinalattribute_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2882 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productimage_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2698 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productrelated_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2744 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/subcategory_sublist.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      684 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/tests.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    43792 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/urls.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)   102957 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.2/codenerix_products/views.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-01-29 13:00:45.969864 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3233 2023-01-29 13:00:45.000000 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5856 2023-01-29 13:00:45.000000 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2023-01-29 13:00:45.000000 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       45 2023-01-29 13:00:45.000000 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       19 2023-01-29 13:00:45.000000 django-codenerix-products-4.0.2/django_codenerix_products.egg-info/top_level.txt
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2023-01-29 13:00:45.969864 django-codenerix-products-4.0.2/setup.cfg
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1736 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.2/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:40.000000 django-codenerix-products-4.0.3/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      301 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3233 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2008 2022-08-14 19:57:03.000000 django-codenerix-products-4.0.3/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-04-09 07:39:58.000000 django-codenerix-products-4.0.3/codenerix_products/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2440 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      152 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      892 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/exceptions.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    42432 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/forms.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/locale/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/locale/en/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/locale/en/LC_MESSAGES/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    34434 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/locale/es/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/locale/es/LC_MESSAGES/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13606 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    38346 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.907090 django-codenerix-products-4.0.3/codenerix_products/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    61602 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    19768 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0002_auto_20180117_1628.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      846 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0003_auto_20180117_1655.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1936 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0004_auto_20180117_1745.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      834 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0005_auto_20180118_0739.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1715 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0006_auto_20180118_1126.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      929 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0007_auto_20180123_1316.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      493 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0007_product_caducable.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      527 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0008_auto_20180126_1711.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      814 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0009_auto_20180201_1137.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      359 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0010_merge_20180202_0726.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      424 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0011_auto_20180202_0826.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      516 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0012_productunique_caducity.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7108 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/0013_alter_attribute_public_alter_brand_outstanding_and_more.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    16306 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    23789 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    15355 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7278 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8782 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6753 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      900 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      963 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      915 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1187 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1371 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1202 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      773 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      848 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      788 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1012 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1187 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1027 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      849 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      936 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      864 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      681 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      718 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      696 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      629 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      661 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      644 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      927 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      992 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      942 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      549 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      577 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      564 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      609 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      636 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      624 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      704 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      749 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      719 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2693 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2542 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      154 2023-01-29 13:03:07.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      150 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      171 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    78720 2023-01-29 13:00:13.000000 django-codenerix-products-4.0.3/codenerix_products/models.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      725 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/app.js
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1306 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/app_product.js
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3649 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/controllers.js
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/partials/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    19360 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/partials/products_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1028 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/productfinals_sublist_rows.html
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.903090 django-codenerix-products-4.0.3/codenerix_products/templates/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1260 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/attribute_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1642 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvalue_formmodal.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1642 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvalueattribute_formmodal_next_version.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1180 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvalueattribute_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1642 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvaluefeature_formmodal_next_version.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1180 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvaluefeature_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1180 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvaluefeaturespecial_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvalue_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvalueattribute_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvaluefeature_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2064 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvaluefeaturespecial_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1268 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/product_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2389 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productdocument_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2203 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfeature_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2382 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfeaturespecial_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1268 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfinal_list.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2207 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfinalattribute_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2882 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productimage_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2698 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productrelated_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2744 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/subcategory_sublist.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      684 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/tests.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    43792 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)   102957 2022-08-14 19:57:04.000000 django-codenerix-products-4.0.3/codenerix_products/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3233 2024-04-09 07:39:58.000000 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7101 2024-04-09 07:39:58.000000 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-04-09 07:39:58.000000 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:37:51.000000 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       59 2024-04-09 07:39:58.000000 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       19 2024-04-09 07:39:58.000000 django-codenerix-products-4.0.3/django_codenerix_products.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-04-09 07:39:58.911090 django-codenerix-products-4.0.3/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1762 2024-04-09 07:35:33.000000 django-codenerix-products-4.0.3/setup.py
```

### Comparing `django-codenerix-products-4.0.2/LICENSE` & `django-codenerix-products-4.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {yyyy} {name of copyright owner}
+   Copyright 2024 Codenerix
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `django-codenerix-products-4.0.2/PKG-INFO` & `django-codenerix-products-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-products
-Version: 4.0.2
+Version: 4.0.3
 Summary: Codenerix Products is a module that enables CODENERIX to set products on serveral platforms in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-products
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,products
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-products-4.0.2/README.rst` & `django-codenerix-products-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/admin.py` & `django-codenerix-products-4.0.3/codenerix_products/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/exceptions.py` & `django-codenerix-products-4.0.3/codenerix_products/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/forms.py` & `django-codenerix-products-4.0.3/codenerix_products/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/locale/en/LC_MESSAGES/django.po` & `django-codenerix-products-4.0.3/codenerix_products/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/locale/es/LC_MESSAGES/django.mo` & `django-codenerix-products-4.0.3/codenerix_products/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/locale/es/LC_MESSAGES/django.po` & `django-codenerix-products-4.0.3/codenerix_products/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0001_initial.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0002_auto_20180117_1628.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0002_auto_20180117_1628.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0003_auto_20180117_1655.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0003_auto_20180117_1655.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0004_auto_20180117_1745.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0004_auto_20180117_1745.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0005_auto_20180118_0739.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0005_auto_20180118_0739.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0006_auto_20180118_1126.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0006_auto_20180118_1126.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0007_auto_20180123_1316.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0007_auto_20180123_1316.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0008_auto_20180126_1711.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0008_auto_20180126_1711.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0009_auto_20180201_1137.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0009_auto_20180201_1137.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0012_productunique_caducity.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0012_productunique_caducity.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/0013_alter_attribute_public_alter_brand_outstanding_and_more.py` & `django-codenerix-products-4.0.3/codenerix_products/migrations/0013_alter_attribute_public_alter_brand_outstanding_and_more.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-35.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-39.pyc` & `django-codenerix-products-4.0.3/codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/models.py` & `django-codenerix-products-4.0.3/codenerix_products/models.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/app.js` & `django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/app.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/app_product.js` & `django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/app_product.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/js/controllers.js` & `django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/js/controllers.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/partials/products_list.html` & `django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/partials/products_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/static/codenerix_products/productfinals_sublist_rows.html` & `django-codenerix-products-4.0.3/codenerix_products/static/codenerix_products/productfinals_sublist_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/attribute_list.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/attribute_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvalue_formmodal.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvalue_formmodal.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvalueattribute_formmodal_next_version.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvalueattribute_formmodal_next_version.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvalueattribute_list.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvalueattribute_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvaluefeature_formmodal_next_version.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvaluefeature_formmodal_next_version.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvaluefeature_list.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvaluefeature_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/groupvaluefeaturespecial_list.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/groupvaluefeaturespecial_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvalue_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvalue_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvalueattribute_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvalueattribute_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvaluefeature_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvaluefeature_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/optionvaluefeaturespecial_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/optionvaluefeaturespecial_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/product_list.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/product_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productdocument_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productdocument_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfeature_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfeature_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfeaturespecial_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfeaturespecial_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfinal_list.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfinal_list.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productfinalattribute_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productfinalattribute_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productimage_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productimage_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/productrelated_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/productrelated_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/templates/codenerix_products/subcategory_sublist.html` & `django-codenerix-products-4.0.3/codenerix_products/templates/codenerix_products/subcategory_sublist.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/tests.py` & `django-codenerix-products-4.0.3/codenerix_products/tests.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/urls.py` & `django-codenerix-products-4.0.3/codenerix_products/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/codenerix_products/views.py` & `django-codenerix-products-4.0.3/codenerix_products/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-products-4.0.2/django_codenerix_products.egg-info/PKG-INFO` & `django-codenerix-products-4.0.3/django_codenerix_products.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-products
-Version: 4.0.2
+Version: 4.0.3
 Summary: Codenerix Products is a module that enables CODENERIX to set products on serveral platforms in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-products
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,products
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-products-4.0.2/django_codenerix_products.egg-info/SOURCES.txt` & `django-codenerix-products-4.0.3/django_codenerix_products.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,41 +25,56 @@
 codenerix_products/migrations/0008_auto_20180126_1711.py
 codenerix_products/migrations/0009_auto_20180201_1137.py
 codenerix_products/migrations/0010_merge_20180202_0726.py
 codenerix_products/migrations/0011_auto_20180202_0826.py
 codenerix_products/migrations/0012_productunique_caducity.py
 codenerix_products/migrations/0013_alter_attribute_public_alter_brand_outstanding_and_more.py
 codenerix_products/migrations/__init__.py
+codenerix_products/migrations/__pycache__/0001_initial.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0001_initial.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0001_initial.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0002_auto_20180117_1628.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0003_auto_20180117_1655.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0004_auto_20180117_1745.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0005_auto_20180118_0739.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0006_auto_20180118_1126.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0007_auto_20180123_1316.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0007_product_caducable.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0008_auto_20180126_1711.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0009_auto_20180201_1137.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0010_merge_20180202_0726.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0011_auto_20180202_0826.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-35.pyc
 codenerix_products/migrations/__pycache__/0012_productunique_caducity.cpython-39.pyc
+codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-310.pyc
 codenerix_products/migrations/__pycache__/0013_alter_attribute_public_alter_brand_outstanding_and_more.cpython-39.pyc
+codenerix_products/migrations/__pycache__/__init__.cpython-310.pyc
 codenerix_products/migrations/__pycache__/__init__.cpython-35.pyc
 codenerix_products/migrations/__pycache__/__init__.cpython-39.pyc
 codenerix_products/static/codenerix_products/productfinals_sublist_rows.html
 codenerix_products/static/codenerix_products/js/app.js
 codenerix_products/static/codenerix_products/js/app_product.js
 codenerix_products/static/codenerix_products/js/controllers.js
 codenerix_products/static/codenerix_products/partials/products_list.html
```

### Comparing `django-codenerix-products-4.0.2/setup.py` & `django-codenerix-products-4.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 import os
 from setuptools import setup
 
 import codenerix_products
 
-with open(os.path.join(os.path.dirname(__file__), 'README.rst')) as readme:
+with open(os.path.join(os.path.dirname(__file__), "README.rst")) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
-    name='django-codenerix-products',
+    name="django-codenerix-products",
     version=codenerix_products.__version__,
     packages=["codenerix_products"],
     include_package_data=True,
     zip_safe=False,
-    license='Apache License Version 2.0',
-    description='Codenerix Products is a module that enables CODENERIX to set products on serveral platforms in a general manner.',
+    license="Apache License Version 2.0",
+    description="Codenerix Products is a module that enables CODENERIX to set products on serveral platforms in a general manner.",
     long_description=README,
-    url='https://github.com/codenerix/django-codenerix-products',
+    url="https://github.com/codenerix/django-codenerix-products",
     author=", ".join(codenerix_products.__authors__),
-    keywords=['django', 'codenerix', 'management', 'erp', 'crm', 'products'],
-    platforms=['OS Independent'],
+    keywords=["django", "codenerix", "management", "erp", "crm", "products"],
+    platforms=["OS Independent"],
     classifiers=[
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Framework :: Django :: 1.8',
-        'Framework :: Django :: 1.9',
-        'Framework :: Django :: 1.10',
-        'Intended Audience :: Developers',
-        'License :: Other/Proprietary License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Topic :: Internet :: WWW/HTTP',
-        'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
+        "Environment :: Web Environment",
+        "Framework :: Django",
+        "Framework :: Django :: 1.8",
+        "Framework :: Django :: 1.9",
+        "Framework :: Django :: 1.10",
+        "Intended Audience :: Developers",
+        "License :: Other/Proprietary License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Topic :: Internet :: WWW/HTTP",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
     install_requires=[
-        'django-codenerix',
-        'django-codenerix-extensions',
-    ]
+        "codenerix-lib",
+        "django-codenerix",
+        "django-codenerix-extensions",
+    ],
 )
```

