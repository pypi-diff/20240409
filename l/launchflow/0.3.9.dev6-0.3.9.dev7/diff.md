# Comparing `tmp/launchflow-0.3.9.dev6.tar.gz` & `tmp/launchflow-0.3.9.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchflow-0.3.9.dev6.tar", last modified: Sun Apr  7 23:54:42 2024, max compression
+gzip compressed data, was "launchflow-0.3.9.dev7.tar", last modified: Tue Apr  9 01:29:21 2024, max compression
```

## Comparing `launchflow-0.3.9.dev6.tar` & `launchflow-0.3.9.dev7.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.242891 launchflow-0.3.9.dev6/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      118 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/MANIFEST.in
--rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-07 23:54:42.242891 launchflow-0.3.9.dev6/PKG-INFO
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1996 2024-03-13 23:12:43.000000 launchflow-0.3.9.dev6/README.md
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.214890 launchflow-0.3.9.dev6/launchflow/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      528 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.214890 launchflow-0.3.9.dev6/launchflow/aws/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       67 2024-03-20 15:00:34.000000 launchflow-0.3.9.dev6/launchflow/aws/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4480 2024-04-04 22:30:13.000000 launchflow-0.3.9.dev6/launchflow/aws/rds.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3512 2024-04-02 20:56:37.000000 launchflow-0.3.9.dev6/launchflow/aws/s3.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.214890 launchflow-0.3.9.dev6/launchflow/cache/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       95 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/cache/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4980 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cache/launchflow_tmp.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-25 20:38:50.000000 launchflow-0.3.9.dev6/launchflow/cli/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/accounts/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/accounts/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1250 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/accounts/account_commands.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/config/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/config/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1026 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/config/config_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      566 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/constants.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/environments/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/environments/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2535 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/environments/environment_commands.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2692 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      209 2024-04-02 23:44:00.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.218890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      216 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    15518 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:53:05.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      162 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      100 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      748 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      151 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      487 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      264 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2021 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.222890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:52:02.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      164 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      326 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    14570 2024-04-05 00:17:09.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/django_template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      217 2024-04-02 23:47:30.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17805 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.226890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      576 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      573 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    18560 2024-04-05 00:17:11.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/fastapi_template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      215 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17114 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.230890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      297 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:33.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      324 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17509 2024-04-05 00:17:00.000000 launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/flask_template.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    19278 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/main.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/project/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-30 20:01:40.000000 launchflow-0.3.9.dev6/launchflow/cli/project/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1702 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/cli/project/project_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3067 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/project_gen.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/resources/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/cli/resources/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4436 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/resources/resource_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5382 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/cli/resources_ast.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.234890 launchflow-0.3.9.dev6/launchflow/cli/services/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/cli/services/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4413 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/cli/services/service_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3501 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/cli/utils.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      482 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/cli/utyper.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/clients/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      296 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1155 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/accounts_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1137 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev6/launchflow/clients/client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1832 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/connect_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4806 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/clients/environments_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1911 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/operations_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1820 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/clients/projects_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5117 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/resources_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3767 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/response_schemas.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3477 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/clients/services_client.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/config/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/config/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4412 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/config/launchflow_config.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1361 2024-04-03 22:09:55.000000 launchflow-0.3.9.dev6/launchflow/config/launchflow_env.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5144 2024-03-14 16:50:08.000000 launchflow-0.3.9.dev6/launchflow/config/launchflow_yaml.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/context/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-03-13 17:41:44.000000 launchflow-0.3.9.dev6/launchflow/context/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    16535 2024-04-03 22:10:20.000000 launchflow-0.3.9.dev6/launchflow/context/launchflow_ctx.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/exceptions.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5180 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev6/launchflow/fastapi.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       52 2024-03-27 23:08:23.000000 launchflow-0.3.9.dev6/launchflow/flask.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/flows/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      129 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev6/launchflow/flows/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1236 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/flows/account_id.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3746 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/flows/auth.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    27648 2024-04-06 20:06:09.000000 launchflow-0.3.9.dev6/launchflow/flows/cloud_provider.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     7171 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev6/launchflow/flows/environments_flows.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev6/launchflow/flows/project_flows.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    18602 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev6/launchflow/flows/resource_flows.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow/gcp/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      219 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     7762 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/cloudsql.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2978 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/compute_engine.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3523 2024-04-02 20:56:22.000000 launchflow-0.3.9.dev6/launchflow/gcp/gcs.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2755 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev6/launchflow/gcp/memorystore.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2578 2024-04-05 21:08:46.000000 launchflow-0.3.9.dev6/launchflow/gcp/utils.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2059 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev6/launchflow/operations.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2288 2024-04-02 21:12:53.000000 launchflow-0.3.9.dev6/launchflow/resource.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       50 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev6/launchflow/service.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      789 2024-03-28 23:07:50.000000 launchflow-0.3.9.dev6/launchflow/utils.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-07 23:54:42.238891 launchflow-0.3.9.dev6/launchflow.egg-info/
--rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/PKG-INFO
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     8331 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/SOURCES.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        1 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/dependency_links.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       84 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/entry_points.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      309 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/requires.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       11 2024-04-07 23:54:42.000000 launchflow-0.3.9.dev6/launchflow.egg-info/top_level.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1421 2024-04-07 23:54:33.000000 launchflow-0.3.9.dev6/pyproject.toml
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       38 2024-04-07 23:54:42.242891 launchflow-0.3.9.dev6/setup.cfg
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.481048 launchflow-0.3.9.dev7/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      118 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/MANIFEST.in
+-rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-09 01:29:21.481048 launchflow-0.3.9.dev7/PKG-INFO
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1996 2024-03-13 23:12:43.000000 launchflow-0.3.9.dev7/README.md
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.453048 launchflow-0.3.9.dev7/launchflow/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      528 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.457048 launchflow-0.3.9.dev7/launchflow/aws/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       67 2024-03-20 15:00:34.000000 launchflow-0.3.9.dev7/launchflow/aws/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4480 2024-04-04 22:30:13.000000 launchflow-0.3.9.dev7/launchflow/aws/rds.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3512 2024-04-02 20:56:37.000000 launchflow-0.3.9.dev7/launchflow/aws/s3.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.457048 launchflow-0.3.9.dev7/launchflow/cache/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       95 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev7/launchflow/cache/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4980 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cache/launchflow_tmp.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.457048 launchflow-0.3.9.dev7/launchflow/cli/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-25 20:38:50.000000 launchflow-0.3.9.dev7/launchflow/cli/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.457048 launchflow-0.3.9.dev7/launchflow/cli/accounts/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev7/launchflow/cli/accounts/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1250 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/accounts/account_commands.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.457048 launchflow-0.3.9.dev7/launchflow/cli/config/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev7/launchflow/cli/config/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1026 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/config/config_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      566 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/constants.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/environments/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev7/launchflow/cli/environments/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2535 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/environments/environment_commands.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2692 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      209 2024-04-02 23:44:00.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      216 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    15518 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:53:05.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      162 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      100 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.461048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      748 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      151 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      487 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      264 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2021 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.465048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.465048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:52:02.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.465048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      164 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      326 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.465048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    14570 2024-04-05 00:17:09.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/django_template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.469048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.469048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      217 2024-04-02 23:47:30.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17805 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.469048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.469048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      576 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.469048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.473048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      573 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    18560 2024-04-05 00:17:11.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/fastapi_template.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.473048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/__init__.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.473048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/__pycache__/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      215 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17114 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.473048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.473048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      297 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.473048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:33.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/app/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      324 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    17509 2024-04-05 00:17:00.000000 launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/flask_template.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    19278 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/main.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/cli/project/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-30 20:01:40.000000 launchflow-0.3.9.dev7/launchflow/cli/project/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1702 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/cli/project/project_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3067 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/project_gen.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/cli/resources/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev7/launchflow/cli/resources/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4436 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/resources/resource_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5382 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/cli/resources_ast.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/cli/services/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/cli/services/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4413 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/cli/services/service_commands.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3501 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev7/launchflow/cli/utils.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      482 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/cli/utyper.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/clients/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      296 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/clients/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1155 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/clients/accounts_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1137 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev7/launchflow/clients/client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1832 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/clients/connect_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4806 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/clients/environments_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1911 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/clients/operations_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1820 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/clients/projects_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5117 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/clients/resources_client.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3767 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/clients/response_schemas.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3477 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/clients/services_client.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/config/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev7/launchflow/config/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4412 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev7/launchflow/config/launchflow_config.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1361 2024-04-03 22:09:55.000000 launchflow-0.3.9.dev7/launchflow/config/launchflow_env.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5144 2024-03-14 16:50:08.000000 launchflow-0.3.9.dev7/launchflow/config/launchflow_yaml.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.477048 launchflow-0.3.9.dev7/launchflow/context/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-03-13 17:41:44.000000 launchflow-0.3.9.dev7/launchflow/context/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    16535 2024-04-03 22:10:20.000000 launchflow-0.3.9.dev7/launchflow/context/launchflow_ctx.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/exceptions.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     5180 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev7/launchflow/fastapi.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       52 2024-03-27 23:08:23.000000 launchflow-0.3.9.dev7/launchflow/flask.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.481048 launchflow-0.3.9.dev7/launchflow/flows/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      129 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev7/launchflow/flows/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1236 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/flows/account_id.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3746 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/flows/auth.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    31282 2024-04-09 01:28:38.000000 launchflow-0.3.9.dev7/launchflow/flows/cloud_provider.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     7171 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev7/launchflow/flows/environments_flows.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev7/launchflow/flows/project_flows.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)    18602 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev7/launchflow/flows/resource_flows.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.481048 launchflow-0.3.9.dev7/launchflow/gcp/
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      219 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/gcp/__init__.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     7762 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/gcp/cloudsql.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2978 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/gcp/compute_engine.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     3523 2024-04-02 20:56:22.000000 launchflow-0.3.9.dev7/launchflow/gcp/gcs.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2755 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev7/launchflow/gcp/memorystore.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2578 2024-04-05 21:08:46.000000 launchflow-0.3.9.dev7/launchflow/gcp/utils.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2059 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev7/launchflow/operations.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     2288 2024-04-02 21:12:53.000000 launchflow-0.3.9.dev7/launchflow/resource.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       50 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev7/launchflow/service.py
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      789 2024-03-28 23:07:50.000000 launchflow-0.3.9.dev7/launchflow/utils.py
+drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:29:21.481048 launchflow-0.3.9.dev7/launchflow.egg-info/
+-rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-09 01:29:21.000000 launchflow-0.3.9.dev7/launchflow.egg-info/PKG-INFO
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     8331 2024-04-09 01:29:21.000000 launchflow-0.3.9.dev7/launchflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)        1 2024-04-09 01:29:21.000000 launchflow-0.3.9.dev7/launchflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       84 2024-04-09 01:29:21.000000 launchflow-0.3.9.dev7/launchflow.egg-info/entry_points.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)      309 2024-04-09 01:29:21.000000 launchflow-0.3.9.dev7/launchflow.egg-info/requires.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       11 2024-04-09 01:29:21.000000 launchflow-0.3.9.dev7/launchflow.egg-info/top_level.txt
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)     1421 2024-04-09 01:29:02.000000 launchflow-0.3.9.dev7/pyproject.toml
+-rw-rw-r--   0 tanke     (1000) tanke     (1000)       38 2024-04-09 01:29:21.481048 launchflow-0.3.9.dev7/setup.cfg
```

### Comparing `launchflow-0.3.9.dev6/PKG-INFO` & `launchflow-0.3.9.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchflow
-Version: 0.3.9.dev6
+Version: 0.3.9.dev7
 Summary: Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic.
 Author-email: CalebTVanDyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: beaupy
 Requires-Dist: rich
```

### Comparing `launchflow-0.3.9.dev6/README.md` & `launchflow-0.3.9.dev7/README.md`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/__init__.py` & `launchflow-0.3.9.dev7/launchflow/__init__.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/aws/rds.py` & `launchflow-0.3.9.dev7/launchflow/aws/rds.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/aws/s3.py` & `launchflow-0.3.9.dev7/launchflow/aws/s3.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cache/launchflow_tmp.py` & `launchflow-0.3.9.dev7/launchflow/cache/launchflow_tmp.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/accounts/account_commands.py` & `launchflow-0.3.9.dev7/launchflow/cli/accounts/account_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/config/config_commands.py` & `launchflow-0.3.9.dev7/launchflow/cli/config/config_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/constants.py` & `launchflow-0.3.9.dev7/launchflow/cli/constants.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/environments/environment_commands.py` & `launchflow-0.3.9.dev7/launchflow/cli/environments/environment_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/template.py` & `launchflow-0.3.9.dev7/launchflow/cli/gen/template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/django/django_template.py` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/django/django_template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/fastapi/fastapi_template.py` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/fastapi/fastapi_template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/gen/templates/flask/flask_template.py` & `launchflow-0.3.9.dev7/launchflow/cli/gen/templates/flask/flask_template.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/main.py` & `launchflow-0.3.9.dev7/launchflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/project/project_commands.py` & `launchflow-0.3.9.dev7/launchflow/cli/project/project_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/project_gen.py` & `launchflow-0.3.9.dev7/launchflow/cli/project_gen.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/resources/resource_commands.py` & `launchflow-0.3.9.dev7/launchflow/cli/resources/resource_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/resources_ast.py` & `launchflow-0.3.9.dev7/launchflow/cli/resources_ast.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/services/service_commands.py` & `launchflow-0.3.9.dev7/launchflow/cli/services/service_commands.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/cli/utils.py` & `launchflow-0.3.9.dev7/launchflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/accounts_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/accounts_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/client.py` & `launchflow-0.3.9.dev7/launchflow/clients/client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/connect_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/connect_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/environments_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/environments_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/operations_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/operations_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/projects_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/projects_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/resources_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/resources_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/response_schemas.py` & `launchflow-0.3.9.dev7/launchflow/clients/response_schemas.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/clients/services_client.py` & `launchflow-0.3.9.dev7/launchflow/clients/services_client.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/config/launchflow_config.py` & `launchflow-0.3.9.dev7/launchflow/config/launchflow_config.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/config/launchflow_env.py` & `launchflow-0.3.9.dev7/launchflow/config/launchflow_env.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/config/launchflow_yaml.py` & `launchflow-0.3.9.dev7/launchflow/config/launchflow_yaml.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/context/launchflow_ctx.py` & `launchflow-0.3.9.dev7/launchflow/context/launchflow_ctx.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/exceptions.py` & `launchflow-0.3.9.dev7/launchflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/fastapi.py` & `launchflow-0.3.9.dev7/launchflow/fastapi.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/flows/account_id.py` & `launchflow-0.3.9.dev7/launchflow/flows/account_id.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/flows/auth.py` & `launchflow-0.3.9.dev7/launchflow/flows/auth.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/flows/cloud_provider.py` & `launchflow-0.3.9.dev7/launchflow/flows/cloud_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,31 @@
 from launchflow.exceptions import LaunchFlowRequestFailure
 from launchflow.flows.account_id import get_account_id_from_config
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.prompt import Prompt
 
 from launchflow.clients import LaunchFlowAsyncClient
 
+XML_TEMPLATE = """
+<?xml version="1.0" encoding="UTF-8"?>
+<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
+<plist version="1.0">
+  <array>
+    <dict>
+      <key>choiceAttribute</key>
+      <string>customLocation</string>
+      <key>attributeSetting</key>
+      <string>{install_dir}</string>
+      <key>choiceIdentifier</key>
+      <string>default</string>
+    </dict>
+  </array>
+</plist>
+"""
+
 
 class CloudProvider(Enum):
     GCP = "gcp"
     AWS = "aws"
     AZURE = "azure"
 
 
@@ -145,32 +162,35 @@
                 initial_value="~/aws",
             )
             if install_dir == "~/aws":
                 install_dir = os.path.expanduser(install_dir)
             system = platform.system()
             download_url = ""
             proc_type = ""
+            is_mac = None
             if system == "Darwin":
+                is_mac = True
                 proc = subprocess.run("uname -m", shell=True, capture_output=True)
                 proc_type = proc.stdout.decode("utf-8").strip()
                 if proc.returncode != 0:
                     rich.print(
                         "[red]Error: failed to determine your processor type.[/red]."
                     )
                     return
                 if proc_type == "arm64":
                     download_url = "https://awscli.amazonaws.com/AWSCLIV2.pkg"
                 elif proc_type == "x86_64":
-                    download_url = "https://awscli.amazonaws.com/AWSCLIV2.zip"
+                    download_url = "https://awscli.amazonaws.com/AWSCLIV2.pkg"
                 else:
                     rich.print(
                         f"[red]Error: Processor not supported: {proc_type}.[/red] You can manually install aws following the instructions at: https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html, please reach out to us at founders@launchflow.com to have us add support for your machine type."
                     )
                     return
             elif system == "Linux":
+                is_mac = False
                 proc_type = platform.machine()
                 if proc_type == "x86_64":
                     download_url = (
                         "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip"
                     )
                 elif proc_type == "x86":
                     download_url = (
@@ -200,55 +220,105 @@
                 )
                 response = requests.get(download_url, stream=True)
                 if response.status_code != 200:
                     rich.print(
                         f"[red]Error: failed to download aws from: {download_url}.[/red]."
                     )
                     return
-                zip_file = os.path.join(install_dir, "aws.zip")
+
+                file_name = "aws.zip"
+                if is_mac:
+                    file_name = "AWSCLIV2.pkg"
+                file_path = os.path.join(install_dir, file_name)
                 os.makedirs(install_dir, exist_ok=True)
-                with open(zip_file, "wb") as f:
+                with open(file_path, "wb") as f:
                     f.write(response.raw.read())
                 progress.remove_task(download_task)
                 progress.console.print(
                     f"[green]✓[/green] Downloaded aws for {system} {proc_type}."
                 )
-            with zipfile.ZipFile(zip_file, "r") as zip_ref:
-                zip_ref.extractall(install_dir)
-            os.chmod(os.path.join(install_dir, "aws", "install"), 0o755)
-            os.chmod(os.path.join(install_dir, "aws", "dist", "aws"), 0o744)
-            bin_dir = os.path.join(install_dir, "bin")
-            install_sh = subprocess.run(
-                f"./aws/install --install-dir {install_dir} --bin-dir {bin_dir}",
-                shell=True,
-                cwd=install_dir,
-            )
+
+            if is_mac:
+                is_apple_silicon = proc_type == "arm64"
+                if is_apple_silicon:
+                    # Check if rosetta is installed
+                    rosetta_check = subprocess.run("pgrep oahd", shell=True)
+                    if rosetta_check.returncode != 0:
+                        rich.print(
+                            "[red]Error: Rosetta is not installed.[/red] This requires sudo permissions, so we cannot run it on your behalf.\n"
+                        )
+                        # Prompts the user to run the command and then continues on with the installation when they hit enter
+                        _ = Prompt.ask(
+                            "Please install Rosetta by running `sudo softwareupdate --install-rosetta` in another terminal window.\nHit enter once complete and we will continue with the aws cli installation."
+                        )
+                        # Continues to prompt the user until the rosetta installation is found
+                        while True:
+                            rosetta_check = subprocess.run("pgrep oahd", shell=True)
+                            if rosetta_check.returncode == 0:
+                                rich.print(
+                                    "[green]Rosetta has been installed successfully.[/green] Continuing with the aws cli installation."
+                                )
+                                break
+                            else:
+                                _ = Prompt.ask(
+                                    "[red]Error: Rosetta installation still not found.[/red] Please run `sudo softwareupdate --install-rosetta` in another terminal window.\nHit enter once complete and we will continue with the aws cli installation."
+                                )
+
+                choices_xml_path = os.path.join(install_dir, "choices.xml")
+                with open(choices_xml_path, "w") as f:
+                    f.write(XML_TEMPLATE.format(install_dir=install_dir))
+                install_sh = subprocess.run(
+                    f"installer -pkg {file_path} -target CurrentUserHomeDirectory -applyChoiceChangesXML {choices_xml_path}",
+                    shell=True,
+                )
+                if install_sh.returncode != 0:
+                    rich.print(
+                        f"[red]Error: failed to install aws, please run `installer -pkg {file_path} -target CurrentUserHomeDirectory -applyChoiceChangesXML choices.xml` in {install_dir}.[/red]."
+                    )
+                    return
+            else:
+                with zipfile.ZipFile(file_path, "r") as zip_ref:
+                    zip_ref.extractall(install_dir)
+                os.chmod(os.path.join(install_dir, "aws", "install"), 0o755)
+                os.chmod(os.path.join(install_dir, "aws", "dist", "aws"), 0o744)
+                bin_dir = os.path.join(install_dir, "bin")
+                install_sh = subprocess.run(
+                    f"./aws/install --install-dir {install_dir} --bin-dir {bin_dir}",
+                    shell=True,
+                    cwd=install_dir,
+                )
+                if install_sh.returncode != 0:
+                    rich.print(
+                        f"[red]Error: failed to install aws, please run `./aws/install --bin-dir {bin_dir}` in {install_dir}.[/red]."
+                    )
+                    return
+
             add_to_path = beaupy.confirm(
                 "Would you like to add the `aws` binary to your PATH?",
                 default_is_yes=True,
             )
             if add_to_path:
                 if os.path.exists(os.path.expanduser("~/.bashrc")):
                     with open(os.path.expanduser("~/.bashrc"), "a") as f:
                         f.write(f'export PATH="$PATH:{bin_dir}"\n')
+                if os.path.exists(os.path.expanduser("~/.bash_profile")):
+                    with open(os.path.expanduser("~/.bash_profile"), "a") as f:
+                        f.write(f'export PATH="$PATH:{bin_dir}"\n')
                 if os.path.exists(os.path.expanduser("~/.zshrc")):
                     with open(os.path.expanduser("~/.zshrc"), "a") as f:
                         f.write(f'export PATH="$PATH:{bin_dir}"\n')
-            if install_sh.returncode != 0:
-                rich.print(
-                    f"[red]Error: failed to install aws, please run `./aws/install --bin-dir {bin_dir}` in {install_dir}.[/red]."
-                )
-                return
             rich.print(
                 "[green]`aws` CLI successfully installed. You will need to reload your terminal to use it.[/green]"
             )
+            aws_bin = os.path.join(bin_dir, "aws")
         else:
             rich.print("[green]`aws` CLI is installed[/green]")
+            aws_bin = "aws"
         process = subprocess.run(
-            "aws sts get-caller-identity", shell=True, capture_output=True
+            f"{aws_bin} sts get-caller-identity", shell=True, capture_output=True
         )
         if process.returncode != 0:
             rich.print("[red]Error: No default `aws` credentials found.[/red]")
             set_up_auth = beaupy.confirm(
                 "Would you like us to authenticate for you?", default_is_yes=True
             )
             if set_up_auth:
@@ -261,33 +331,34 @@
                     default_is_yes=False,
                 )
                 if use_sso:
                     rich.print(
                         f"Running:\n\n\t$ aws configure sso --profile {profile_name}\n\nYou will need to have your AWS SSO URL ready. Visit https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sso.html for more information.\n"
                     )
                     process = subprocess.run(
-                        f"aws configure sso --profile {profile_name}", shell=True
+                        f"{aws_bin} configure sso --profile {profile_name}", shell=True
                     )
                 else:
                     rich.print(
                         f"Running:\n\n\t$ aws configure --profile {profile_name}\n\nYou will need to have your AWS access key ID and secret access key ready. Visit https://console.aws.amazon.com/iam/home#/security_credentials to create them.\nVisit https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html for more information.\n"
                     )
                     process = subprocess.run(
-                        f"aws configure --profile {profile_name}", shell=True
+                        f"{aws_bin} configure --profile {profile_name}", shell=True
                     )
                 set_default_profile = beaupy.confirm(
                     f"Would you like to set `{profile_name}` as your default AWS profile? (Recommended)",
                     default_is_yes=True,
                 )
                 if set_default_profile:
                     print(
                         f"Running:\n\n\t$ aws configure set default.profile {profile_name}\n"
                     )
                     process = subprocess.run(
-                        f"aws configure set default.profile {profile_name}", shell=True
+                        f"{aws_bin} configure set default.profile {profile_name}",
+                        shell=True,
                     )
                 # TODO: Make sure this doesnt run on cntl+c
                 rich.print(
                     f"[green]`aws` successfully authenticated with profile `{profile_name}`[/green]"
                 )
         else:
             rich.print("[green]`aws` is authenticated[/green]")
```

### Comparing `launchflow-0.3.9.dev6/launchflow/flows/environments_flows.py` & `launchflow-0.3.9.dev7/launchflow/flows/environments_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/flows/project_flows.py` & `launchflow-0.3.9.dev7/launchflow/flows/project_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/flows/resource_flows.py` & `launchflow-0.3.9.dev7/launchflow/flows/resource_flows.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/gcp/cloudsql.py` & `launchflow-0.3.9.dev7/launchflow/gcp/cloudsql.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/gcp/compute_engine.py` & `launchflow-0.3.9.dev7/launchflow/gcp/compute_engine.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/gcp/gcs.py` & `launchflow-0.3.9.dev7/launchflow/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/gcp/memorystore.py` & `launchflow-0.3.9.dev7/launchflow/gcp/memorystore.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/gcp/utils.py` & `launchflow-0.3.9.dev7/launchflow/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/operations.py` & `launchflow-0.3.9.dev7/launchflow/operations.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/resource.py` & `launchflow-0.3.9.dev7/launchflow/resource.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow/utils.py` & `launchflow-0.3.9.dev7/launchflow/utils.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/launchflow.egg-info/PKG-INFO` & `launchflow-0.3.9.dev7/launchflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchflow
-Version: 0.3.9.dev6
+Version: 0.3.9.dev7
 Summary: Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic.
 Author-email: CalebTVanDyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: beaupy
 Requires-Dist: rich
```

### Comparing `launchflow-0.3.9.dev6/launchflow.egg-info/SOURCES.txt` & `launchflow-0.3.9.dev7/launchflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev6/pyproject.toml` & `launchflow-0.3.9.dev7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launchflow"
-version = "0.3.9.dev6"
+version = "0.3.9.dev7"
 description = "Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic."
 authors = [
     { name = "CalebTVanDyke", email = "caleb@launchflow.com" },
     { name = "Josh Tanke", email = "josh@launchflow.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
```

