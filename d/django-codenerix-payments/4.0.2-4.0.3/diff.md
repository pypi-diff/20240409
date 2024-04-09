# Comparing `tmp/django-codenerix-payments-4.0.2.tar.gz` & `tmp/django-codenerix-payments-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-payments-4.0.2.tar", last modified: Thu Aug 18 06:18:12 2022, max compression
+gzip compressed data, was "django-codenerix-payments-4.0.3.tar", last modified: Tue Apr  9 07:53:59 2024, max compression
```

## Comparing `django-codenerix-payments-4.0.2.tar` & `django-codenerix-payments-4.0.3.tar`

### file list

```diff
@@ -1,105 +1,121 @@
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/LICENSE
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      401 2022-08-18 04:22:55.000000 django-codenerix-payments-4.0.2/MANIFEST.in
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3389 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1690 2022-07-15 06:45:44.000000 django-codenerix-payments-4.0.2/README.rst
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.701084 django-codenerix-payments-4.0.2/codenerix_payments/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      148 2022-08-18 04:23:07.000000 django-codenerix-payments-4.0.2/codenerix_payments/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      933 2022-05-17 12:36:29.000000 django-codenerix-payments-4.0.2/codenerix_payments/admin.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      152 2022-05-17 12:36:29.000000 django-codenerix-payments-4.0.2/codenerix_payments/apps.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2524 2022-08-18 04:07:38.000000 django-codenerix-payments-4.0.2/codenerix_payments/forms.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      925 2022-05-17 12:36:29.000000 django-codenerix-payments-4.0.2/codenerix_payments/helpers.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.697085 django-codenerix-payments-4.0.2/codenerix_payments/locale/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.697085 django-codenerix-payments-4.0.2/codenerix_payments/locale/en/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.701084 django-codenerix-payments-4.0.2/codenerix_payments/locale/en/LC_MESSAGES/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4331 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.697085 django-codenerix-payments-4.0.2/codenerix_payments/locale/es/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.701084 django-codenerix-payments-4.0.2/codenerix_payments/locale/es/LC_MESSAGES/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1974 2022-05-17 13:43:22.000000 django-codenerix-payments-4.0.2/codenerix_payments/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    10422 2022-07-15 06:51:06.000000 django-codenerix-payments-4.0.2/codenerix_payments/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.701084 django-codenerix-payments-4.0.2/codenerix_payments/management/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/management/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.705085 django-codenerix-payments-4.0.2/codenerix_payments/management/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      163 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      171 2022-05-17 13:55:31.000000 django-codenerix-payments-4.0.2/codenerix_payments/management/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.705085 django-codenerix-payments-4.0.2/codenerix_payments/management/commands/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/management/commands/__init__.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8067 2022-05-17 12:36:29.000000 django-codenerix-payments-4.0.2/codenerix_payments/management/commands/paypal_test.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11317 2022-05-17 12:36:29.000000 django-codenerix-payments-4.0.2/codenerix_payments/management/commands/redsys_test.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.709085 django-codenerix-payments-4.0.2/codenerix_payments/migrations/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     7121 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      589 2019-01-29 13:56:54.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0002_auto_20190109_0752.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      510 2019-08-06 06:11:26.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0003_auto_20190806_0808.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      680 2019-08-06 09:37:05.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0004_paymentrequest_user.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      528 2019-08-20 06:01:03.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0005_paymentrequest_feedback.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1066 2019-08-27 05:59:51.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0006_auto_20190827_0759.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      494 2020-04-29 11:31:05.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0007_auto_20200429_1331.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      707 2020-05-04 09:45:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0008_auto_20200504_1145.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1215 2020-07-06 08:26:06.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0009_auto_20200706_1013.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      551 2020-07-06 08:32:07.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0010_auto_20200706_1032.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      888 2022-08-18 04:40:41.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        0 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.713085 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4438 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3614 2022-05-17 13:55:09.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4568 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0001_squashed_0002_auto_20180526_1515.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      682 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0002_auto_20180526_1515.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      775 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      710 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      861 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      725 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      853 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      688 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      770 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1363 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      735 2022-08-18 04:24:48.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      854 2022-08-18 04:41:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      150 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      171 2022-05-17 13:55:09.000000 django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    99366 2022-08-18 06:05:27.000000 django-codenerix-payments-4.0.2/codenerix_payments/models.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.713085 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    11357 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/LICENSE
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1606 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/README.md
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       85 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.717085 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      153 2022-08-18 04:23:41.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.717085 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       85 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__init__.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      181 2019-08-06 09:27:12.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      162 2022-08-18 04:23:41.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6662 2019-08-06 09:27:12.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5912 2022-08-18 04:23:41.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4901 2019-08-06 09:27:13.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4338 2022-08-18 04:24:23.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8729 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/authorization.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    14911 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/encode.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8239 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/streaminghttp.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5630 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/yop_security_utils.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     8619 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/yp2util_rsa.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2513 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yop_sdk_config_default.json
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     5630 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yop_security_utils.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      593 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yp2const.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6024 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yp2const2.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     6354 2019-08-02 08:57:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yp2util.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.701084 django-codenerix-payments-4.0.2/codenerix_payments/static/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      624 2022-08-18 04:05:09.000000 django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/paymentsanswerlist_rows.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      614 2022-08-18 04:05:16.000000 django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/paymentsconfirmlist_rows.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     2304 2022-08-18 04:05:43.000000 django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/paymentslist_rows.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1461 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/paymentrequests_controllers.js
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.701084 django-codenerix-payments-4.0.2/codenerix_payments/templates/
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/codenerix_payments/templates/codenerix_payments/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)      925 2022-08-18 04:05:52.000000 django-codenerix-payments-4.0.2/codenerix_payments/templates/codenerix_payments/confirmation.html
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3317 2022-08-18 04:14:51.000000 django-codenerix-payments-4.0.2/codenerix_payments/urls.py
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)    20720 2022-08-18 05:01:03.000000 django-codenerix-payments-4.0.2/codenerix_payments/views.py
-drwxr-xr-x   0 br0th3r   (1000) br0th3r   (1000)        0 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     3389 2022-08-18 06:18:12.000000 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     4668 2022-08-18 06:18:12.000000 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-08-18 06:18:12.000000 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)        1 2022-05-17 11:43:32.000000 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       51 2022-08-18 06:18:12.000000 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       19 2022-08-18 06:18:12.000000 django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/top_level.txt
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)       38 2022-08-18 06:18:12.721085 django-codenerix-payments-4.0.2/setup.cfg
--rw-r--r--   0 br0th3r   (1000) br0th3r   (1000)     1822 2022-08-18 04:48:45.000000 django-codenerix-payments-4.0.2/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.680273 django-codenerix-payments-4.0.3/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:07:09.000000 django-codenerix-payments-4.0.3/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      401 2022-10-13 14:03:59.000000 django-codenerix-payments-4.0.3/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2569 2024-04-09 07:53:59.680273 django-codenerix-payments-4.0.3/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1428 2022-10-13 14:03:59.000000 django-codenerix-payments-4.0.3/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.664273 django-codenerix-payments-4.0.3/codenerix_payments/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-04-09 07:53:59.000000 django-codenerix-payments-4.0.3/codenerix_payments/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      933 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      152 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2524 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/forms.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      925 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/helpers.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.660273 django-codenerix-payments-4.0.3/codenerix_payments/locale/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.660273 django-codenerix-payments-4.0.3/codenerix_payments/locale/en/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.664273 django-codenerix-payments-4.0.3/codenerix_payments/locale/en/LC_MESSAGES/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4331 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.660273 django-codenerix-payments-4.0.3/codenerix_payments/locale/es/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.664273 django-codenerix-payments-4.0.3/codenerix_payments/locale/es/LC_MESSAGES/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1974 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    10422 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.664273 django-codenerix-payments-4.0.3/codenerix_payments/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.664273 django-codenerix-payments-4.0.3/codenerix_payments/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      163 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      171 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.668273 django-codenerix-payments-4.0.3/codenerix_payments/management/commands/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/management/commands/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     9351 2024-04-09 07:48:51.000000 django-codenerix-payments-4.0.3/codenerix_payments/management/commands/paypal_test.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13379 2024-04-09 07:52:55.000000 django-codenerix-payments-4.0.3/codenerix_payments/management/commands/redsys_test.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.668273 django-codenerix-payments-4.0.3/codenerix_payments/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7121 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      589 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0002_auto_20190109_0752.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      510 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0003_auto_20190806_0808.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      680 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0004_paymentrequest_user.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      528 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0005_paymentrequest_feedback.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1066 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0006_auto_20190827_0759.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      494 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0007_auto_20200429_1331.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      707 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0008_auto_20200504_1145.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1215 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0009_auto_20200706_1013.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      551 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0010_auto_20200706_1032.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      888 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.672273 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3601 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4438 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3614 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4568 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_squashed_0002_auto_20180526_1515.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      682 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0002_auto_20180526_1515.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      778 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      775 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      710 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      864 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      861 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      725 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      856 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      853 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      688 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      773 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      770 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1368 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1363 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      738 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      735 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      857 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      154 2023-01-29 13:03:07.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      150 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      171 2022-08-14 19:57:02.000000 django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    99366 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/models.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.672273 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11357 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1606 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/README.md
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       85 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      154 2023-01-29 13:03:04.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      153 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       85 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      163 2023-01-29 13:03:04.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      181 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      162 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5919 2023-01-29 13:03:04.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6662 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5912 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4335 2023-01-29 13:03:04.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4901 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4338 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8729 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/authorization.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    14911 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/encode.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8239 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/streaminghttp.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5630 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/yop_security_utils.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8619 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/yp2util_rsa.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2513 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yop_sdk_config_default.json
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5630 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yop_security_utils.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      593 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yp2const.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6024 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yp2const2.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6354 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yp2util.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.660273 django-codenerix-payments-4.0.3/codenerix_payments/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      624 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/paymentsanswerlist_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      614 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/paymentsconfirmlist_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2304 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/paymentslist_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1461 2020-05-15 23:37:49.000000 django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/paymentrequests_controllers.js
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.660273 django-codenerix-payments-4.0.3/codenerix_payments/templates/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/codenerix_payments/templates/codenerix_payments/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      925 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/templates/codenerix_payments/confirmation.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3317 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    20720 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/codenerix_payments/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-04-09 07:53:59.676273 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2569 2024-04-09 07:53:59.000000 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5982 2024-04-09 07:53:59.000000 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-04-09 07:53:59.000000 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:37:50.000000 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       51 2024-04-09 07:53:59.000000 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       19 2024-04-09 07:53:59.000000 django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-04-09 07:53:59.680273 django-codenerix-payments-4.0.3/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1749 2022-10-13 14:04:00.000000 django-codenerix-payments-4.0.3/setup.py
```

### Comparing `django-codenerix-payments-4.0.2/LICENSE` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/README.rst` & `django-codenerix-payments-4.0.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,19 @@
     :target: https://www.codenerix.com
     :alt: Try our demo with Codenerix Cloud
 
 ********
 Features
 ********
 
-* `Paypal <https://www.paypal.com/>`_
-* `Redsys <http://www.redsys.es/en/>`_
-
-*********
-Changelog
-*********
+This module support the next providers:
 
-2018-01-17 - Codenerix Payments v1.x is incompatible with v2.x, `what has changed and how to migrate to v2.x? <https://github.com/codenerix/django-codenerix-payments/wiki/Codenerix-Payments-version-1.x-is-icompatible-with-2.x>`_.
+* `Paypal <https://www.paypal.com/>`_
+* `Redsys <https://www.redsys.es/en/>`_
+* `Yeepay <https://yeepay.com/>`_
 
 ****
 Demo
 ****
 
 You can have a look to our demos online:
 
@@ -34,16 +31,15 @@
 
 **********
 Quickstart
 **********
 
 1. Install this package::
 
-    For python 2: sudo pip2 install django-codenerix-payments
-    For python 3: sudo pip3 install django-codenerix-payments
+    sudo pip3 install django-codenerix-payments
 
 2. Add "codenerix_payments" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [
         ...
         'codenerix_payments',
     ]
```

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/admin.py` & `django-codenerix-payments-4.0.3/codenerix_payments/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/forms.py` & `django-codenerix-payments-4.0.3/codenerix_payments/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/helpers.py` & `django-codenerix-payments-4.0.3/codenerix_payments/helpers.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/locale/en/LC_MESSAGES/django.po` & `django-codenerix-payments-4.0.3/codenerix_payments/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/locale/es/LC_MESSAGES/django.mo` & `django-codenerix-payments-4.0.3/codenerix_payments/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/locale/es/LC_MESSAGES/django.po` & `django-codenerix-payments-4.0.3/codenerix_payments/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/management/commands/paypal_test.py` & `django-codenerix-payments-4.0.3/codenerix_payments/management/commands/paypal_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,172 +19,236 @@
 # limitations under the License.
 
 
 import time
 
 from django.core.management.base import BaseCommand, CommandError
 
-from codenerix.lib.debugger import Debugger
-from codenerix_payments.models import PaymentRequest, PaymentConfirmation, Currency, PaymentError
+from codenerix_lib.debugger import Debugger
+from codenerix_payments.models import (
+    PaymentRequest,
+    PaymentConfirmation,
+    Currency,
+    PaymentError,
+)
 
 
 class Command(BaseCommand, Debugger):
-    
+
     # Show this when the user types help
     help = "Check paypal library and configuration"
-    
+
     def add_arguments(self, parser):
-        
+
         # Named (optional) arguments
         parser.add_argument(
-            '--action',
-            action='append',
-            dest='action',
-            help='Actions can be create, confirm or cancel'
+            "--action",
+            action="append",
+            dest="action",
+            help="Actions can be create, confirm or cancel",
         )
-        
+
         # Named (optional) arguments
         parser.add_argument(
-            '--id',
-            action='store',
-            dest='id',
+            "--id",
+            action="store",
+            dest="id",
             type=int,
-            help='ID of the action (except create)'
+            help="ID of the action (except create)",
         )
-        
+
         # Named (optional) arguments
         parser.add_argument(
-            '--url',
-            action='store',
-            dest='url',
-            help='Confirmation URL from the user to be used in confirm action if available'
+            "--url",
+            action="store",
+            dest="url",
+            help="Confirmation URL from the user to be used in "
+            "confirm action if available",
         )
-    
+
     def handle(self, *args, **options):
-        
+
         # Autoconfigure Debugger
         self.set_name("PAYPAL")
         self.set_debug()
-        
+
         # Config
         currency_id = "EUR"
-        
+
         # Arguments
-        actions = options['action']
+        actions = options["action"]
         alloptions = actions is None
         cid = None
         if not alloptions:
             for action in actions:
-                if action not in ['create', 'confirm', 'cancel']:
-                    raise CommandError("Unknow action '{}', you can use 'create', 'confirm' or 'cancel'".format(action))
-            if 'confirm' in actions and 'cancel' in actions:
-                raise CommandError("Cannot confirm and cancel at the same time")
-            for action in ['confirm', 'cancel']:
+                if action not in ["create", "confirm", "cancel"]:
+                    raise CommandError(
+                        f"Unknow action '{action}', you can use 'create', "
+                        "'confirm' or 'cancel'"
+                    )
+            if "confirm" in actions and "cancel" in actions:
+                raise CommandError(
+                    "Cannot confirm and cancel at the same time"
+                )
+            for action in ["confirm", "cancel"]:
                 if action in actions:
-                    cid = options['id']
+                    cid = options["id"]
                     if cid:
-                        self.debug("ID detected: {}".format(cid), color='cyan')
+                        self.debug("ID detected: {}".format(cid), color="cyan")
                         break
                     else:
-                        self.debug("ID required", color='red')
-                        raise CommandError('ID required')
-        
+                        self.debug("ID required", color="red")
+                        raise CommandError("ID required")
+
         # Set and get currency
         cs = Currency.objects.filter(iso4217=currency_id)
         if len(cs) == 0:
             c = Currency()
             c.name = "Euro"  # "Dollar"
             c.symbol = "€".decode("utf-8")  # "$"
             c.iso4217 = currency_id
-            c.price = 1.0   # 1.14
+            c.price = 1.0  # 1.14
             c.save()
             currency = c
         elif len(cs) == 1:
             currency = cs[0]
         else:
-            raise IOError("Currency {} found more than once".format(currency_id))
-        
+            raise IOError(
+                "Currency {} found more than once".format(currency_id)
+            )
+
         # Payment Request
-        if alloptions or 'create' in actions:
+        if alloptions or "create" in actions:
             self.debug("Creating Payment Request", color="yellow")
             pr = PaymentRequest()
             pr.order = int(time.time())
-            pr.reverse = 'reverse'
+            pr.reverse = "reverse"
             pr.currency = currency
             pr.platform = "paypalonline"
             pr.real = False
             pr.total = 12
             try:
                 pr.save()
-                self.debug("Payment Request: Created with ID '{}' and LOCATOR '{}'".format(pr.pk, pr.locator), color="green")
+                self.debug(
+                    f"Payment Request: Created with ID '{pr.pk}' "
+                    f"and LOCATOR '{pr.locator}'",
+                    color="green",
+                )
             except PaymentError as e:
-                self.debug("Payment Request: ERROR - {}".format(e), color="red")
+                self.debug(
+                    "Payment Request: ERROR - {}".format(e), color="red"
+                )
                 raise
         else:
             pr = PaymentRequest.objects.get(pk=cid)
-            self.debug("Payment Request: Restored ID '{}' and LOCATOR '{}' from database".format(pr.pk, pr.locator), color="green")
-        
+            self.debug(
+                f"Payment Request: Restored ID '{pr.pk}' "
+                f"and LOCATOR '{pr.locator}' from database",
+                color="green",
+            )
+
         # Check if payment hasn't been cancelled before
         if not pr.cancelled:
             # Get Authorization URL
-            if alloptions or 'confirm' in actions or 'cancel' in actions:
+            if alloptions or "confirm" in actions or "cancel" in actions:
                 # Get approval URL and show to user
                 try:
-                    self.debug("Approval URL: {}".format(pr.get_approval()['url']), color='cyan')
+                    self.debug(
+                        "Approval URL: {}".format(pr.get_approval()["url"]),
+                        color="cyan",
+                    )
                 except PaymentError as e:
-                    self.debug("Approval URL: ERROR - {}".format(e), color="red")
+                    self.debug(
+                        "Approval URL: ERROR - {}".format(e), color="red"
+                    )
                     raise
-                
+
                 # Get confirmation URL
-                if options['url']:
+                if options["url"]:
                     # Get confirmation URL from command line
-                    confirmation = options['url']
-                    self.debug("Using confirmation URL from command line: {}".format(confirmation), color='yellow')
+                    confirmation = options["url"]
+                    self.debug(
+                        "Using confirmation URL from command line: {}".format(
+                            confirmation
+                        ),
+                        color="yellow",
+                    )
                 else:
                     # Get confirmation
-                    self.debug("Visit approval URL and pay, then when Paypal drives you to our confirmation site, copy and paste the URL here", color='yellow')
-                    confirmation = raw_input("URL: ")
-                
+                    self.debug(
+                        "Visit approval URL and pay, then when Paypal drives "
+                        "you to our confirmation site, copy and paste the URL "
+                        "here",
+                        color="yellow",
+                    )
+                    confirmation = input("URL: ")
+
                 # If confirmation URL
-                if (len(confirmation.split("?")) > 1) and (len(confirmation.split("/")) > 1):
-                    
+                if (len(confirmation.split("?")) > 1) and (
+                    len(confirmation.split("/")) > 1
+                ):
+
                     # Process the confirmation URL
                     data = {}
                     for arg in confirmation.split("?")[1].split("&"):
                         (key, value) = arg.split("=")
                         data[key] = value
-                    
+
                     # Get action
                     action = confirmation.split("/")[-2]
-                    if action == 'confirm':
-                        if (not alloptions) and ('confirm' not in actions):
-                            raise CommandError("Not a normal flow payment and not a confirm payment action but URL you gave me was for a confirm payment: 1) or you gave me a mistaken URL, 2) or you told me to do a wrong action")
-                    elif action == 'cancel':
-                        if (not alloptions) and ('cancel' not in actions):
-                            raise CommandError("This is not a cancel payment action but the URL you gave me was for a cancel payment: 1) or you gave me a mistaken URL, 2) or you told me to do a wrong action")
+                    if action == "confirm":
+                        if (not alloptions) and ("confirm" not in actions):
+                            raise CommandError(
+                                "Not a normal flow payment and not a confirm "
+                                "payment action but URL you gave me was for "
+                                "a confirm payment: 1) or you gave me a "
+                                "mistaken URL, 2) or you told me to do a "
+                                "wrong action"
+                            )
+                    elif action == "cancel":
+                        if (not alloptions) and ("cancel" not in actions):
+                            raise CommandError(
+                                "This is not a cancel payment action but the "
+                                "URL you gave me was for a cancel payment: 1) "
+                                "or you gave me a mistaken URL, 2) or you "
+                                "told me to do a wrong action"
+                            )
                     else:
-                        raise CommandError("The URL that you gave me is not for a 'confirm' neither 'cancel' payment")
-                    
+                        raise CommandError(
+                            "The URL that you gave me is not for a 'confirm' "
+                            "neither 'cancel' payment"
+                        )
+
                     # Payment Confirm or Cancel
-                    if action == 'confirm':
+                    if action == "confirm":
                         self.debug("Confirm payment", color="blue")
                         pc = PaymentConfirmation()
                         try:
                             pc.confirm(pr, data)
                             self.debug("Payment confirmed", color="green")
                         except PaymentError as e:
-                            self.debug("Payment confirmed: ERROR - {}".format(e), color="red")
+                            self.debug(
+                                "Payment confirmed: ERROR - {}".format(e),
+                                color="red",
+                            )
                             raise
-                    elif action == 'cancel':
+                    elif action == "cancel":
                         # Payment Confirm
                         self.debug("Cancel payment", color="blue")
                         pc = PaymentConfirmation()
                         try:
                             pc.cancel(pr, data)
                             self.debug("Payment canceled", color="yellow")
                         except PaymentError as e:
-                            self.debug("Payment cancel: ERROR - {}".format(e), color="red")
+                            self.debug(
+                                "Payment cancel: ERROR - {}".format(e),
+                                color="red",
+                            )
                             raise
                 else:
-                    self.debug("No URL given: stopping process here", color='yellow')
+                    self.debug(
+                        "No URL given: stopping process here", color="yellow"
+                    )
         else:
-            raise CommandError("This payment has been cancelled previously, sorry!")
+            raise CommandError(
+                "This payment has been cancelled previously, sorry!"
+            )
```

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/management/commands/redsys_test.py` & `django-codenerix-payments-4.0.3/codenerix_payments/management/commands/redsys_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,225 +23,327 @@
 # Number: 4548 8120 4940 0004
 # Caducity: 12/20
 # CVV2: 123
 # CIP: 123456
 
 import os
 import time
-import commands
+import commands  # type: ignore
 import tempfile
 
 from django.core.management.base import BaseCommand, CommandError
 
-from codenerix.lib.debugger import Debugger
-from codenerix_payments.models import PaymentRequest, PaymentConfirmation, PaymentAnswer, Currency, PaymentError
+from codenerix_lib.debugger import Debugger
+from codenerix_payments.models import (
+    PaymentRequest,
+    PaymentConfirmation,
+    PaymentAnswer,
+    Currency,
+    PaymentError,
+)
 
 
 class Command(BaseCommand, Debugger):
-    
+
     # Show this when the user types help
     help = "Check Redsys library and configuration"
-    
+
     def add_arguments(self, parser):
-        
+
         # Named (optional) arguments
         parser.add_argument(
-            '--action',
-            action='append',
-            dest='action',
-            help='Actions can be create, success, confirm or cancel'
+            "--action",
+            action="append",
+            dest="action",
+            help="Actions can be create, success, confirm or cancel",
         )
-        
+
         # Named (optional) arguments
         parser.add_argument(
-            '--id',
-            action='store',
-            dest='id',
+            "--id",
+            action="store",
+            dest="id",
             type=int,
-            help='ID of the action (except create)'
+            help="ID of the action (except create)",
         )
-        
+
         # Named (optional) arguments
         parser.add_argument(
-            '--url',
-            action='store',
-            dest='url',
-            help='Confirmation URL from the user to be used in confirm action if available'
+            "--url",
+            action="store",
+            dest="url",
+            help="Confirmation URL from the user to be used in confirm "
+            "action if available",
         )
-    
+
     def handle(self, *args, **options):
-        
+
         # Autoconfigure Debugger
         self.set_name("REDSYS")
         self.set_debug()
-        
+
         # Config
         currency_id = "EUR"
-        
+
         # Arguments
-        actions = options['action']
+        actions = options["action"]
         alloptions = actions is None
         cid = None
         if not alloptions:
             for action in actions:
-                if action not in ['create', 'success', 'confirm', 'cancel']:
-                    raise CommandError("Unknow action '{}', you can use 'create', 'success', 'confirm' or 'cancel'".format(action))
-            if 'confirm' in actions and 'cancel' in actions:
-                raise CommandError("Cannot confirm and cancel at the same time")
-            for action in ['success', 'confirm', 'cancel']:
+                if action not in ["create", "success", "confirm", "cancel"]:
+                    raise CommandError(
+                        f"Unknow action '{action}', you can use 'create', "
+                        "'success', 'confirm' or 'cancel'"
+                    )
+            if "confirm" in actions and "cancel" in actions:
+                raise CommandError(
+                    "Cannot confirm and cancel at the same time"
+                )
+            for action in ["success", "confirm", "cancel"]:
                 if action in actions:
-                    cid = options['id']
+                    cid = options["id"]
                     if cid:
-                        self.debug("ID detected: {}".format(cid), color='cyan')
+                        self.debug("ID detected: {}".format(cid), color="cyan")
                         break
                     else:
-                        self.debug("ID required", color='red')
-                        raise CommandError('ID required')
-        
+                        self.debug("ID required", color="red")
+                        raise CommandError("ID required")
+
         # Set and get currency
         cs = Currency.objects.filter(iso4217=currency_id)
         if len(cs) == 0:
             c = Currency()
             c.name = "Euro"  # "Dollar"
             c.symbol = "€".decode("utf-8")  # "$"
             c.iso4217 = currency_id
-            c.price = 1.0   # 1.14
+            c.price = 1.0  # 1.14
             c.save()
             currency = c
         elif len(cs) == 1:
             currency = cs[0]
         else:
-            raise IOError("Currency {} found more than once".format(currency_id))
-        
+            raise IOError(
+                "Currency {} found more than once".format(currency_id)
+            )
+
         # Payment Request
-        if alloptions or 'create' in actions:
+        if alloptions or "create" in actions:
             self.debug("Creating Payment Request", color="yellow")
             pr = PaymentRequest()
             pr.order = int(time.time())
-            pr.reverse = 'reverse'
+            pr.reverse = "reverse"
             pr.currency = currency
             pr.platform = "redsys"
             pr.real = False
             pr.total = 12
             try:
                 pr.save()
-                self.debug("Payment Request: Created with ID '{}' and LOCATOR '{}'".format(pr.pk, pr.locator), color="green")
-            except PaymentError, e:
-                self.debug("Payment Request: ERROR - {}".format(e), color="red")
+                self.debug(
+                    f"Payment Request: Created with ID '{pr.pk}' "
+                    f"and LOCATOR '{pr.locator}'",
+                    color="green",
+                )
+            except PaymentError as e:
+                self.debug(
+                    "Payment Request: ERROR - {}".format(e), color="red"
+                )
                 raise
         else:
             pr = PaymentRequest.objects.get(pk=cid)
-            self.debug("Payment Request: Restored ID '{}' and LOCATOR '{}' from database".format(pr.pk, pr.locator), color="green")
-        
+            self.debug(
+                f"Payment Request: Restored ID '{pr.pk}' "
+                f"and LOCATOR '{pr.locator}' from database",
+                color="green",
+            )
+
         # Check if payment hasn't been cancelled before
         if not pr.cancelled:
             # Get Authorization URL
-            if alloptions or 'confirm' in actions or 'cancel' in actions:
+            if alloptions or "confirm" in actions or "cancel" in actions:
                 # Get approval URL and show to user
                 try:
-                    self.debug("Approval URL: {}".format(pr.get_approval()), color='cyan')
+                    self.debug(
+                        "Approval URL: {}".format(pr.get_approval()),
+                        color="cyan",
+                    )
                 except PaymentError as e:
-                    self.debug("Approval URL: ERROR - {}".format(e), color="red")
+                    self.debug(
+                        "Approval URL: ERROR - {}".format(e), color="red"
+                    )
                     raise
-                
+
                 # Get confirmation URL
-                if options['url']:
+                if options["url"]:
                     # Get confirmation URL from command line
-                    confirmation = options['url']
-                    self.debug("Using confirmation URL from command line: {}".format(confirmation), color='yellow')
+                    confirmation = options["url"]
+                    self.debug(
+                        "Using confirmation URL from command line: {}".format(
+                            confirmation
+                        ),
+                        color="yellow",
+                    )
                 else:
                     # Prepare to jump
-                    self.debug("Get Approval INFO", color='cyan')
+                    self.debug("Get Approval INFO", color="cyan")
                     info = pr.get_approval()
-                    
+
                     # Create a temporal filename
-                    (fd, filename) = tempfile.mkstemp(suffix='.html', prefix='pay_', text=True)
-                    
+                    (fd, filename) = tempfile.mkstemp(
+                        suffix=".html", prefix="pay_", text=True
+                    )
+
                     # Write to disk
-                    FILE = open(filename, 'w')
-                    FILE.write('<form action="' + info['url'] + '" method="POST">')
-                    for key in info['form']:
-                        FILE.write('<input type="hidden" name="' + key + '" value="' + info['form'][key] + '"/>')
-                    FILE.write('<input type="submit" value="PAGAR!">')
-                    FILE.write('</form>')
-                    FILE.close()
+                    fp = open(filename, "w")
+                    fp.write(
+                        '<form action="' + info["url"] + '" method="POST">'
+                    )
+                    for key in info["form"]:
+                        fp.write(
+                            '<input type="hidden" name="'
+                            + key
+                            + '" value="'
+                            + info["form"][key]
+                            + '"/>'
+                        )
+                    fp.write('<input type="submit" value="PAGAR!">')
+                    fp.write("</form>")
+                    fp.close()
                     os.close(fd)
-                    
+
                     # Call browser
-                    commands.getstatusoutput("google-chrome {}".format(filename))
-                    raw_input("When you are ready to keep going, hit enter!")
-                    
+                    commands.getstatusoutput(
+                        "google-chrome {}".format(filename)
+                    )
+                    input("When you are ready to keep going, hit enter!")
+
                     # Delete temporal file
                     os.unlink(filename)
-                    
+
                     # Get confirmation
-                    self.debug("Visit approval URL and pay, then when Redsys drives you to our confirmation site, copy and paste the URL here", color='yellow')
-                    confirmation = raw_input("URL: ")
-                
-                if (len(confirmation.split("?")) > 1) and (len(confirmation.split("/")) > 1):
-                    
+                    self.debug(
+                        "Visit approval URL and pay, then when Redsys drives "
+                        "you to our confirmation site, copy and paste the URL "
+                        "here",
+                        color="yellow",
+                    )
+                    confirmation = input("URL: ")
+
+                if (len(confirmation.split("?")) > 1) and (
+                    len(confirmation.split("/")) > 1
+                ):
+
                     # Get args
                     url = confirmation.split("?")[0]
                     args = confirmation.split("?")[1]
-                    
+
                     # Process the confirmation URL
                     data = {}
                     for arg in args.split("&"):
                         argsp = arg.split("=")
                         key = argsp[0]
-                        value = '='.join(argsp[1:])
+                        value = "=".join(argsp[1:])
                         data[key] = value
-                    
+
                     # Get action
                     action = url.split("/")[-2]
-                    if action == 'success':
-                        if (not alloptions) and ('success' not in actions):
-                            raise CommandError("Not a normal flow payment and not a confirm payment action but URL you gave me was for a success payment: 1) or you gave me a mistaken URL, 2) or you told me to do a wrong action")
-                    elif action == 'confirm':
-                        if (not alloptions) and ('confirm' not in actions):
-                            raise CommandError("Not a normal flow payment and not a confirm payment action but URL you gave me was for a success payment: 1) or you gave me a mistaken URL, 2) or you told me to do a wrong action")
-                    elif action == 'cancel':
-                        if (not alloptions) and ('cancel' not in actions):
-                            raise CommandError("This is not a cancel payment action but the URL you gave me was for a cancel payment: 1) or you gave me a mistaken URL, 2) or you told me to do a wrong action")
+                    if action == "success":
+                        if (not alloptions) and ("success" not in actions):
+                            raise CommandError(
+                                "Not a normal flow payment and not a confirm "
+                                "payment action but URL you gave me was "
+                                "for a success payment: 1) or you gave me "
+                                "a mistaken URL, 2) or you told me to do "
+                                "a wrong action"
+                            )
+                    elif action == "confirm":
+                        if (not alloptions) and ("confirm" not in actions):
+                            raise CommandError(
+                                "Not a normal flow payment and not a confirm "
+                                "payment action but URL you gave me was "
+                                "for a success payment: 1) or you gave me "
+                                "a mistaken URL, 2) or you told me to do "
+                                "a wrong action"
+                            )
+                    elif action == "cancel":
+                        if (not alloptions) and ("cancel" not in actions):
+                            raise CommandError(
+                                "This is not a cancel payment action but "
+                                "the URL you gave me was for a cancel "
+                                "payment: 1) or you gave me a mistaken "
+                                "URL, 2) or you told me to do a wrong action"
+                            )
                     else:
-                        raise CommandError("The URL that you gave me is not for a 'success' neither 'cancel' payment")
-                    
+                        raise CommandError(
+                            "The URL that you gave me is not for a 'success' "
+                            "neither 'cancel' payment"
+                        )
+
                     # Payment Confirm or Cancel
-                    if action == 'confirm':
+                    if action == "confirm":
                         self.debug("Confirm payment", color="blue")
                         pc = PaymentConfirmation()
                         try:
                             pc.confirm(pr, data)
                             self.debug("Payment confirmed", color="green")
                         except PaymentError as e:
-                            self.debug("Payment confirmed: ERROR - {}".format(e), color="red")
+                            self.debug(
+                                "Payment confirmed: ERROR - {}".format(e),
+                                color="red",
+                            )
                             raise
-                    elif action == 'cancel':
+                    elif action == "cancel":
                         # Payment Confirm
                         self.debug("Cancel payment", color="blue")
                         pc = PaymentConfirmation()
                         try:
                             pc.cancel(pr, data)
                             self.debug("Payment canceled", color="yellow")
                         except PaymentError as e:
-                            self.debug("Payment cancel: ERROR - {}".format(e), color="red")
+                            self.debug(
+                                "Payment cancel: ERROR - {}".format(e),
+                                color="red",
+                            )
                             raise
                 else:
-                    self.debug("No URL given: stopping process here", color='yellow')
-            
-            elif action == 'success':
+                    self.debug(
+                        "No URL given: stopping process here", color="yellow"
+                    )
+
+            elif action == "success":
                 self.debug("Remote system payment answered", color="blue")
                 pa = PaymentAnswer()
-                data = {u'Ds_Signature': [u'cURiymdHBZof0dhnWCHki7muP59t9o5SNJy5nVLrGew='], u'Ds_MerchantParameters': [u'eyJEc19EYXRlIjoiMjNcLzA4XC8yMDE2IiwiRHNfSG91ciI6IjE3OjUyIiwiRHNfU2VjdXJlUGF5bWVudCI6IjEiLCJEc19DYXJkX051bWJlciI6IjQ1NDg4MSoqKioqKjAwMDQiLCJEc19DYXJkX0NvdW50cnkiOiI3MjQiLCJEc19BbW91bnQiOiIxMjAwIiwiRHNfQ3VycmVuY3kiOiI5NzgiLCJEc19PcmRlciI6IjAwMDAwMDE1IiwiRHNfTWVyY2hhbnRDb2RlIjoiOTk5MDA4ODgxIiwiRHNfVGVybWluYWwiOiIwMDEiLCJEc19SZXNwb25zZSI6IjAwMDAiLCJEc19NZXJjaGFudERhdGEiOiIiLCJEc19UcmFuc2FjdGlvblR5cGUiOiIwIiwiRHNfQ29uc3VtZXJMYW5ndWFnZSI6IjEiLCJEc19BdXRob3Jpc2F0aW9uQ29kZSI6IjYyOTE3OCJ9'], u'Ds_SignatureVersion': [u'HMAC_SHA256_V1']}
+                data = {
+                    "Ds_Signature": [
+                        "cURiymdHBZof0dhnWCHki7muP59t9o5SNJy5nVLrGew="
+                    ],
+                    "Ds_MerchantParameters": [
+                        "eyJEc19EYXRlIjoiMjNcLzA4XC8yMDE2IiwiRHNfSG91ciI6IjE3OjUyIiwiRHNfU2VjdXJlUGF5bWVudCI6IjEiLCJEc19DYXJkX051bWJlciI6IjQ1NDg4MSoqKioqKjAwMDQiLCJEc19DYXJkX0NvdW50cnkiOiI3MjQiLCJEc19BbW91bnQiOiIxMjAwIiwiRHNfQ3VycmVuY3kiOiI5NzgiLCJEc19PcmRlciI6IjAwMDAwMDE1IiwiRHNfTWVyY2hhbnRDb2RlIjoiOTk5MDA4ODgxIiwiRHNfVGVybWluYWwiOiIwMDEiLCJEc19SZXNwb25zZSI6IjAwMDAiLCJEc19NZXJjaGFudERhdGEiOiIiLCJEc19UcmFuc2FjdGlvblR5cGUiOiIwIiwiRHNfQ29uc3VtZXJMYW5ndWFnZSI6IjEiLCJEc19BdXRob3Jpc2F0aW9uQ29kZSI6IjYyOTE3OCJ9"  # noqa: E501
+                    ],
+                    "Ds_SignatureVersion": ["HMAC_SHA256_V1"],
+                }
                 try:
                     pa.success(pr, data)
                 except PaymentError as e:
-                    self.debug("Payment not confirmed by the remote system: ERROR - {}".format(e), color="red")
+                    self.debug(
+                        "Payment not confirmed by the remote system: "
+                        f"ERROR - {e}",
+                        color="red",
+                    )
                     raise
-                
+
                 if not pa.error:
-                    self.debug("Payment successfully confirmed by the remote system", color="green")
+                    self.debug(
+                        "Payment successfully confirmed by the remote system",
+                        color="green",
+                    )
                 else:
-                    self.debug("Payment wrongly confirmed by the remote system: {}".format(pa.error_txt), color="red")
-                
+                    self.debug(
+                        "Payment wrongly confirmed by the remote "
+                        f"system: {pa.error_txt}",
+                        color="red",
+                    )
+
         else:
-            raise CommandError("This payment has been cancelled previously, sorry!")
+            raise CommandError(
+                "This payment has been cancelled previously, sorry!"
+            )
```

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0001_initial.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0002_auto_20190109_0752.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0002_auto_20190109_0752.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0004_paymentrequest_user.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0004_paymentrequest_user.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0005_paymentrequest_feedback.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0005_paymentrequest_feedback.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0006_auto_20190827_0759.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0006_auto_20190827_0759.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0008_auto_20200504_1145.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0008_auto_20200504_1145.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0009_auto_20200706_1013.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0009_auto_20200706_1013.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0010_auto_20200706_1032.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0010_auto_20200706_1032.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.py` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0001_squashed_0002_auto_20180526_1515.cpython-35.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0001_squashed_0002_auto_20180526_1515.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0002_auto_20180526_1515.cpython-35.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0002_auto_20180526_1515.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/models.py` & `django-codenerix-payments-4.0.3/codenerix_payments/models.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/LICENSE` & `django-codenerix-payments-4.0.3/LICENSE`

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

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/README.md` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/README.md`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-35.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-35.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-39.pyc` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/authorization.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/authorization.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/encode.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/encode.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/streaminghttp.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/streaminghttp.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/yop_security_utils.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/yop_security_utils.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/sign_rsa/yp2util_rsa.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/sign_rsa/yp2util_rsa.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yop_sdk_config_default.json` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yop_sdk_config_default.json`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yop_security_utils.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yop_security_utils.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yp2const.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yp2const.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yp2const2.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yp2const2.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/sdk_yeepay/yp2util.py` & `django-codenerix-payments-4.0.3/codenerix_payments/sdk_yeepay/yp2util.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/paymentsanswerlist_rows.html` & `django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/paymentsanswerlist_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/paymentsconfirmlist_rows.html` & `django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/paymentsconfirmlist_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/partials/paymentslist_rows.html` & `django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/partials/paymentslist_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/static/codenerix_payments/paymentrequests_controllers.js` & `django-codenerix-payments-4.0.3/codenerix_payments/static/codenerix_payments/paymentrequests_controllers.js`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/templates/codenerix_payments/confirmation.html` & `django-codenerix-payments-4.0.3/codenerix_payments/templates/codenerix_payments/confirmation.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/urls.py` & `django-codenerix-payments-4.0.3/codenerix_payments/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/codenerix_payments/views.py` & `django-codenerix-payments-4.0.3/codenerix_payments/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-payments-4.0.2/django_codenerix_payments.egg-info/SOURCES.txt` & `django-codenerix-payments-4.0.3/django_codenerix_payments.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -27,49 +27,65 @@
 codenerix_payments/migrations/0006_auto_20190827_0759.py
 codenerix_payments/migrations/0007_auto_20200429_1331.py
 codenerix_payments/migrations/0008_auto_20200504_1145.py
 codenerix_payments/migrations/0009_auto_20200706_1013.py
 codenerix_payments/migrations/0010_auto_20200706_1032.py
 codenerix_payments/migrations/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.py
 codenerix_payments/migrations/__init__.py
+codenerix_payments/migrations/__pycache__/0001_initial.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0001_initial.cpython-35.pyc
 codenerix_payments/migrations/__pycache__/0001_initial.cpython-39.pyc
 codenerix_payments/migrations/__pycache__/0001_squashed_0002_auto_20180526_1515.cpython-35.pyc
 codenerix_payments/migrations/__pycache__/0002_auto_20180526_1515.cpython-35.pyc
+codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0002_auto_20190109_0752.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0003_auto_20190806_0808.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0004_paymentrequest_user.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0005_paymentrequest_feedback.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0006_auto_20190827_0759.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0007_auto_20200429_1331.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0008_auto_20200504_1145.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0009_auto_20200706_1013.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0010_auto_20200706_1032.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/0011_alter_currency_price_alter_paymentrequest_reverse_and_more.cpython-39.pyc
+codenerix_payments/migrations/__pycache__/__init__.cpython-310.pyc
 codenerix_payments/migrations/__pycache__/__init__.cpython-35.pyc
 codenerix_payments/migrations/__pycache__/__init__.cpython-39.pyc
 codenerix_payments/sdk_yeepay/LICENSE
 codenerix_payments/sdk_yeepay/README.md
 codenerix_payments/sdk_yeepay/__init__.py
 codenerix_payments/sdk_yeepay/yop_sdk_config_default.json
 codenerix_payments/sdk_yeepay/yop_security_utils.py
 codenerix_payments/sdk_yeepay/yp2const.py
 codenerix_payments/sdk_yeepay/yp2const2.py
 codenerix_payments/sdk_yeepay/yp2util.py
+codenerix_payments/sdk_yeepay/__pycache__/__init__.cpython-310.pyc
 codenerix_payments/sdk_yeepay/__pycache__/__init__.cpython-39.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__init__.py
 codenerix_payments/sdk_yeepay/sign_rsa/authorization.py
 codenerix_payments/sdk_yeepay/sign_rsa/encode.py
 codenerix_payments/sdk_yeepay/sign_rsa/streaminghttp.py
 codenerix_payments/sdk_yeepay/sign_rsa/yop_security_utils.py
 codenerix_payments/sdk_yeepay/sign_rsa/yp2util_rsa.py
+codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-310.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-35.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/__init__.cpython-39.pyc
+codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-310.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-35.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/authorization.cpython-39.pyc
+codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-310.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-35.pyc
 codenerix_payments/sdk_yeepay/sign_rsa/__pycache__/yop_security_utils.cpython-39.pyc
 codenerix_payments/static/codenerix_payments/paymentrequests_controllers.js
 codenerix_payments/static/codenerix_payments/partials/paymentsanswerlist_rows.html
 codenerix_payments/static/codenerix_payments/partials/paymentsconfirmlist_rows.html
 codenerix_payments/static/codenerix_payments/partials/paymentslist_rows.html
 codenerix_payments/templates/codenerix_payments/confirmation.html
```

### Comparing `django-codenerix-payments-4.0.2/setup.py` & `django-codenerix-payments-4.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,26 +28,24 @@
         "crm",
         "payments",
     ],
     platforms=["OS Independent"],
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
-        "Framework :: Django :: 1.8",
-        "Framework :: Django :: 1.9",
-        "Framework :: Django :: 1.10",
+        "Framework :: Django :: 4.0",
         "Intended Audience :: Developers",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     ],
     install_requires=[
         "django-codenerix",
         "paypalrestsdk",
         "oss2",
```

