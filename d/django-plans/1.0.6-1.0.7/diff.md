# Comparing `tmp/django-plans-1.0.6.tar.gz` & `tmp/django-plans-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-1.0.6.tar", last modified: Wed Oct 11 14:21:21 2023, max compression
+gzip compressed data, was "django-plans-1.0.7.tar", last modified: Tue Apr  9 10:06:48 2024, max compression
```

## Comparing `django-plans-1.0.6.tar` & `django-plans-1.0.7.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.264299 django-plans-1.0.6/
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2023-10-11 14:21:20.000000 django-plans-1.0.6/.coveragerc
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4394 2023-10-11 14:21:20.000000 django-plans-1.0.6/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      343 2023-10-11 14:21:20.000000 django-plans-1.0.6/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      616 2023-10-11 14:21:20.000000 django-plans-1.0.6/.travis.yml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/.tx/
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-10-11 14:21:20.000000 django-plans-1.0.6/.tx/config
--rw-rw-r--   0 petr      (1000) petr      (1000)       83 2023-10-11 14:21:20.000000 django-plans-1.0.6/AUTHORS
--rw-rw-r--   0 petr      (1000) petr      (1000)     5430 2023-10-11 14:21:20.000000 django-plans-1.0.6/CHANGELOG
--rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2023-10-11 14:21:20.000000 django-plans-1.0.6/CODE_OF_CONDUCT.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2023-10-11 14:21:20.000000 django-plans-1.0.6/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-10-11 14:21:20.000000 django-plans-1.0.6/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1709 2023-10-11 14:21:21.264299 django-plans-1.0.6/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2023-10-11 14:21:20.000000 django-plans-1.0.6/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2023-10-11 14:21:20.000000 django-plans-1.0.6/conftest.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/foo/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/fixtures/initial_data.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/forms.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/foo/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      279 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/demo/example/foo/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/foo/templates/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)      591 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/templates/foo/foo_confirm_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/templates/foo/foo_form.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/templates/foo/foo_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      402 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/foo/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/demo/example/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/demo/example/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      378 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      714 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/demo/example/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      603 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      904 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/demo/example/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      495 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      804 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.232299 django-plans-1.0.6/demo/example/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      549 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      858 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.240299 django-plans-1.0.6/demo/example/sample_plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      160 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.244299 django-plans-1.0.6/demo/example/sample_plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      693 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/fixtures/test_django-plans_plans.json
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.244299 django-plans-1.0.6/demo/example/sample_plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.244299 django-plans-1.0.6/demo/example/sample_plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      119 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      117 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      116 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.244299 django-plans-1.0.6/demo/example/sample_plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    30867 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/demo/example/sample_plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.244299 django-plans-1.0.6/demo/example/sample_plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/sample_plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      744 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/sample_plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/templates/plans/upgrade.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/sample_plans/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/demo/example/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/static/css/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/static/css/example.css
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/demo/example/static/img/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/static/img/messages/
--rw-rw-r--   0 petr      (1000) petr      (1000)      294 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/static/img/messages/icon_alert.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/static/img/messages/icon_error.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/static/img/messages/icon_success.png
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/templates/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      823 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/templates/home.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      757 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      882 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/templates/plans/billing_info_update.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/demo/example/templates/registration/
--rw-rw-r--   0 petr      (1000) petr      (1000)      718 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/templates/registration/login.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      605 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1131 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/example/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/fabfile.py
--rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-10-11 14:21:20.000000 django-plans-1.0.6/demo/requirements.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/django_plans.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1709 2023-10-11 14:21:21.000000 django-plans-1.0.6/django_plans.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     8397 2023-10-11 14:21:21.000000 django-plans-1.0.6/django_plans.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-10-11 14:21:21.000000 django-plans-1.0.6/django_plans.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-10-11 14:21:21.000000 django-plans-1.0.6/django_plans.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-10-11 14:21:21.000000 django-plans-1.0.6/django_plans.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2023-10-11 14:21:21.000000 django-plans-1.0.6/django_plans.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.248299 django-plans-1.0.6/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.252299 django-plans-1.0.6/docs/source/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/docs/source/_static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.252299 django-plans-1.0.6/docs/source/_static/images/
--rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/_static/images/django-plans-1.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/_static/images/django-plans-2.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/_static/images/django-plans-3.png
--rw-rw-r--   0 petr      (1000) petr      (1000)      860 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/caveats.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/customize_models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1668 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/integration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/invoicing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/plans.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/plans_change.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      847 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/plans_expiration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2246 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/plans_recurrence.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/quota_validators.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/settings.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/south.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/taxation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2023-10-11 14:21:20.000000 django-plans-1.0.6/docs/source/templating.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      296 2023-10-11 14:21:20.000000 django-plans-1.0.6/fabfile.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.252299 django-plans-1.0.6/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     8840 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      277 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.252299 django-plans-1.0.6/plans/base/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/base/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    44931 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/base/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      273 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/context_processors.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/contrib.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/enumeration.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      678 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/fixtures/test_django-plans_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/forms.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      351 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/importer.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/listeners.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/plans/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/plans/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/plans/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/plans/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/plans/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      930 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      417 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      291 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      890 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0002_auto_20180901_1744.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0003_make_plans_unique.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      480 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0004_create_user_plans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0005_recurring_payments.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      665 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0006_auto_20200504_1541.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0007_recurringuserplan_card_masked_number.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      625 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0008_recurringuserplan_token_verified.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      456 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0009_auto_20210303_1134.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0010_auto_20220113_1317.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0011_auto_20220208_1344.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      531 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/0012_planpricing_visible.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/mixins.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3643 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/plan_change.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      308 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/quota.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/signals.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2079 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.256299 django-plans-1.0.6/plans/taxation/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/taxation/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/taxation/eu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/taxation/ru.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.236299 django-plans-1.0.6/plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.260299 django-plans-1.0.6/plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.260299 django-plans-1.0.6/plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.260299 django-plans-1.0.6/plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/templates/plans/upgrade.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.260299 django-plans-1.0.6/plans/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)       29 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2213 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/tests/test_autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    49156 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/tests/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    19429 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:21.264299 django-plans-1.0.6/plans_i18n/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      815 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       65 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      764 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/translation.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       26 2023-10-11 14:21:20.000000 django-plans-1.0.6/plans_i18n/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      371 2023-10-11 14:21:21.264299 django-plans-1.0.6/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2023-10-11 14:21:20.000000 django-plans-1.0.6/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      624 2023-10-11 14:21:20.000000 django-plans-1.0.6/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-09 10:06:47.000000 django-plans-1.0.7/.coveragerc
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.979654 django-plans-1.0.7/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4394 2024-04-09 10:06:47.000000 django-plans-1.0.7/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      343 2024-04-09 10:06:47.000000 django-plans-1.0.7/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      616 2024-04-09 10:06:47.000000 django-plans-1.0.7/.travis.yml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/.tx/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-09 10:06:47.000000 django-plans-1.0.7/.tx/config
+-rw-rw-r--   0 petr      (1000) petr      (1000)       83 2024-04-09 10:06:47.000000 django-plans-1.0.7/AUTHORS
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5506 2024-04-09 10:06:47.000000 django-plans-1.0.7/CHANGELOG
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2024-04-09 10:06:47.000000 django-plans-1.0.7/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2024-04-09 10:06:47.000000 django-plans-1.0.7/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-09 10:06:47.000000 django-plans-1.0.7/MANIFEST.in
+-rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-09 10:06:48.011654 django-plans-1.0.7/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2024-04-09 10:06:47.000000 django-plans-1.0.7/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2024-04-09 10:06:47.000000 django-plans-1.0.7/conftest.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/fixtures/initial_data.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/forms.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      279 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/foo/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/templates/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      591 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/templates/foo/foo_confirm_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/templates/foo/foo_form.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/templates/foo/foo_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      402 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      378 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      714 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      603 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      904 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      495 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      804 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      858 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      160 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      693 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_plans.json
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      119 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      117 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      116 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    30867 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/sample_plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/sample_plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      744 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/upgrade.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/css/example.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/static/img/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/static/img/messages/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      294 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/img/messages/icon_alert.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/img/messages/icon_error.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/img/messages/icon_success.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      823 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/home.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      757 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      882 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/plans/billing_info_update.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/templates/registration/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      718 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/registration/login.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      605 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1132 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/fabfile.py
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/django_plans.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8397 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.999654 django-plans-1.0.7/docs/source/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/docs/source/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.999654 django-plans-1.0.7/docs/source/_static/images/
+-rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/_static/images/django-plans-1.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/_static/images/django-plans-2.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/_static/images/django-plans-3.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)      860 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/caveats.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/customize_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1703 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/integration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/invoicing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans_change.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      847 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans_expiration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2246 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans_recurrence.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/quota_validators.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/south.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/taxation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/templating.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      296 2024-04-09 10:06:47.000000 django-plans-1.0.7/fabfile.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9052 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      277 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/base/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/base/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    46940 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/base/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      273 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/context_processors.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/contrib.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/enumeration.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/test_django-plans_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/forms.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      351 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/importer.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/listeners.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      930 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      417 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      291 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.007654 django-plans-1.0.7/plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      890 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0002_auto_20180901_1744.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0003_make_plans_unique.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      480 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0004_create_user_plans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0005_recurring_payments.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      665 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0006_auto_20200504_1541.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0007_recurringuserplan_card_masked_number.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      625 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0008_recurringuserplan_token_verified.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      456 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0009_auto_20210303_1134.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0010_auto_20220113_1317.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0011_auto_20220208_1344.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      531 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0012_planpricing_visible.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/mixins.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3643 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/plan_change.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/quota.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/signals.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2079 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.007654 django-plans-1.0.7/plans/taxation/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/taxation/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/taxation/eu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/taxation/ru.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.007654 django-plans-1.0.7/plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/upgrade.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       29 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2213 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/test_autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    58966 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    19429 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans_i18n/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      815 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       65 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      764 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/translation.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       26 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      371 2024-04-09 10:06:48.011654 django-plans-1.0.7/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2024-04-09 10:06:47.000000 django-plans-1.0.7/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      624 2024-04-09 10:06:47.000000 django-plans-1.0.7/tox.ini
```

### Comparing `django-plans-1.0.6/.coveragerc` & `django-plans-1.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/.github/workflows/main.yml` & `django-plans-1.0.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/.travis.yml` & `django-plans-1.0.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/CHANGELOG` & `django-plans-1.0.7/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 django-plans changelog
 ======================
 
+1.0.7 (unreleased)
+------------------
+* Add `AbstractOrder.return_order()`
+
 1.0.6
 -----
 * Simplify the query generated by get_initial_number
 
 1.0.5
 -----
 * Re-use old RecurringUserPlan in set_plan_renewal() to retain ID and history
```

### Comparing `django-plans-1.0.6/CODE_OF_CONDUCT.md` & `django-plans-1.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/LICENSE` & `django-plans-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/README.rst` & `django-plans-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/conftest.py` & `django-plans-1.0.7/conftest.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/foo/fixtures/initial_data.json` & `django-plans-1.0.7/demo/example/foo/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/foo/migrations/0001_initial.py` & `django-plans-1.0.7/demo/example/foo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/foo/templates/foo/foo_confirm_delete.html` & `django-plans-1.0.7/demo/example/foo/templates/foo/foo_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/foo/templates/foo/foo_form.html` & `django-plans-1.0.7/demo/example/foo/templates/foo/foo_form.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/foo/templates/foo/foo_list.html` & `django-plans-1.0.7/demo/example/foo/templates/foo/foo_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/foo/views.py` & `django-plans-1.0.7/demo/example/foo/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/locale/en/LC_MESSAGES/django.po` & `django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/fixtures/initial_plan.json` & `django-plans-1.0.7/demo/example/sample_plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/fixtures/test_django-plans_auth.json` & `django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/fixtures/test_django-plans_plans.json` & `django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/migrations/0001_initial.py` & `django-plans-1.0.7/demo/example/sample_plans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/models.py` & `django-plans-1.0.7/demo/example/sample_plans/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/mail/change_plan_body.txt` & `django-plans-1.0.7/demo/example/sample_plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/mail/expired_account_body.txt` & `django-plans-1.0.7/demo/example/sample_plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/mail/extend_account_body.txt` & `django-plans-1.0.7/demo/example/sample_plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/mail/remind_expire_body.txt` & `django-plans-1.0.7/demo/example/sample_plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/account_activation.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_create.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/billing_info_update.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/create_order.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/current.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/expiration_messages.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/extend.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/order_detail.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/order_detail_table.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/order_list.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/pagination.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/templates/plans/plan_table.html` & `django-plans-1.0.7/demo/example/sample_plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/sample_plans/tests.py` & `django-plans-1.0.7/demo/example/sample_plans/tests.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/settings.py` & `django-plans-1.0.7/demo/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/static/css/example.css` & `django-plans-1.0.7/demo/example/static/css/example.css`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/static/img/messages/icon_error.png` & `django-plans-1.0.7/demo/example/static/img/messages/icon_error.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/static/img/messages/icon_success.png` & `django-plans-1.0.7/demo/example/static/img/messages/icon_success.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/templates/base.html` & `django-plans-1.0.7/demo/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/templates/home.html` & `django-plans-1.0.7/demo/example/templates/home.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/templates/plans/billing_info_create.html` & `django-plans-1.0.7/demo/example/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/templates/plans/billing_info_update.html` & `django-plans-1.0.7/demo/example/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/templates/registration/login.html` & `django-plans-1.0.7/demo/example/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/urls.py` & `django-plans-1.0.7/demo/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/demo/example/wsgi.py` & `django-plans-1.0.7/demo/example/wsgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Usually you will have the standard Django WSGI application here, but it also
 might make sense to replace the whole Django WSGI application with a custom one
 that later delegates to the Django one. For example, you could introduce WSGI
 middleware here, or combine a Django application with an application of another
 framework.
 
 """
+
 import os
 
 from django.core.wsgi import get_wsgi_application
 
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "xmpl.settings")
 
 # This application object is used by any WSGI server configured to use this
```

### Comparing `django-plans-1.0.6/demo/manage.py` & `django-plans-1.0.7/demo/manage.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/django_plans.egg-info/SOURCES.txt` & `django-plans-1.0.7/django_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/Makefile` & `django-plans-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/_static/images/django-plans-1.png` & `django-plans-1.0.7/docs/source/_static/images/django-plans-1.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/_static/images/django-plans-2.png` & `django-plans-1.0.7/docs/source/_static/images/django-plans-2.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/_static/images/django-plans-3.png` & `django-plans-1.0.7/docs/source/_static/images/django-plans-3.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/caveats.rst` & `django-plans-1.0.7/docs/source/caveats.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/conf.py` & `django-plans-1.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/customize_models.rst` & `django-plans-1.0.7/docs/source/customize_models.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/index.rst` & `django-plans-1.0.7/docs/source/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 * Krzysztof Dorosz <cypreess@gmail.com>
 
 Contributors:
 
 * Victor Safronovich <vsafronovich@gmail.com>
 * Dominik Kozaczko <http://dominik.kozaczko.info>
 * Petr Dlouhý <petr.dlouhy@email.cz>
+* BlenderKit <info@blenderkit.com>
 
 Source code:
 https://github.com/cypreess/django-plans
 
 You are very welcome to join the development team of django-plans.
 Contribution via github fork and pull requests. Here are some ideas what is needed:
```

### Comparing `django-plans-1.0.6/docs/source/installation.rst` & `django-plans-1.0.7/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/integration.rst` & `django-plans-1.0.7/docs/source/integration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/invoicing.rst` & `django-plans-1.0.7/docs/source/invoicing.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/plans.rst` & `django-plans-1.0.7/docs/source/plans.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/plans_change.rst` & `django-plans-1.0.7/docs/source/plans_change.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/plans_expiration.rst` & `django-plans-1.0.7/docs/source/plans_expiration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/plans_recurrence.rst` & `django-plans-1.0.7/docs/source/plans_recurrence.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/quota_validators.rst` & `django-plans-1.0.7/docs/source/quota_validators.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/settings.rst` & `django-plans-1.0.7/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/south.rst` & `django-plans-1.0.7/docs/source/south.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/taxation.rst` & `django-plans-1.0.7/docs/source/taxation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/docs/source/templating.rst` & `django-plans-1.0.7/docs/source/templating.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/admin.py` & `django-plans-1.0.7/plans/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,14 +147,22 @@
     for order in queryset:
         order.complete_order()
 
 
 make_order_completed.short_description = _("Make selected orders completed")
 
 
+def make_order_returned(modeladmin, request, queryset):
+    for order in queryset:
+        order.return_order()
+
+
+make_order_returned.short_description = _("Make selected orders returned")
+
+
 def make_order_invoice(modeladmin, request, queryset):
     for order in queryset:
         if (
             Invoice.objects.filter(
                 type=Invoice.INVOICE_TYPES["INVOICE"], order=order
             ).count()
             == 0
@@ -188,15 +196,15 @@
         "plan",
         "pricing",
         "plan_extended_from",
         "plan_extended_until",
     )
     readonly_fields = ("created", "updated_at")
     list_display_links = list_display
-    actions = [make_order_completed, make_order_invoice]
+    actions = [make_order_completed, make_order_returned, make_order_invoice]
     inlines = (InvoiceInline,)
 
     def queryset(self, request):
         return (
             super(OrderAdmin, self)
             .queryset(request)
             .select_related("plan", "pricing", "user")
```

### Comparing `django-plans-1.0.6/plans/base/models.py` & `django-plans-1.0.7/plans/base/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,14 +306,21 @@
     def get_plan_extended_until(self, plan, pricing):
         if plan.is_free():
             return None
         if pricing is None:
             return self.expire
         return self.get_plan_extended_from(plan) + timedelta(days=pricing.period)
 
+    def get_plan_reduced_until(self, pricing):
+        if self.expire is None:
+            return self.expire
+        if pricing is None:
+            return self.expire
+        return self.expire - timedelta(days=pricing.period)
+
     def plan_autorenew_at(self):
         """
         Helper function which calculates when the plan autorenewal will occur
         """
         if self.expire:
             plans_autorenew_before_days = getattr(
                 settings, "PLANS_AUTORENEW_BEFORE_DAYS", 0
@@ -426,14 +433,24 @@
                     )
 
         if status:
             self.clean_activation()
 
         return status
 
+    def reduce_account(self, pricing):
+        """
+        Manages reducing account after returning an order
+        :param pricing: if pricing is None then nothing is changed
+        :return:
+        """
+        if pricing is not None:
+            self.expire = self.get_plan_reduced_until(pricing)
+            self.save()
+
     def expire_account(self):
         """manages account expiration"""
 
         self.deactivate()
 
         accounts_logger.info(
             "Account '%s' [id=%d] has expired" % (self.user, self.user.pk)
@@ -827,14 +844,42 @@
                 self.status = self.STATUS.NOT_VALID
             self.save()
             order_completed.send(self)
             return True
         else:
             return False
 
+    def return_order(self):
+        if self.status != self.STATUS.RETURNED:
+            if self.status == self.STATUS.COMPLETED:
+                if self.pricing is not None:
+                    extended_from = self.plan_extended_from
+                    if extended_from is None:
+                        extended_from = self.completed
+                    # Should never happen, but make sure we reduce for the same number of days as we extended.
+                    if (
+                        self.plan_extended_until is None
+                        or extended_from is None
+                        or self.plan_extended_until - extended_from
+                        != timedelta(days=self.pricing.period)
+                    ):
+                        raise ValueError(
+                            f"Invalid order state: completed={self.completed}, "
+                            f"plan_extended_from={self.plan_extended_from}, "
+                            f"plan_extended_until={self.plan_extended_until}, "
+                            f"pricing.period={self.pricing.period}"
+                        )
+                self.user.userplan.reduce_account(self.pricing)
+            elif self.status != self.STATUS.NOT_VALID:
+                raise ValueError(
+                    f"Cannot return order with status other than COMPLETED and NOT_VALID: {self.status}"
+                )
+            self.status = self.STATUS.RETURNED
+            self.save()
+
     def get_invoices_proforma(self):
         return AbstractInvoice.get_concrete_model().proforma.filter(order=self)
 
     def get_invoices(self):
         return AbstractInvoice.get_concrete_model().invoices.filter(order=self)
 
     def get_all_invoices(self):
```

### Comparing `django-plans-1.0.6/plans/context_processors.py` & `django-plans-1.0.7/plans/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/contrib.py` & `django-plans-1.0.7/plans/contrib.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/enumeration.py` & `django-plans-1.0.7/plans/enumeration.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/fixtures/initial_plan.json` & `django-plans-1.0.7/plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/fixtures/test_django-plans_auth.json` & `django-plans-1.0.7/plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/fixtures/test_django-plans_plans.json` & `django-plans-1.0.7/plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/forms.py` & `django-plans-1.0.7/plans/forms.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/listeners.py` & `django-plans-1.0.7/plans/listeners.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/en/LC_MESSAGES/django.po` & `django-plans-1.0.7/plans/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/pt_BR/LC_MESSAGES/django.mo` & `django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/management/commands/autorenew_accounts.py` & `django-plans-1.0.7/plans/management/commands/autorenew_accounts.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0001_initial.py` & `django-plans-1.0.7/plans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0002_auto_20180901_1744.py` & `django-plans-1.0.7/plans/migrations/0002_auto_20180901_1744.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0003_make_plans_unique.py` & `django-plans-1.0.7/plans/migrations/0003_make_plans_unique.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0005_recurring_payments.py` & `django-plans-1.0.7/plans/migrations/0005_recurring_payments.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0006_auto_20200504_1541.py` & `django-plans-1.0.7/plans/migrations/0006_auto_20200504_1541.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0008_recurringuserplan_token_verified.py` & `django-plans-1.0.7/plans/migrations/0008_recurringuserplan_token_verified.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0010_auto_20220113_1317.py` & `django-plans-1.0.7/plans/migrations/0010_auto_20220113_1317.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0011_auto_20220208_1344.py` & `django-plans-1.0.7/plans/migrations/0011_auto_20220208_1344.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/migrations/0012_planpricing_visible.py` & `django-plans-1.0.7/plans/migrations/0012_planpricing_visible.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/mixins.py` & `django-plans-1.0.7/plans/mixins.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/models.py` & `django-plans-1.0.7/plans/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/plan_change.py` & `django-plans-1.0.7/plans/plan_change.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/signals.py` & `django-plans-1.0.7/plans/signals.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/tasks.py` & `django-plans-1.0.7/plans/tasks.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/taxation/__init__.py` & `django-plans-1.0.7/plans/taxation/__init__.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/taxation/eu.py` & `django-plans-1.0.7/plans/taxation/eu.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/taxation/ru.py` & `django-plans-1.0.7/plans/taxation/ru.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/mail/change_plan_body.txt` & `django-plans-1.0.7/plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/mail/expired_account_body.txt` & `django-plans-1.0.7/plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/mail/extend_account_body.txt` & `django-plans-1.0.7/plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/mail/remind_expire_body.txt` & `django-plans-1.0.7/plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/account_activation.html` & `django-plans-1.0.7/plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.0.7/plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/create_order.html` & `django-plans-1.0.7/plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/current.html` & `django-plans-1.0.7/plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/expiration_messages.html` & `django-plans-1.0.7/plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/extend.html` & `django-plans-1.0.7/plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.0.7/plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.0.7/plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/order_detail.html` & `django-plans-1.0.7/plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/order_detail_table.html` & `django-plans-1.0.7/plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/order_list.html` & `django-plans-1.0.7/plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/pagination.html` & `django-plans-1.0.7/plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/templates/plans/plan_table.html` & `django-plans-1.0.7/plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/tests/test_autorenew_accounts.py` & `django-plans-1.0.7/plans/tests/test_autorenew_accounts.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/tests/test_views.py` & `django-plans-1.0.7/plans/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/tests/tests.py` & `django-plans-1.0.7/plans/tests/tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import random
-from datetime import date, timedelta
+import re
+from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from io import StringIO
 from unittest import mock
 from unittest.mock import patch
 
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.messages.storage.fallback import FallbackStorage
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.core import mail
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.core.management import call_command
 from django.db import transaction
-from django.db.models import Q
+from django.db.models import Exists, OuterRef, Q
 from django.test import RequestFactory, TestCase, TransactionTestCase, override_settings
 from django.urls import reverse
 from django_concurrent_tests.helpers import call_concurrently
 from freezegun import freeze_time
 from internet_sabotage import no_connection
 from model_bakery import baker
 
 from plans import tasks
 from plans.base.models import (
     AbstractBillingInfo,
     AbstractInvoice,
     AbstractOrder,
     AbstractPlan,
     AbstractPlanPricing,
+    AbstractPricing,
     AbstractUserPlan,
 )
 from plans.plan_change import PlanChangePolicy, StandardPlanChangePolicy
 from plans.quota import get_user_quota
 from plans.taxation.eu import EUTaxationPolicy
 from plans.validators import ModelCountValidator
 from plans.views import CreateOrderView
@@ -40,14 +42,15 @@
 User = get_user_model()
 BillingInfo = AbstractBillingInfo.get_concrete_model()
 PlanPricing = AbstractPlanPricing.get_concrete_model()
 Invoice = AbstractInvoice.get_concrete_model()
 Order = AbstractOrder.get_concrete_model()
 Plan = AbstractPlan.get_concrete_model()
 UserPlan = AbstractUserPlan.get_concrete_model()
+Pricing = AbstractPricing.get_concrete_model()
 
 
 class PlansTestCase(TestCase):
     fixtures = ["initial_plan", "test_django-plans_auth", "test_django-plans_plans"]
 
     def setUp(self):
         mail.outbox = []
@@ -207,14 +210,45 @@
         default_plan = Plan.objects.get(pk=1)
         u.userplan.extend_account(plan_pricing.plan, plan_pricing.pricing)
         self.assertEqual(u.userplan.expire, date.today() + timedelta(days=5))
         self.assertEqual(u.userplan.plan, default_plan)
         self.assertEqual(u.userplan.active, False)
         self.assertEqual(len(mail.outbox), 0)
 
+    def test_reduce_account_future(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.save()
+        pricing = Pricing.objects.get(planpricing__plan=u.userplan.plan, period=30)
+        u.userplan.reduce_account(pricing)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=20))
+
+    def test_reduce_account_before(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() - timedelta(days=50)
+        u.save()
+        pricing = Pricing.objects.get(planpricing__plan=u.userplan.plan, period=30)
+        u.userplan.reduce_account(pricing)
+        self.assertEqual(u.userplan.expire, date.today() - timedelta(days=80))
+
+    def test_reduce_account_expire_none(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = None
+        u.save()
+        pricing = Pricing.objects.get(planpricing__plan=u.userplan.plan, period=30)
+        u.userplan.reduce_account(pricing)
+        self.assertIsNone(u.userplan.expire)
+
+    def test_reduce_account_pricing_none(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.save()
+        u.userplan.reduce_account(None)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50))
+
     def test_expire_account(self):
         u = User.objects.get(username="test1")
         u.userplan.expire = date.today() + timedelta(days=50)
         u.userplan.active = True
         u.userplan.save()
         u.userplan.expire_account()
         self.assertEqual(u.userplan.active, False)
@@ -820,14 +854,243 @@
             pricing=plan_pricing.pricing,
             amount=100,
             plan=plan_pricing.plan,
             completed=date(2010, 10, 10),
         )
         self.assertFalse(order.complete_order())
 
+    def test_return_order_new(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.filter(
+            plan=u.userplan.plan, pricing__period__gt=0
+        ).first()
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+
+        with self.assertRaisesRegex(
+            ValueError,
+            rf"^Cannot return order with status other than COMPLETED and NOT_VALID: "
+            rf"{re.escape(str(Order.STATUS.NEW))}$",
+        ):
+            order.return_order()
+        self.assertEqual(order.status, Order.STATUS.NEW)
+        self.assertEqual(u.userplan.plan, plan_pricing.plan)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50))
+
+    def test_return_order_completed(self):
+        u = User.objects.get(username="test1")
+        u.userplan.plan = Plan.objects.filter(planpricing__isnull=True).first()
+        u.userplan.expire = None
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.filter(pricing__period__gt=0).first()
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+        order.complete_order()
+
+        order.return_order()
+
+        self.assertEqual(order.status, Order.STATUS.RETURNED)
+        self.assertEqual(u.userplan.plan, plan_pricing.plan)
+        self.assertEqual(u.userplan.expire, date.today())
+
+    def test_return_order_completed_then_same_plan(self):
+        u = User.objects.get(username="test1")
+        u.userplan.plan = (
+            Plan.objects.annotate(
+                planpricing_pricing_period_eq_30_exists=Exists(
+                    PlanPricing.objects.filter(plan=OuterRef("pk"), pricing__period=30)
+                ),
+                planpricing_pricing_period_gt_30_exists=Exists(
+                    PlanPricing.objects.filter(
+                        plan=OuterRef("pk"), pricing__period__gt=30
+                    )
+                ),
+            )
+            .filter(
+                planpricing_pricing_period_eq_30_exists=True,
+                planpricing_pricing_period_gt_30_exists=True,
+            )
+            .first()
+        )
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.filter(
+            plan=u.userplan.plan, pricing__period__gt=30
+        ).first()
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+        order.complete_order()
+        plan_pricing_then = PlanPricing.objects.get(
+            plan=plan_pricing.plan, pricing__period=30
+        )
+        order_then = Order.objects.create(
+            user=u,
+            pricing=plan_pricing_then.pricing,
+            amount=100,
+            plan=plan_pricing_then.plan,
+            status=Order.STATUS.NEW,
+        )
+        order_then.complete_order()
+
+        order.return_order()
+
+        self.assertEqual(order.status, Order.STATUS.RETURNED)
+        self.assertEqual(u.userplan.plan, plan_pricing_then.plan)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50 + 30))
+
+    def test_return_order_completed_then_paid_plan(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+        order.complete_order()
+        plan_pricing_then = (
+            PlanPricing.objects.exclude(plan=plan_pricing.plan)
+            .filter(pricing__period=365)
+            .first()
+        )
+        order_then = Order.objects.create(
+            user=u,
+            pricing=plan_pricing_then.pricing,
+            amount=100,
+            plan=plan_pricing_then.plan,
+            status=Order.STATUS.NEW,
+        )
+        with freeze_time(datetime.combine(u.userplan.expire, time())):
+            order_then.complete_order()
+
+        order.return_order()
+
+        self.assertEqual(order.status, Order.STATUS.RETURNED)
+        self.assertEqual(u.userplan.plan, plan_pricing_then.plan)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50 + 365))
+
+    def test_return_order_completed_then_free_plan(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.get(plan=u.userplan.plan, pricing__period=30)
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+        order.complete_order()
+        plan_then = (
+            Plan.objects.exclude(pk=plan_pricing.plan.pk)
+            .filter(planpricing__isnull=True)
+            .first()
+        )
+        u.userplan.extend_account(plan_then, None)
+
+        order.return_order()
+
+        self.assertEqual(order.status, Order.STATUS.RETURNED)
+        self.assertEqual(u.userplan.plan, plan_then)
+        self.assertIsNone(u.userplan.expire)
+
+    def test_return_order_not_valid(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_user = u.userplan.plan
+        plan_pricing = (
+            PlanPricing.objects.exclude(plan=u.userplan.plan)
+            .filter(pricing__period__gt=0)
+            .first()
+        )
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+        order.complete_order()
+
+        order.return_order()
+
+        self.assertEqual(order.status, Order.STATUS.RETURNED)
+        self.assertEqual(u.userplan.plan, plan_user)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50))
+
+    def test_return_order_canceled(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.filter(
+            plan=u.userplan.plan, pricing__period__gt=0
+        ).first()
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.CANCELED,
+        )
+
+        with self.assertRaisesRegex(
+            ValueError,
+            rf"^Cannot return order with status other than COMPLETED and NOT_VALID: "
+            rf"{re.escape(str(Order.STATUS.CANCELED))}$",
+        ):
+            order.return_order()
+        self.assertEqual(order.status, Order.STATUS.CANCELED)
+        self.assertEqual(u.userplan.plan, plan_pricing.plan)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50))
+
+    def test_return_order_returned(self):
+        u = User.objects.get(username="test1")
+        u.userplan.expire = date.today() + timedelta(days=50)
+        u.userplan.save()
+        plan_pricing = PlanPricing.objects.filter(
+            plan=u.userplan.plan, pricing__period__gt=0
+        ).first()
+        order = Order.objects.create(
+            user=u,
+            pricing=plan_pricing.pricing,
+            amount=100,
+            plan=plan_pricing.plan,
+            status=Order.STATUS.NEW,
+        )
+        order.complete_order()
+        order.return_order()
+
+        order.return_order()
+
+        self.assertEqual(order.status, Order.STATUS.RETURNED)
+        self.assertEqual(u.userplan.plan, plan_pricing.plan)
+        self.assertEqual(u.userplan.expire, date.today() + timedelta(days=50))
+
     def test_amount_taxed_none(self):
         o = Order()
         o.amount = Decimal(123)
         o.tax = None
         self.assertEqual(o.total(), Decimal("123"))
 
     def test_amount_taxed_0(self):
```

### Comparing `django-plans-1.0.6/plans/urls.py` & `django-plans-1.0.7/plans/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/utils.py` & `django-plans-1.0.7/plans/utils.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/validators.py` & `django-plans-1.0.7/plans/validators.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans/views.py` & `django-plans-1.0.7/plans/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans_i18n/README.rst` & `django-plans-1.0.7/plans_i18n/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans_i18n/admin.py` & `django-plans-1.0.7/plans_i18n/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/plans_i18n/translation.py` & `django-plans-1.0.7/plans_i18n/translation.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/setup.py` & `django-plans-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.6/tox.ini` & `django-plans-1.0.7/tox.ini`

 * *Files identical despite different names*

