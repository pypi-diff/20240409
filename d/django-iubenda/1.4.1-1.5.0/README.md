# Comparing `tmp/django-iubenda-1.4.1.tar.gz` & `tmp/django-iubenda-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-iubenda-1.4.1.tar", last modified: Sat Mar 30 21:33:24 2024, max compression
+gzip compressed data, was "django-iubenda-1.5.0.tar", last modified: Tue Apr  9 20:17:10 2024, max compression
```

## Comparing `django-iubenda-1.4.1.tar` & `django-iubenda-1.5.0.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.423978 django-iubenda-1.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py310-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py311-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py38-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py39-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-30 21:33:24.431978 django-iubenda-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.415978 django-iubenda-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/src/django_iubenda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-30 21:33:24.000000 django-iubenda-1.4.1/src/django_iubenda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-30 21:33:24.000000 django-iubenda-1.4.1/src/django_iubenda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:33:24.000000 django-iubenda-1.4.1/src/django_iubenda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:33:24.000000 django-iubenda-1.4.1/src/django_iubenda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-30 21:33:24.000000 django-iubenda-1.4.1/src/django_iubenda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-30 21:33:24.000000 django-iubenda-1.4.1/src/django_iubenda.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.423978 django-iubenda-1.4.1/src/iubenda/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.423978 django-iubenda-1.4.1/src/iubenda/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/fixtures/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.415978 django-iubenda-1.4.1/src/iubenda/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.415978 django-iubenda-1.4.1/src/iubenda/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/src/iubenda/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/src/iubenda/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/sitemaps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.415978 django-iubenda-1.4.1/src/iubenda/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.415978 django-iubenda-1.4.1/src/iubenda/static/iubenda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/src/iubenda/static/iubenda/css/
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/static/iubenda/css/iubenda_badge.css
--rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/static/iubenda/css/iubenda_policy.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.415978 django-iubenda-1.4.1/src/iubenda/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/src/iubenda/templates/iubenda/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/templates/iubenda/cookie-compress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/templates/iubenda/cookie.html
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/templates/iubenda/include-content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/templates/iubenda/privacy-compress.html
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/templates/iubenda/privacy.html
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/src/iubenda/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/fixtures/data.json
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:33:24.427978 django-iubenda-1.4.1/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/test_iubenda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/test_iubenda_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/test_iubenda_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-30 21:33:14.000000 django-iubenda-1.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.265572 django-iubenda-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-09 20:17:10.265572 django-iubenda-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.257573 django-iubenda-1.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py310-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py311-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py38-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15799 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py39-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-09 20:17:10.265572 django-iubenda-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.249572 django-iubenda-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/django_iubenda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 20:17:10.000000 django-iubenda-1.5.0/src/django_iubenda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.257573 django-iubenda-1.5.0/src/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/fixtures/data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.249572 django-iubenda-1.5.0/src/iubenda/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/sitemaps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/static/iubenda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/static/iubenda/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_badge.css
+-rw-r--r--   0 runner    (1001) docker     (127)    42615 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_policy.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.253573 django-iubenda-1.5.0/src/iubenda/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/src/iubenda/templates/iubenda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie-compress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/include-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy-compress.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/src/iubenda/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/fixtures/data.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:17:10.261572 django-iubenda-1.5.0/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_custom_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_default_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/test_iubenda_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 20:16:56.000000 django-iubenda-1.5.0/tox.ini
```

### Comparing `django-iubenda-1.4.1/.pre-commit-config.yaml` & `django-iubenda-1.5.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: check-added-large-files
   - id: check-case-conflict
   - id: check-json
   - id: check-merge-conflict
   - id: check-symlinks
   - id: check-toml
```

### Comparing `django-iubenda-1.4.1/LICENSE` & `django-iubenda-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/PKG-INFO` & `django-iubenda-1.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,539 +1,467 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
-00000020: 676f 2d69 7562 656e 6461 0a56 6572 7369  go-iubenda.Versi
-00000030: 6f6e 3a20 312e 342e 310a 5375 6d6d 6172  on: 1.4.1.Summar
-00000040: 793a 2044 6a61 6e67 6f27 2773 2061 7070  y: Django''s app
-00000050: 6c69 6361 7469 6f6e 2066 6f72 2068 616e  lication for han
-00000060: 646c 696e 6720 7072 6976 6163 7920 616e  dling privacy an
-00000070: 6420 636f 6f6b 6965 2070 6f6c 6963 6965  d cookie policie
-00000080: 7320 636f 6e66 6967 7572 6564 2077 6974  s configured wit
-00000090: 6820 4975 6265 6e64 612e 0a48 6f6d 652d  h Iubenda..Home-
-000000a0: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
-000000b0: 7468 7562 2e63 6f6d 2f44 4c52 5350 2f64  thub.com/DLRSP/d
-000000c0: 6a61 6e67 6f2d 6975 6265 6e64 610a 4175  jango-iubenda.Au
-000000d0: 7468 6f72 3a20 444c 5253 500a 4175 7468  thor: DLRSP.Auth
-000000e0: 6f72 2d65 6d61 696c 3a20 646c 7273 702e  or-email: dlrsp.
-000000f0: 6465 7640 676d 6169 6c2e 636f 6d0a 4c69  dev@gmail.com.Li
-00000100: 6365 6e73 653a 204d 4954 204c 6963 656e  cense: MIT Licen
-00000110: 7365 0a4b 6579 776f 7264 733a 2064 6a61  se.Keywords: dja
-00000120: 6e67 6f2c 6975 6265 6e64 612c 7072 6976  ngo,iubenda,priv
-00000130: 6163 792c 636f 6f6b 6965 0a43 6c61 7373  acy,cookie.Class
-00000140: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
-00000150: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-00000160: 2042 6574 610a 436c 6173 7369 6669 6572   Beta.Classifier
-00000170: 3a20 456e 7669 726f 6e6d 656e 7420 3a3a  : Environment ::
-00000180: 2057 6562 2045 6e76 6972 6f6e 6d65 6e74   Web Environment
-00000190: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
-000001a0: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
-000001b0: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
-000001c0: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
-000001d0: 203a 3a20 332e 320a 436c 6173 7369 6669   :: 3.2.Classifi
-000001e0: 6572 3a20 4672 616d 6577 6f72 6b20 3a3a  er: Framework ::
-000001f0: 2044 6a61 6e67 6f20 3a3a 2034 2e30 0a43   Django :: 4.0.C
-00000200: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000210: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000220: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
-00000230: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000240: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000250: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
-00000260: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
-00000270: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
-00000280: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
-00000290: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000002b0: 2050 7974 686f 6e0a 436c 6173 7369 6669   Python.Classifi
-000002c0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002e0: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
-000002f0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
-00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000310: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790a  on :: 3 :: Only.
-00000320: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
-00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000340: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000350: 380a 436c 6173 7369 6669 6572 3a20 5072  8.Classifier: Pr
-00000360: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000370: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000380: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
-00000390: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000003a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000003b0: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
-000003c0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-000003d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003e0: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
-000003f0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000400: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000410: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
-00000420: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
-00000430: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
-00000440: 5450 0a43 6c61 7373 6966 6965 723a 2054  TP.Classifier: T
-00000450: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
-00000460: 203a 3a20 5757 572f 4854 5450 203a 3a20   :: WWW/HTTP :: 
-00000470: 4479 6e61 6d69 6320 436f 6e74 656e 740a  Dynamic Content.
-00000480: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
-00000490: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-000004a0: 2057 5757 2f48 5454 5020 3a3a 2057 5347   WWW/HTTP :: WSG
-000004b0: 4920 3a3a 2041 7070 6c69 6361 7469 6f6e  I :: Application
-000004c0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
-000004d0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-000004e0: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
-000004f0: 6272 6172 6965 7320 3a3a 2041 7070 6c69  braries :: Appli
-00000500: 6361 7469 6f6e 2046 7261 6d65 776f 726b  cation Framework
-00000510: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
-00000520: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
-00000530: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
-00000540: 6962 7261 7269 6573 0a52 6571 7569 7265  ibraries.Require
-00000550: 732d 5079 7468 6f6e 3a20 3e3d 332e 380a  s-Python: >=3.8.
-00000560: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
-00000570: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
-00000580: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
-00000590: 4669 6c65 3a20 4c49 4345 4e53 450a 5265  File: LICENSE.Re
-000005a0: 7175 6972 6573 2d44 6973 743a 2044 6a61  quires-Dist: Dja
-000005b0: 6e67 6f3e 3d33 2e32 0a50 726f 7669 6465  ngo>=3.2.Provide
-000005c0: 732d 4578 7472 613a 2074 6573 7469 6e67  s-Extra: testing
-000005d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000005e0: 636f 7665 7261 6765 3b20 6578 7472 6120  coverage; extra 
-000005f0: 3d3d 2022 7465 7374 696e 6722 0a52 6571  == "testing".Req
-00000600: 7569 7265 732d 4469 7374 3a20 636f 6465  uires-Dist: code
-00000610: 636f 763b 2065 7874 7261 203d 3d20 2274  cov; extra == "t
-00000620: 6573 7469 6e67 220a 5072 6f76 6964 6573  esting".Provides
-00000630: 2d45 7874 7261 3a20 6c69 6e74 696e 670a  -Extra: linting.
-00000640: 5265 7175 6972 6573 2d44 6973 743a 2066  Requires-Dist: f
-00000650: 6c61 6b65 383b 2065 7874 7261 203d 3d20  lake8; extra == 
-00000660: 226c 696e 7469 6e67 220a 5265 7175 6972  "linting".Requir
-00000670: 6573 2d44 6973 743a 2070 796c 696e 743b  es-Dist: pylint;
-00000680: 2065 7874 7261 203d 3d20 226c 696e 7469   extra == "linti
-00000690: 6e67 220a 0a23 2064 6a61 6e67 6f2d 6975  ng"..# django-iu
-000006a0: 6265 6e64 6120 5b21 5b50 7950 6920 6c69  benda [![PyPi li
-000006b0: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
-000006c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-000006d0: 7069 2f6c 2f64 6a61 6e67 6f2d 6975 6265  pi/l/django-iube
-000006e0: 6e64 612e 7376 6729 5d28 6874 7470 733a  nda.svg)](https:
-000006f0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000700: 672f 7079 7069 2f64 6a61 6e67 6f2d 6975  g/pypi/django-iu
-00000710: 6265 6e64 6129 0a0a 5b21 5b50 7950 6920  benda)..[![PyPi 
-00000720: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
-00000730: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
-00000740: 7970 692f 7374 6174 7573 2f64 6a61 6e67  ypi/status/djang
-00000750: 6f2d 6975 6265 6e64 612e 7376 6729 5d28  o-iubenda.svg)](
-00000760: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
-00000770: 686f 6e2e 6f72 672f 7079 7069 2f64 6a61  hon.org/pypi/dja
-00000780: 6e67 6f2d 6975 6265 6e64 6129 0a5b 215b  ngo-iubenda).[![
-00000790: 5079 5069 2076 6572 7369 6f6e 5d28 6874  PyPi version](ht
-000007a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000007b0: 732e 696f 2f70 7970 692f 762f 646a 616e  s.io/pypi/v/djan
-000007c0: 676f 2d69 7562 656e 6461 2e73 7667 295d  go-iubenda.svg)]
-000007d0: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
-000007e0: 7468 6f6e 2e6f 7267 2f70 7970 692f 646a  thon.org/pypi/dj
-000007f0: 616e 676f 2d69 7562 656e 6461 290a 5b21  ango-iubenda).[!
-00000800: 5b50 7950 6920 7079 7468 6f6e 2076 6572  [PyPi python ver
-00000810: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-00000820: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000830: 692f 7079 7665 7273 696f 6e73 2f64 6a61  i/pyversions/dja
-00000840: 6e67 6f2d 6975 6265 6e64 612e 7376 6729  ngo-iubenda.svg)
-00000850: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
-00000860: 7974 686f 6e2e 6f72 672f 7079 7069 2f64  ython.org/pypi/d
-00000870: 6a61 6e67 6f2d 6975 6265 6e64 6129 0a5b  jango-iubenda).[
-00000880: 215b 5079 5069 2064 6f77 6e6c 6f61 6473  ![PyPi downloads
-00000890: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000008a0: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
-000008b0: 2f64 6a61 6e67 6f2d 6975 6265 6e64 612e  /django-iubenda.
-000008c0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
-000008d0: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
-000008e0: 7069 2f64 6a61 6e67 6f2d 6975 6265 6e64  pi/django-iubend
-000008f0: 6129 0a5b 215b 5079 5069 2064 6f77 6e6c  a).[![PyPi downl
-00000900: 6f61 6473 5d28 6874 7470 733a 2f2f 696d  oads](https://im
-00000910: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000920: 692f 6477 2f64 6a61 6e67 6f2d 6975 6265  i/dw/django-iube
-00000930: 6e64 612e 7376 6729 5d28 6874 7470 733a  nda.svg)](https:
-00000940: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000950: 672f 7079 7069 2f64 6a61 6e67 6f2d 6975  g/pypi/django-iu
-00000960: 6265 6e64 6129 0a5b 215b 5079 5069 2064  benda).[![PyPi d
-00000970: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
-00000980: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000990: 2f70 7970 692f 6464 2f64 6a61 6e67 6f2d  /pypi/dd/django-
-000009a0: 6975 6265 6e64 612e 7376 6729 5d28 6874  iubenda.svg)](ht
-000009b0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
-000009c0: 6e2e 6f72 672f 7079 7069 2f64 6a61 6e67  n.org/pypi/djang
-000009d0: 6f2d 6975 6265 6e64 6129 0a0a 2323 2047  o-iubenda)..## G
-000009e0: 6974 4875 6220 215b 4769 7448 7562 2072  itHub ![GitHub r
-000009f0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
-00000a00: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-00000a10: 6974 6875 622f 7461 672f 444c 5253 502f  ithub/tag/DLRSP/
-00000a20: 646a 616e 676f 2d69 7562 656e 6461 2e73  django-iubenda.s
-00000a30: 7667 2920 215b 4769 7448 7562 2072 656c  vg) ![GitHub rel
-00000a40: 6561 7365 5d28 6874 7470 733a 2f2f 696d  ease](https://im
-00000a50: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000a60: 6875 622f 7265 6c65 6173 652f 444c 5253  hub/release/DLRS
-00000a70: 502f 646a 616e 676f 2d69 7562 656e 6461  P/django-iubenda
-00000a80: 2e73 7667 290a 0a23 2320 5465 7374 205b  .svg)..## Test [
-00000a90: 215b 636f 6465 636f 762e 696f 5d28 6874  ![codecov.io](ht
-00000aa0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
-00000ab0: 2f67 6974 6875 622f 444c 5253 502f 646a  /github/DLRSP/dj
-00000ac0: 616e 676f 2d69 7562 656e 6461 2f63 6f76  ango-iubenda/cov
-00000ad0: 6572 6167 652e 7376 673f 6272 616e 6368  erage.svg?branch
-00000ae0: 3d6d 6169 6e29 5d28 6874 7470 733a 2f2f  =main)](https://
-00000af0: 636f 6465 636f 762e 696f 2f67 6974 6875  codecov.io/githu
-00000b00: 622f 444c 5253 502f 646a 616e 676f 2d69  b/DLRSP/django-i
-00000b10: 7562 656e 6461 3f62 7261 6e63 683d 6d61  ubenda?branch=ma
-00000b20: 696e 2920 5b21 5b70 7265 2d63 6f6d 6d69  in) [![pre-commi
-00000b30: 742e 6369 2073 7461 7475 735d 2868 7474  t.ci status](htt
-00000b40: 7073 3a2f 2f72 6573 756c 7473 2e70 7265  ps://results.pre
-00000b50: 2d63 6f6d 6d69 742e 6369 2f62 6164 6765  -commit.ci/badge
-00000b60: 2f67 6974 6875 622f 444c 5253 502f 646a  /github/DLRSP/dj
-00000b70: 616e 676f 2d69 7562 656e 6461 2f6d 6169  ango-iubenda/mai
-00000b80: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
-00000b90: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
-00000ba0: 6974 2e63 692f 6c61 7465 7374 2f67 6974  it.ci/latest/git
-00000bb0: 6875 622f 444c 5253 502f 646a 616e 676f  hub/DLRSP/django
-00000bc0: 2d69 7562 656e 6461 2f6d 6169 6e29 205b  -iubenda/main) [
-00000bd0: 215b 6769 7474 6875 622e 636f 6d5d 2868  ![gitthub.com](h
-00000be0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000bf0: 6d2f 444c 5253 502f 646a 616e 676f 2d69  m/DLRSP/django-i
-00000c00: 7562 656e 6461 2f61 6374 696f 6e73 2f77  ubenda/actions/w
-00000c10: 6f72 6b66 6c6f 7773 2f63 692e 7961 6d6c  orkflows/ci.yaml
-00000c20: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
-00000c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000c40: 444c 5253 502f 646a 616e 676f 2d69 7562  DLRSP/django-iub
-00000c50: 656e 6461 2f61 6374 696f 6e73 2f77 6f72  enda/actions/wor
-00000c60: 6b66 6c6f 7773 2f63 692e 7961 6d6c 290a  kflows/ci.yaml).
-00000c70: 0a23 2320 436f 6d70 6c69 616e 6365 2066  .## Compliance f
-00000c80: 6f72 2077 6562 7369 7465 7320 616e 6420  or websites and 
-00000c90: 6170 7073 0a43 6c69 636b 205b 6865 7265  apps.Click [here
-00000ca0: 5d28 6874 7470 3a2f 2f69 7562 656e 6461  ](http://iubenda
-00000cb0: 2e72 6566 722e 6363 2f64 6c72 7370 6170  .refr.cc/dlrspap
-00000cc0: 6929 2061 6e64 2067 6574 2031 3025 2064  i) and get 10% d
-00000cd0: 6973 636f 756e 7420 6f6e 2066 6972 7374  iscount on first
-00000ce0: 2079 6561 7220 6174 2049 7562 656e 6461   year at Iubenda
-00000cf0: 0a5b 215b 4975 6265 6e64 615d 2868 7474  .[![Iubenda](htt
-00000d00: 7073 3a2f 2f63 6c69 656e 742d 6173 7365  ps://client-asse
-00000d10: 7473 2e72 6566 6572 7261 6c63 616e 6479  ts.referralcandy
-00000d20: 2e63 6f6d 2f6d 6436 5934 366a 4254 3575  .com/md6Y46jBT5u
-00000d30: 6654 434f 327a 7a47 745f 3136 3638 3539  fTCO2zzGt_166859
-00000d40: 3831 3836 2e70 6e67 295d 2868 7474 703a  8186.png)](http:
-00000d50: 2f2f 6975 6265 6e64 612e 7265 6672 2e63  //iubenda.refr.c
-00000d60: 632f 646c 7273 7061 7069 290a 0a0a 2323  c/dlrspapi)...##
-00000d70: 2043 6865 636b 2044 656d 6f20 5072 6f6a   Check Demo Proj
-00000d80: 6563 740a 2a20 4368 6563 6b20 7468 6520  ect.* Check the 
-00000d90: 6465 6d6f 2072 6570 6f20 6f6e 205b 4769  demo repo on [Gi
-00000da0: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
-00000db0: 7468 7562 2e63 6f6d 2f44 4c52 5350 2f65  thub.com/DLRSP/e
-00000dc0: 7861 6d70 6c65 2f74 7265 652f 646a 616e  xample/tree/djan
-00000dd0: 676f 2d69 7562 656e 6461 290a 0a23 2320  go-iubenda)..## 
-00000de0: 5265 7175 6972 656d 656e 7473 0a2d 2020  Requirements.-  
-00000df0: 2050 7974 686f 6e20 2b33 2e38 2073 7570   Python +3.8 sup
-00000e00: 706f 7274 6564 2e0a 2d20 2020 446a 616e  ported..-   Djan
-00000e10: 676f 202b 332e 3220 7375 7070 6f72 7465  go +3.2 supporte
-00000e20: 642e 0a0a 2323 2053 6574 7570 0a31 2e20  d...## Setup.1. 
-00000e30: 496e 7374 616c 6c20 6672 6f6d 202a 2a70  Install from **p
-00000e40: 6970 2a2a 3a0a 2020 2060 6060 7368 656c  ip**:.   ```shel
-00000e50: 6c0a 2020 2070 6970 2069 6e73 7461 6c6c  l.   pip install
-00000e60: 2064 6a61 6e67 6f2d 6975 6265 6e64 610a   django-iubenda.
-00000e70: 2020 2060 6060 0a32 2e20 4d6f 6469 6679     ```.2. Modify
-00000e80: 2060 7365 7474 696e 6773 2e70 7960 2062   `settings.py` b
-00000e90: 7920 6164 6469 6e67 2074 6865 2061 7070  y adding the app
-00000ea0: 2074 6f20 6049 4e53 5441 4c4c 4544 5f41   to `INSTALLED_A
-00000eb0: 5050 5360 3a0a 2020 2060 6060 7079 7468  PPS`:.   ```pyth
-00000ec0: 6f6e 0a20 2020 494e 5354 414c 4c45 445f  on.   INSTALLED_
-00000ed0: 4150 5053 203d 2028 0a20 2020 2020 2020  APPS = (.       
-00000ee0: 226d 6f64 656c 7472 616e 736c 6174 696f  "modeltranslatio
-00000ef0: 6e22 2c0a 2020 2020 2020 2023 202e 2e2e  n",.       # ...
-00000f00: 0a20 2020 2020 2020 2269 7562 656e 6461  .       "iubenda
-00000f10: 222c 0a20 2020 2020 2020 2320 2e2e 2e0a  ",.       # ....
-00000f20: 2020 2029 0a20 2020 6060 600a 332e 204d     ).   ```.3. M
-00000f30: 6f64 6966 7920 6073 6574 7469 6e67 732e  odify `settings.
-00000f40: 7079 6020 6279 2061 6464 696e 6720 7468  py` by adding th
-00000f50: 6520 6170 7027 7320 636f 6e74 6578 7420  e app's context 
-00000f60: 7072 6f63 6573 736f 7220 746f 2060 5445  processor to `TE
-00000f70: 4d50 4c41 5445 5360 3a0a 2020 2060 6060  MPLATES`:.   ```
-00000f80: 7079 7468 6f6e 0a20 2020 5445 4d50 4c41  python.   TEMPLA
-00000f90: 5445 5320 3d20 5b0a 2020 2020 2020 207b  TES = [.       {
-00000fa0: 0a20 2020 2020 2020 2020 2020 2320 2e2e  .           # ..
-00000fb0: 2e0a 2020 2020 2020 2020 2020 2022 4f50  ..           "OP
-00000fc0: 5449 4f4e 5322 3a20 7b0a 2020 2020 2020  TIONS": {.      
-00000fd0: 2020 2020 2020 2020 2022 636f 6e74 6578           "contex
-00000fe0: 745f 7072 6f63 6573 736f 7273 223a 205b  t_processors": [
-00000ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001000: 2020 2020 2320 2e2e 2e0a 2020 2020 2020      # ....      
-00001010: 2020 2020 2020 2020 2020 2020 2022 6975               "iu
-00001020: 6265 6e64 612e 636f 6e74 6578 745f 7072  benda.context_pr
-00001030: 6f63 6573 736f 7273 2e69 7562 656e 6461  ocessors.iubenda
-00001040: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001050: 2020 2020 2020 2320 2e2e 2e0a 2020 2020        # ....    
-00001060: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-00001070: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001080: 2020 207d 2c0a 2020 205d 0a20 2020 6060     },.   ].   ``
-00001090: 600a 342e 2042 6520 7375 7265 2074 6865  `.4. Be sure the
-000010a0: 2044 6a61 6e67 6f27 7320 4c6f 6361 6c65   Django's Locale
-000010b0: 206d 6964 646c 6577 6172 6520 6973 2065   middleware is e
-000010c0: 6e61 626c 6564 2069 6e73 6964 6520 6073  nabled inside `s
-000010d0: 6574 7469 6e67 732e 7079 603a 0a20 2020  ettings.py`:.   
-000010e0: 6060 6070 7974 686f 6e0a 2020 204d 4944  ```python.   MID
-000010f0: 444c 4557 4152 4520 3d20 280a 2020 2020  DLEWARE = (.    
-00001100: 2020 2023 202e 2e2e 0a20 2020 2020 2020     # ....       
-00001110: 2264 6a61 6e67 6f2e 6d69 6464 6c65 7761  "django.middlewa
-00001120: 7265 2e6c 6f63 616c 652e 4c6f 6361 6c65  re.locale.Locale
-00001130: 4d69 6464 6c65 7761 7265 222c 0a20 2020  Middleware",.   
-00001140: 2020 2020 2320 2e2e 2e0a 2020 2029 0a20      # ....   ). 
-00001150: 2020 6060 600a 352e 204f 7074 696f 6e61    ```.5. Optiona
-00001160: 6c6c 792c 2062 7574 2073 7567 6775 6573  lly, but suggues
-00001170: 7465 642c 2074 6865 2044 6a61 6e67 6f27  ted, the Django'
-00001180: 7320 4375 7272 656e 7420 5369 7465 206d  s Current Site m
-00001190: 6964 646c 6577 6172 6520 6973 2065 6e61  iddleware is ena
-000011a0: 626c 6564 2069 6e73 6964 6520 6073 6574  bled inside `set
-000011b0: 7469 6e67 732e 7079 603a 0a20 2020 6060  tings.py`:.   ``
-000011c0: 6070 7974 686f 6e0a 2020 204d 4944 444c  `python.   MIDDL
-000011d0: 4557 4152 4520 3d20 280a 2020 2020 2020  EWARE = (.      
-000011e0: 2023 202e 2e2e 0a20 2020 2020 2020 2264   # ....       "d
-000011f0: 6a61 6e67 6f2e 636f 6e74 7269 622e 7369  jango.contrib.si
-00001200: 7465 732e 6d69 6464 6c65 7761 7265 2e43  tes.middleware.C
-00001210: 7572 7265 6e74 5369 7465 4d69 6464 6c65  urrentSiteMiddle
-00001220: 7761 7265 222c 0a20 2020 2020 2020 2320  ware",.       # 
-00001230: 2e2e 2e0a 2020 2029 0a20 2020 6060 600a  ....   ).   ```.
-00001240: 362e 204d 6f64 6966 7920 6075 726c 2e70  6. Modify `url.p
-00001250: 7960 2062 7920 6164 6469 6e67 2074 6865  y` by adding the
-00001260: 2061 7070 2773 2075 726c 7320 746f 2060   app's urls to `
-00001270: 7572 6c70 6174 7465 726e 7360 3a0a 2020  urlpatterns`:.  
-00001280: 2060 6060 7079 7468 6f6e 0a20 2020 7572   ```python.   ur
-00001290: 6c70 6174 7465 726e 7320 2b3d 205b 0a20  lpatterns += [. 
-000012a0: 2020 2020 2020 7061 7468 2822 222c 2069        path("", i
-000012b0: 6e63 6c75 6465 2822 6975 6265 6e64 612e  nclude("iubenda.
-000012c0: 7572 6c73 2229 292c 0a20 2020 5d0a 2020  urls")),.   ].  
-000012d0: 2060 6060 0a37 2e20 4d6f 6469 6679 2060   ```.7. Modify `
-000012e0: 7572 6c2e 7079 6020 6279 2061 6464 696e  url.py` by addin
-000012f0: 6720 7468 6520 6170 7027 7320 7369 7465  g the app's site
-00001300: 6d61 7073 2074 6f20 6073 6974 656d 6170  maps to `sitemap
-00001310: 7360 3a0a 2020 2060 6060 7079 7468 6f6e  s`:.   ```python
-00001320: 0a20 2020 6672 6f6d 2069 7562 656e 6461  .   from iubenda
-00001330: 2e73 6974 656d 6170 7320 696d 706f 7274  .sitemaps import
-00001340: 2050 7269 7661 6379 5369 7465 6d61 702c   PrivacySitemap,
-00001350: 2043 6f6f 6b69 6553 6974 656d 6170 0a20   CookieSitemap. 
-00001360: 2020 0a20 2020 7369 7465 6d61 7073 203d    .   sitemaps =
-00001370: 207b 0a20 2020 2020 2020 2320 2e2e 2e0a   {.       # ....
-00001380: 2020 2020 2020 2022 7072 6976 6163 7922         "privacy"
-00001390: 3a20 5072 6976 6163 7953 6974 656d 6170  : PrivacySitemap
-000013a0: 2c0a 2020 2020 2020 2022 636f 6f6b 6965  ,.       "cookie
-000013b0: 223a 2043 6f6f 6b69 6553 6974 656d 6170  ": CookieSitemap
-000013c0: 2c0a 2020 2020 2020 2023 202e 2e2e 0a20  ,.       # .... 
-000013d0: 2020 7d0a 2020 2060 6060 0a38 2e20 4265    }.   ```.8. Be
-000013e0: 2073 7572 6520 7468 6520 7661 7269 6162   sure the variab
-000013f0: 6c65 2060 4c41 4e47 5541 4745 5f43 4f44  le `LANGUAGE_COD
-00001400: 4560 2069 7320 6176 6169 6c61 626c 6520  E` is available 
-00001410: 666f 7220 4854 4d4c 2074 656d 706c 6174  for HTML templat
-00001420: 6573 3a0a 2020 2060 6060 6874 6d6c 0a20  es:.   ```html. 
-00001430: 2020 7b25 206c 6f61 6420 6931 386e 2025    {% load i18n %
-00001440: 7d0a 2020 207b 2520 6765 745f 6375 7272  }.   {% get_curr
-00001450: 656e 745f 6c61 6e67 7561 6765 2061 7320  ent_language as 
-00001460: 4c41 4e47 5541 4745 5f43 4f44 4520 257d  LANGUAGE_CODE %}
-00001470: 0a20 2020 6060 600a 392e 204d 6f64 6966  .   ```.9. Modif
-00001480: 7920 796f 7572 2070 726f 6a65 6374 2773  y your project's
-00001490: 2074 656d 706c 6174 6520 746f 2061 6464   template to add
-000014a0: 2070 7269 7661 6379 2061 6e64 2063 6f6f   privacy and coo
-000014b0: 6b69 6520 706f 6c69 6369 6573 2e0a 2020  kie policies..  
-000014c0: 2046 6f72 2065 7861 6d70 6c65 2069 6e73   For example ins
-000014d0: 6964 6520 7468 6520 6066 6f6f 7465 722e  ide the `footer.
-000014e0: 6874 6d6c 6020 6164 6420 666f 6c6c 6f77  html` add follow
-000014f0: 696e 6720 636f 6465 3a0a 2020 2060 6060  ing code:.   ```
-00001500: 6874 6d6c 0a20 2020 7b25 2069 6620 6e6f  html.   {% if no
-00001510: 7420 6465 6275 6720 257d 0a20 2020 2020  t debug %}.     
-00001520: 2020 7b25 2062 6c6f 636b 2069 7562 656e    {% block iuben
-00001530: 6461 2025 7d7b 2520 696e 636c 7564 6520  da %}{% include 
-00001540: 2269 7562 656e 6461 2f69 6e63 6c75 6465  "iubenda/include
-00001550: 2d63 6f6e 7465 6e74 2e68 746d 6c22 2025  -content.html" %
-00001560: 7d7b 2520 656e 6462 6c6f 636b 2069 7562  }{% endblock iub
-00001570: 656e 6461 2025 7d0a 2020 207b 2520 656e  enda %}.   {% en
-00001580: 6469 6620 257d 0a20 2020 6060 600a 0a23  dif %}.   ```..#
-00001590: 2320 4f70 7469 6f6e 616c 0a0a 2323 2320  # Optional..### 
-000015a0: 436f 6e74 656e 7420 5365 6375 7269 7479  Content Security
-000015b0: 2050 6f6c 6963 790a 4966 2043 6f6e 7465   Policy.If Conte
-000015c0: 6e74 2053 6563 7572 6974 7920 506f 6c69  nt Security Poli
-000015d0: 6379 2061 7265 2069 6d70 6c65 6d65 6e74  cy are implement
-000015e0: 6564 2069 6e20 796f 7572 2073 6572 7665  ed in your serve
-000015f0: 7220 616e 6420 696e 6c69 6e65 2073 6372  r and inline scr
-00001600: 6970 7473 2061 7265 2064 6973 6162 6c65  ipts are disable
-00001610: 642c 0a74 6865 2076 6172 6961 626c 6520  d,.the variable 
-00001620: 6049 5542 454e 4441 5f43 5350 5f4e 4f4e  `IUBENDA_CSP_NON
-00001630: 4345 6020 6361 6e20 6265 2073 6574 2077  CE` can be set w
-00001640: 6974 6820 6e6f 6e63 6520 7461 6720 7769  ith nonce tag wi
-00001650: 6c6c 2062 6520 696e 7365 7274 6564 2073  ll be inserted s
-00001660: 6372 6970 7427 7320 6e6f 6e63 652e 0a60  cript's nonce..`
-00001670: 6060 6874 6d6c 0a3c 7363 7269 7074 2074  ``html.<script t
-00001680: 7970 653d 2274 6578 742f 6a61 7661 7363  ype="text/javasc
-00001690: 7269 7074 2220 7b25 2069 6620 6378 5f69  ript" {% if cx_i
-000016a0: 7562 656e 6461 5f6e 6f6e 6365 2025 7d6e  ubenda_nonce %}n
-000016b0: 6f6e 6365 3d22 7b7b 2063 785f 6975 6265  once="{{ cx_iube
-000016c0: 6e64 615f 6e6f 6e63 6520 7d7d 227b 2520  nda_nonce }}"{% 
-000016d0: 656e 6469 6620 257d 3e0a 6060 600a 496e  endif %}>.```.In
-000016e0: 7369 6465 2079 6f75 7220 7765 6273 6572  side your webser
-000016f0: 7665 7227 7320 636f 6e66 6967 7572 6174  ver's configurat
-00001700: 696f 6e73 2c20 6120 7275 6c65 2074 6f20  ions, a rule to 
-00001710: 6479 6e61 6d69 6361 6c6c 7920 7265 706c  dynamically repl
-00001720: 6163 6520 796f 7572 2043 4f4e 5354 414e  ace your CONSTAN
-00001730: 5420 6e6f 6e63 6520 696e 2061 2072 616e  T nonce in a ran
-00001740: 646f 6d20 7374 7269 6e67 2069 7320 6e65  dom string is ne
-00001750: 6564 6564 2e0a 0a54 6f20 616c 6c6f 7720  eded...To allow 
-00001760: 2065 7874 6572 6e61 6c20 736f 7572 6365   external source
-00001770: 2066 726f 6d20 4975 6265 6e64 6120 646f   from Iubenda do
-00001780: 6d61 696e 732c 2070 6c65 6173 6520 696d  mains, please im
-00001790: 706c 656d 656e 7420 7468 6573 6520 7275  plement these ru
-000017a0: 6c65 733a 0a60 6060 6564 6974 6f72 636f  les:.```editorco
-000017b0: 6e66 6967 0a43 6f6e 7465 6e74 2d53 6563  nfig.Content-Sec
-000017c0: 7572 6974 792d 506f 6c69 6379 3a0a 2020  urity-Policy:.  
-000017d0: 2020 7363 7269 7074 2d73 7263 2d65 6c65    script-src-ele
-000017e0: 6d20 6874 7470 733a 2f2f 2a2e 6975 6265  m https://*.iube
-000017f0: 6e64 612e 636f 6d22 3b0a 2020 2020 696d  nda.com";.    im
-00001800: 672d 7372 6320 6874 7470 733a 2f2f 2a2e  g-src https://*.
-00001810: 6975 6265 6e64 612e 636f 6d20 6461 7461  iubenda.com data
-00001820: 3a22 3b0a 2020 2020 7374 796c 652d 7372  :";.    style-sr
-00001830: 6320 6874 7470 733a 2f2f 2a2e 6975 6265  c https://*.iube
-00001840: 6e64 612e 636f 6d22 3b0a 2020 2020 636f  nda.com";.    co
-00001850: 6e6e 6563 742d 7372 6320 6874 7470 733a  nnect-src https:
-00001860: 2f2f 2a2e 6975 6265 6e64 612e 636f 6d22  //*.iubenda.com"
-00001870: 3b0a 2020 2020 6672 616d 652d 7372 6320  ;.    frame-src 
-00001880: 6874 7470 733a 2f2f 2a2e 6975 6265 6e64  https://*.iubend
-00001890: 612e 636f 6d22 3b0a 6060 600a 0a49 6620  a.com";.```..If 
-000018a0: 796f 7520 7072 6566 6572 2074 6f20 6e6f  you prefer to no
-000018b0: 7420 616c 6c6f 7720 2a2a 2a75 6e73 6166  t allow ***unsaf
-000018c0: 652d 696e 6c69 6e65 2a2a 2a20 696e 7369  e-inline*** insi
-000018d0: 6465 2079 6f75 7220 4353 502c 2070 6c65  de your CSP, ple
-000018e0: 6173 6520 616c 736f 2061 6464 2074 6865  ase also add the
-000018f0: 2074 776f 2073 7065 6369 6669 6320 6861   two specific ha
-00001900: 7368 2066 6f72 2079 6f75 720a 7363 7269  sh for your.scri
-00001910: 7074 2070 726f 6d70 7465 6420 6173 2065  pt prompted as e
-00001920: 7272 6f72 2069 6e20 4a61 7661 7363 7269  rror in Javascri
-00001930: 7074 2043 6f6e 736f 6c65 2e0a 6060 6065  pt Console..```e
-00001940: 6469 746f 7263 6f6e 6669 670a 2320 4975  ditorconfig.# Iu
-00001950: 6265 6e64 6120 5072 6976 6163 7920 416e  benda Privacy An
-00001960: 6420 436f 6f6b 6965 2050 6f6c 6963 7920  d Cookie Policy 
-00001970: 2d20 4150 490a 436f 6e74 656e 742d 5365  - API.Content-Se
-00001980: 6375 7269 7479 2d50 6f6c 6963 793a 0a20  curity-Policy:. 
-00001990: 2020 202e 2e2e 0a20 2020 2073 6372 6970     ....    scrip
-000019a0: 742d 7372 632d 656c 656d 2068 7474 7073  t-src-elem https
-000019b0: 3a2f 2f2a 2e69 7562 656e 6461 2e63 6f6d  ://*.iubenda.com
-000019c0: 2027 7368 6132 3536 2d59 4f55 522d 4649   'sha256-YOUR-FI
-000019d0: 5253 542d 4841 5348 2d50 524f 4d50 5445  RST-HASH-PROMPTE
-000019e0: 442d 494e 5349 4445 2d43 4f4e 534f 4c45  D-INSIDE-CONSOLE
-000019f0: 2720 2773 6861 3235 362d 594f 5552 2d53  ' 'sha256-YOUR-S
-00001a00: 4543 4f4e 442d 4841 5348 2d50 524f 4d50  ECOND-HASH-PROMP
-00001a10: 5445 442d 494e 5349 4445 2d43 4f4e 534f  TED-INSIDE-CONSO
-00001a20: 4c45 273b 0a20 2020 202e 2e2e 0a60 6060  LE';.    ....```
-00001a30: 0a0a 4368 6563 6b20 7468 6973 2061 7274  ..Check this art
-00001a40: 6963 6c65 2066 726f 6d20 5b49 7562 656e  icle from [Iuben
-00001a50: 6461 2068 656c 705d 2868 7474 7073 3a2f  da help](https:/
-00001a60: 2f77 7777 2e69 7562 656e 6461 2e63 6f6d  /www.iubenda.com
-00001a70: 2f69 742f 6865 6c70 2f31 3233 3437 2d63  /it/help/12347-c
-00001a80: 6f6d 652d 636f 6e66 6967 7572 6172 652d  ome-configurare-
-00001a90: 696c 2d63 6f6e 7465 6e74 2d73 6563 7572  il-content-secur
-00001aa0: 6974 792d 706f 6c69 6379 2d70 6572 2d63  ity-policy-per-c
-00001ab0: 6f6e 7365 6e74 6972 652d 6c65 7365 6375  onsentire-lesecu
-00001ac0: 7a69 6f6e 652d 6465 676c 692d 7363 7269  zione-degli-scri
-00001ad0: 7074 2d64 692d 6975 6265 6e64 6129 0a0a  pt-di-iubenda)..
-00001ae0: 2323 2320 4975 6265 6e64 6127 7320 4f70  ### Iubenda's Op
-00001af0: 7469 6f6e 730a 0a54 6f20 7065 7273 6f6e  tions..To person
-00001b00: 616c 697a 6520 7468 6520 4975 6265 6e64  alize the Iubend
-00001b10: 6120 7363 7269 7074 2773 2062 6568 6176  a script's behav
-00001b20: 696f 7572 2c20 7468 6520 6469 6374 2060  iour, the dict `
-00001b30: 4955 4245 4e44 415f 4f50 5449 4f4e 5360  IUBENDA_OPTIONS`
-00001b40: 2063 616e 2062 6520 636f 6e66 6967 7572   can be configur
-00001b50: 6564 2069 6e73 6964 6520 6073 6574 7469  ed inside `setti
-00001b60: 6e67 732e 7079 600a 6060 6070 7974 686f  ngs.py`.```pytho
-00001b70: 6e0a 4955 4245 4e44 415f 4f50 5449 4f4e  n.IUBENDA_OPTION
-00001b80: 5320 3d20 7b0a 2020 2020 2263 6370 6141  S = {.    "ccpaA
-00001b90: 636b 6e6f 776c 6564 6765 4f6e 4469 7370  cknowledgeOnDisp
-00001ba0: 6c61 7922 3a20 2274 7275 6522 2c0a 2020  lay": "true",.  
-00001bb0: 2020 2263 6370 6141 7070 6c69 6573 223a    "ccpaApplies":
-00001bc0: 2022 7472 7565 222c 0a20 2020 2022 636f   "true",.    "co
-00001bd0: 6e73 656e 744f 6e43 6f6e 7469 6e75 6564  nsentOnContinued
-00001be0: 4272 6f77 7369 6e67 223a 2022 6661 6c73  Browsing": "fals
-00001bf0: 6522 2c0a 2020 2020 2265 6e61 626c 6543  e",.    "enableC
-00001c00: 6370 6122 3a20 2274 7275 6522 2c0a 2020  cpa": "true",.  
-00001c10: 2020 2266 6c6f 6174 696e 6750 7265 6665    "floatingPrefe
-00001c20: 7265 6e63 6573 4275 7474 6f6e 4469 7370  rencesButtonDisp
-00001c30: 6c61 7922 3a20 2262 6f74 746f 6d2d 6c65  lay": "bottom-le
-00001c40: 6674 222c 0a20 2020 2022 696e 7661 6c69  ft",.    "invali
-00001c50: 6461 7465 436f 6e73 656e 7457 6974 686f  dateConsentWitho
-00001c60: 7574 4c6f 6722 3a20 2274 7275 6522 2c0a  utLog": "true",.
-00001c70: 2020 2020 2270 6572 5075 7270 6f73 6543      "perPurposeC
-00001c80: 6f6e 7365 6e74 223a 2022 7472 7565 222c  onsent": "true",
-00001c90: 0a20 2020 2022 7768 6974 656c 6162 656c  .    "whitelabel
-00001ca0: 223a 2022 6661 6c73 6522 2c0a 2020 2020  ": "false",.    
-00001cb0: 2262 616e 6e65 7222 3a20 7b0a 2020 2020  "banner": {.    
-00001cc0: 2020 2020 2261 6363 6570 7442 7574 746f      "acceptButto
-00001cd0: 6e44 6973 706c 6179 223a 2022 7472 7565  nDisplay": "true
-00001ce0: 222c 0a20 2020 2020 2020 2022 6261 636b  ",.        "back
-00001cf0: 6772 6f75 6e64 4f76 6572 6c61 7922 3a20  groundOverlay": 
-00001d00: 2274 7275 6522 2c0a 2020 2020 2020 2020  "true",.        
-00001d10: 2263 6c6f 7365 4275 7474 6f6e 5265 6a65  "closeButtonReje
-00001d20: 6374 7322 3a20 2274 7275 6522 2c0a 2020  cts": "true",.  
-00001d30: 2020 2020 2020 2263 7573 746f 6d69 7a65        "customize
-00001d40: 4275 7474 6f6e 4469 7370 6c61 7922 3a20  ButtonDisplay": 
-00001d50: 2274 7275 6522 2c0a 2020 2020 2020 2020  "true",.        
-00001d60: 2265 7870 6c69 6369 7457 6974 6864 7261  "explicitWithdra
-00001d70: 7761 6c22 3a20 2274 7275 6522 2c0a 2020  wal": "true",.  
-00001d80: 2020 2020 2020 2266 6f6e 7453 697a 6522        "fontSize"
-00001d90: 3a20 2231 3470 7822 2c0a 2020 2020 2020  : "14px",.      
-00001da0: 2020 226c 6973 7450 7572 706f 7365 7322    "listPurposes"
-00001db0: 3a20 2274 7275 6522 2c0a 2020 2020 2020  : "true",.      
-00001dc0: 2020 2270 6f73 6974 696f 6e22 3a20 2266    "position": "f
-00001dd0: 6c6f 6174 2d63 656e 7465 7222 2c0a 2020  loat-center",.  
-00001de0: 2020 2020 2020 2272 656a 6563 7442 7574        "rejectBut
-00001df0: 746f 6e44 6973 706c 6179 223a 2022 7472  tonDisplay": "tr
-00001e00: 7565 222c 0a20 2020 207d 2c0a 7d0a 6060  ue",.    },.}.``
-00001e10: 600a 0a23 2323 2049 6e74 6567 7261 7469  `..### Integrati
-00001e20: 6f6e 2077 6974 6820 476f 6f67 6c65 2054  on with Google T
-00001e30: 6167 204d 616e 6167 6572 0a49 6620 476f  ag Manager.If Go
-00001e40: 6f67 6c65 2054 6167 204d 616e 6167 6572  ogle Tag Manager
-00001e50: 2069 7320 696d 706c 656d 656e 7465 6420   is implemented 
-00001e60: 696e 2079 6f75 7220 6170 706c 6963 6174  in your applicat
-00001e70: 696f 6e20 616e 6420 616c 6c20 6e65 6564  ion and all need
-00001e80: 6564 2073 6574 7469 6e67 7320 7765 7265  ed settings were
-00001e90: 2063 6f6e 6669 6775 7265 6420 696e 7369   configured insi
-00001ea0: 6465 2074 6865 2063 6f6e 7461 696e 6572  de the container
-00001eb0: 2c0a 7468 6520 7661 7269 6162 6c65 2060  ,.the variable `
-00001ec0: 4955 4245 4e44 415f 4754 4d60 2063 616e  IUBENDA_GTM` can
-00001ed0: 2062 6520 7365 7420 7769 7468 2074 6865   be set with the
-00001ee0: 2076 616c 7565 2060 5472 7565 6020 616e   value `True` an
-00001ef0: 6420 7468 6520 4975 6265 6e64 6127 7320  d the Iubenda's 
-00001f00: 6361 6c6c 6261 636b 2077 696c 6c20 6265  callback will be
-00001f10: 2069 6e73 6572 7465 6420 696e 7369 6465   inserted inside
-00001f20: 2074 6865 2073 6372 6970 742e 0a0a 466f   the script...Fo
-00001f30: 7220 6e65 6564 6564 2063 6f6e 6669 6775  r needed configu
-00001f40: 7261 7469 6f6e 2069 6e73 6964 6520 476f  ration inside Go
-00001f50: 6f67 6c65 2054 6167 204d 616e 6167 6572  ogle Tag Manager
-00001f60: 2063 6f6e 7461 696e 6572 2c20 706c 6561   container, plea
-00001f70: 7365 2072 6566 6572 2074 6f20 7468 6573  se refer to thes
-00001f80: 6520 6e6f 7465 733a 0a2d 205b 476f 6f67  e notes:.- [Goog
-00001f90: 6c65 2043 6f6e 7365 6e74 204d 6f64 655d  le Consent Mode]
-00001fa0: 2868 7474 7073 3a2f 2f77 7777 2e69 7562  (https://www.iub
-00001fb0: 656e 6461 2e63 6f6d 2f65 6e2f 6865 6c70  enda.com/en/help
-00001fc0: 2f32 3731 3337 2d67 6f6f 676c 652d 636f  /27137-google-co
-00001fd0: 6e73 656e 742d 6d6f 6465 290a 2d20 5b47  nsent-mode).- [G
-00001fe0: 6f6f 676c 6520 436f 6e73 656e 7420 4d6f  oogle Consent Mo
-00001ff0: 6465 2073 6574 7570 2047 544d 2077 6974  de setup GTM wit
-00002000: 6820 4975 6265 6e64 615d 2868 7474 7073  h Iubenda](https
-00002010: 3a2f 2f77 7777 2e69 7562 656e 6461 2e63  ://www.iubenda.c
-00002020: 6f6d 2f65 6e2f 6865 6c70 2f37 3431 3938  om/en/help/74198
-00002030: 2d67 6f6f 676c 652d 636f 6e73 656e 742d  -google-consent-
-00002040: 6d6f 6465 2d73 6574 2d75 702d 676f 6f67  mode-set-up-goog
-00002050: 6c65 2d74 6167 2d6d 616e 6167 6572 2d77  le-tag-manager-w
-00002060: 6974 682d 6975 6265 6e64 6129 0a2d 205b  ith-iubenda).- [
-00002070: 4754 4d20 426c 6f63 6b69 6e67 2043 6f6f  GTM Blocking Coo
-00002080: 6b69 6573 5d28 6874 7470 733a 2f2f 7777  kies](https://ww
-00002090: 772e 6975 6265 6e64 612e 636f 6d2f 656e  w.iubenda.com/en
-000020a0: 2f68 656c 702f 3132 3335 2d67 6f6f 676c  /help/1235-googl
-000020b0: 652d 7461 672d 6d61 6e61 6765 722d 626c  e-tag-manager-bl
-000020c0: 6f63 6b69 6e67 2d63 6f6f 6b69 6573 290a  ocking-cookies).
-000020d0: 0a23 2320 5275 6e20 4578 616d 706c 6520  .## Run Example 
-000020e0: 5072 6f6a 6563 740a 0a60 6060 7368 656c  Project..```shel
-000020f0: 6c0a 6769 7420 636c 6f6e 6520 2d2d 6465  l.git clone --de
-00002100: 7074 683d 3530 202d 2d62 7261 6e63 683d  pth=50 --branch=
-00002110: 646a 616e 676f 2d69 7562 656e 6461 2068  django-iubenda h
-00002120: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002130: 6d2f 444c 5253 502f 6578 616d 706c 652e  m/DLRSP/example.
-00002140: 6769 7420 444c 5253 502f 6578 616d 706c  git DLRSP/exampl
-00002150: 650a 6364 2044 4c52 5350 2f65 7861 6d70  e.cd DLRSP/examp
-00002160: 6c65 0a70 7974 686f 6e20 6d61 6e61 6765  le.python manage
-00002170: 2e70 7920 7275 6e73 6572 7665 720a 6060  .py runserver.``
-00002180: 600a 0a4e 6f77 2062 726f 7773 6572 2074  `..Now browser t
-00002190: 6865 2061 7070 2040 2068 7474 703a 2f2f  he app @ http://
-000021a0: 3132 372e 302e 302e 313a 3830 3030 0a    127.0.0.1:8000.
+00000000: 2320 646a 616e 676f 2d69 7562 656e 6461  # django-iubenda
+00000010: 205b 215b 5079 5069 206c 6963 656e 7365   [![PyPi license
+00000020: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000030: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
+00000040: 646a 616e 676f 2d69 7562 656e 6461 2e73  django-iubenda.s
+00000050: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
+00000060: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+00000070: 692f 646a 616e 676f 2d69 7562 656e 6461  i/django-iubenda
+00000080: 290a 0a5b 215b 5079 5069 2073 7461 7475  )..[![PyPi statu
+00000090: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
+000000a0: 6869 656c 6473 2e69 6f2f 7079 7069 2f73  hields.io/pypi/s
+000000b0: 7461 7475 732f 646a 616e 676f 2d69 7562  tatus/django-iub
+000000c0: 656e 6461 2e73 7667 295d 2868 7474 7073  enda.svg)](https
+000000d0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+000000e0: 7267 2f70 7970 692f 646a 616e 676f 2d69  rg/pypi/django-i
+000000f0: 7562 656e 6461 290a 5b21 5b50 7950 6920  ubenda).[![PyPi 
+00000100: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
+00000110: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000120: 7079 7069 2f76 2f64 6a61 6e67 6f2d 6975  pypi/v/django-iu
+00000130: 6265 6e64 612e 7376 6729 5d28 6874 7470  benda.svg)](http
+00000140: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000150: 6f72 672f 7079 7069 2f64 6a61 6e67 6f2d  org/pypi/django-
+00000160: 6975 6265 6e64 6129 0a5b 215b 5079 5069  iubenda).[![PyPi
+00000170: 2070 7974 686f 6e20 7665 7273 696f 6e5d   python version]
+00000180: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000190: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
+000001a0: 6572 7369 6f6e 732f 646a 616e 676f 2d69  ersions/django-i
+000001b0: 7562 656e 6461 2e73 7667 295d 2868 7474  ubenda.svg)](htt
+000001c0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
+000001d0: 2e6f 7267 2f70 7970 692f 646a 616e 676f  .org/pypi/django
+000001e0: 2d69 7562 656e 6461 290a 5b21 5b50 7950  -iubenda).[![PyP
+000001f0: 6920 646f 776e 6c6f 6164 735d 2868 7474  i downloads](htt
+00000200: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000210: 2e69 6f2f 7079 7069 2f64 6d2f 646a 616e  .io/pypi/dm/djan
+00000220: 676f 2d69 7562 656e 6461 2e73 7667 295d  go-iubenda.svg)]
+00000230: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
+00000240: 7468 6f6e 2e6f 7267 2f70 7970 692f 646a  thon.org/pypi/dj
+00000250: 616e 676f 2d69 7562 656e 6461 290a 5b21  ango-iubenda).[!
+00000260: 5b50 7950 6920 646f 776e 6c6f 6164 735d  [PyPi downloads]
+00000270: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000280: 656c 6473 2e69 6f2f 7079 7069 2f64 772f  elds.io/pypi/dw/
+00000290: 646a 616e 676f 2d69 7562 656e 6461 2e73  django-iubenda.s
+000002a0: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
+000002b0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+000002c0: 692f 646a 616e 676f 2d69 7562 656e 6461  i/django-iubenda
+000002d0: 290a 5b21 5b50 7950 6920 646f 776e 6c6f  ).[![PyPi downlo
+000002e0: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
+000002f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000300: 2f64 642f 646a 616e 676f 2d69 7562 656e  /dd/django-iuben
+00000310: 6461 2e73 7667 295d 2868 7474 7073 3a2f  da.svg)](https:/
+00000320: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
+00000330: 2f70 7970 692f 646a 616e 676f 2d69 7562  /pypi/django-iub
+00000340: 656e 6461 290a 0a23 2320 4769 7448 7562  enda)..## GitHub
+00000350: 2021 5b47 6974 4875 6220 7265 6c65 6173   ![GitHub releas
+00000360: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000370: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000380: 2f74 6167 2f44 4c52 5350 2f64 6a61 6e67  /tag/DLRSP/djang
+00000390: 6f2d 6975 6265 6e64 612e 7376 6729 2021  o-iubenda.svg) !
+000003a0: 5b47 6974 4875 6220 7265 6c65 6173 655d  [GitHub release]
+000003b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000003c0: 656c 6473 2e69 6f2f 6769 7468 7562 2f72  elds.io/github/r
+000003d0: 656c 6561 7365 2f44 4c52 5350 2f64 6a61  elease/DLRSP/dja
+000003e0: 6e67 6f2d 6975 6265 6e64 612e 7376 6729  ngo-iubenda.svg)
+000003f0: 0a0a 2323 2054 6573 7420 5b21 5b63 6f64  ..## Test [![cod
+00000400: 6563 6f76 2e69 6f5d 2868 7474 7073 3a2f  ecov.io](https:/
+00000410: 2f63 6f64 6563 6f76 2e69 6f2f 6769 7468  /codecov.io/gith
+00000420: 7562 2f44 4c52 5350 2f64 6a61 6e67 6f2d  ub/DLRSP/django-
+00000430: 6975 6265 6e64 612f 636f 7665 7261 6765  iubenda/coverage
+00000440: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
+00000450: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
+00000460: 6f76 2e69 6f2f 6769 7468 7562 2f44 4c52  ov.io/github/DLR
+00000470: 5350 2f64 6a61 6e67 6f2d 6975 6265 6e64  SP/django-iubend
+00000480: 613f 6272 616e 6368 3d6d 6169 6e29 205b  a?branch=main) [
+00000490: 215b 7072 652d 636f 6d6d 6974 2e63 6920  ![pre-commit.ci 
+000004a0: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
+000004b0: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+000004c0: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
+000004d0: 7562 2f44 4c52 5350 2f64 6a61 6e67 6f2d  ub/DLRSP/django-
+000004e0: 6975 6265 6e64 612f 6d61 696e 2e73 7667  iubenda/main.svg
+000004f0: 295d 2868 7474 7073 3a2f 2f72 6573 756c  )](https://resul
+00000500: 7473 2e70 7265 2d63 6f6d 6d69 742e 6369  ts.pre-commit.ci
+00000510: 2f6c 6174 6573 742f 6769 7468 7562 2f44  /latest/github/D
+00000520: 4c52 5350 2f64 6a61 6e67 6f2d 6975 6265  LRSP/django-iube
+00000530: 6e64 612f 6d61 696e 2920 5b21 5b67 6974  nda/main) [![git
+00000540: 7468 7562 2e63 6f6d 5d28 6874 7470 733a  thub.com](https:
+00000550: 2f2f 6769 7468 7562 2e63 6f6d 2f44 4c52  //github.com/DLR
+00000560: 5350 2f64 6a61 6e67 6f2d 6975 6265 6e64  SP/django-iubend
+00000570: 612f 6163 7469 6f6e 732f 776f 726b 666c  a/actions/workfl
+00000580: 6f77 732f 6369 2e79 616d 6c2f 6261 6467  ows/ci.yaml/badg
+00000590: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000005a0: 6769 7468 7562 2e63 6f6d 2f44 4c52 5350  github.com/DLRSP
+000005b0: 2f64 6a61 6e67 6f2d 6975 6265 6e64 612f  /django-iubenda/
+000005c0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000005d0: 732f 6369 2e79 616d 6c29 0a0a 2323 2043  s/ci.yaml)..## C
+000005e0: 6f6d 706c 6961 6e63 6520 666f 7220 7765  ompliance for we
+000005f0: 6273 6974 6573 2061 6e64 2061 7070 730a  bsites and apps.
+00000600: 436c 6963 6b20 5b68 6572 655d 2868 7474  Click [here](htt
+00000610: 703a 2f2f 6975 6265 6e64 612e 7265 6672  p://iubenda.refr
+00000620: 2e63 632f 646c 7273 7061 7069 2920 616e  .cc/dlrspapi) an
+00000630: 6420 6765 7420 3130 2520 6469 7363 6f75  d get 10% discou
+00000640: 6e74 206f 6e20 6669 7273 7420 7965 6172  nt on first year
+00000650: 2061 7420 4975 6265 6e64 610a 5b21 5b49   at Iubenda.[![I
+00000660: 7562 656e 6461 5d28 6874 7470 733a 2f2f  ubenda](https://
+00000670: 636c 6965 6e74 2d61 7373 6574 732e 7265  client-assets.re
+00000680: 6665 7272 616c 6361 6e64 792e 636f 6d2f  ferralcandy.com/
+00000690: 6d64 3659 3436 6a42 5435 7566 5443 4f32  md6Y46jBT5ufTCO2
+000006a0: 7a7a 4774 5f31 3636 3835 3938 3138 362e  zzGt_1668598186.
+000006b0: 706e 6729 5d28 6874 7470 3a2f 2f69 7562  png)](http://iub
+000006c0: 656e 6461 2e72 6566 722e 6363 2f64 6c72  enda.refr.cc/dlr
+000006d0: 7370 6170 6929 0a0a 0a23 2320 4368 6563  spapi)...## Chec
+000006e0: 6b20 4465 6d6f 2050 726f 6a65 6374 0a2a  k Demo Project.*
+000006f0: 2043 6865 636b 2074 6865 2064 656d 6f20   Check the demo 
+00000700: 7265 706f 206f 6e20 5b47 6974 4875 625d  repo on [GitHub]
+00000710: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000720: 636f 6d2f 444c 5253 502f 6578 616d 706c  com/DLRSP/exampl
+00000730: 652f 7472 6565 2f64 6a61 6e67 6f2d 6975  e/tree/django-iu
+00000740: 6265 6e64 6129 0a0a 2323 2052 6571 7569  benda)..## Requi
+00000750: 7265 6d65 6e74 730a 2d20 2020 5079 7468  rements.-   Pyth
+00000760: 6f6e 202b 332e 3820 7375 7070 6f72 7465  on +3.8 supporte
+00000770: 642e 0a2d 2020 2044 6a61 6e67 6f20 2b33  d..-   Django +3
+00000780: 2e32 2073 7570 706f 7274 6564 2e0a 0a23  .2 supported...#
+00000790: 2320 5365 7475 700a 312e 2049 6e73 7461  # Setup.1. Insta
+000007a0: 6c6c 2066 726f 6d20 2a2a 7069 702a 2a3a  ll from **pip**:
+000007b0: 0a20 2020 6060 6073 6865 6c6c 0a20 2020  .   ```shell.   
+000007c0: 7069 7020 696e 7374 616c 6c20 646a 616e  pip install djan
+000007d0: 676f 2d69 7562 656e 6461 0a20 2020 6060  go-iubenda.   ``
+000007e0: 600a 322e 204d 6f64 6966 7920 6073 6574  `.2. Modify `set
+000007f0: 7469 6e67 732e 7079 6020 6279 2061 6464  tings.py` by add
+00000800: 696e 6720 7468 6520 6170 7020 746f 2060  ing the app to `
+00000810: 494e 5354 414c 4c45 445f 4150 5053 603a  INSTALLED_APPS`:
+00000820: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
+00000830: 2049 4e53 5441 4c4c 4544 5f41 5050 5320   INSTALLED_APPS 
+00000840: 3d20 280a 2020 2020 2020 2022 6d6f 6465  = (.       "mode
+00000850: 6c74 7261 6e73 6c61 7469 6f6e 222c 0a20  ltranslation",. 
+00000860: 2020 2020 2020 2320 2e2e 2e0a 2020 2020        # ....    
+00000870: 2020 2022 6975 6265 6e64 6122 2c0a 2020     "iubenda",.  
+00000880: 2020 2020 2023 202e 2e2e 0a20 2020 290a       # ....   ).
+00000890: 2020 2060 6060 0a33 2e20 4d6f 6469 6679     ```.3. Modify
+000008a0: 2060 7365 7474 696e 6773 2e70 7960 2062   `settings.py` b
+000008b0: 7920 6164 6469 6e67 2074 6865 2061 7070  y adding the app
+000008c0: 2773 2063 6f6e 7465 7874 2070 726f 6365  's context proce
+000008d0: 7373 6f72 2074 6f20 6054 454d 504c 4154  ssor to `TEMPLAT
+000008e0: 4553 603a 0a20 2020 6060 6070 7974 686f  ES`:.   ```pytho
+000008f0: 6e0a 2020 2054 454d 504c 4154 4553 203d  n.   TEMPLATES =
+00000900: 205b 0a20 2020 2020 2020 7b0a 2020 2020   [.       {.    
+00000910: 2020 2020 2020 2023 202e 2e2e 0a20 2020         # ....   
+00000920: 2020 2020 2020 2020 224f 5054 494f 4e53          "OPTIONS
+00000930: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00000940: 2020 2020 2263 6f6e 7465 7874 5f70 726f      "context_pro
+00000950: 6365 7373 6f72 7322 3a20 5b0a 2020 2020  cessors": [.    
+00000960: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00000970: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00000980: 2020 2020 2020 2020 2269 7562 656e 6461          "iubenda
+00000990: 2e63 6f6e 7465 7874 5f70 726f 6365 7373  .context_process
+000009a0: 6f72 732e 6975 6265 6e64 6122 2c0a 2020  ors.iubenda",.  
+000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009c0: 2023 202e 2e2e 0a20 2020 2020 2020 2020   # ....         
+000009d0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+000009e0: 2020 2020 7d2c 0a20 2020 2020 2020 7d2c      },.       },
+000009f0: 0a20 2020 5d0a 2020 2060 6060 0a34 2e20  .   ].   ```.4. 
+00000a00: 4265 2073 7572 6520 7468 6520 446a 616e  Be sure the Djan
+00000a10: 676f 2773 204c 6f63 616c 6520 6d69 6464  go's Locale midd
+00000a20: 6c65 7761 7265 2069 7320 656e 6162 6c65  leware is enable
+00000a30: 6420 696e 7369 6465 2060 7365 7474 696e  d inside `settin
+00000a40: 6773 2e70 7960 3a0a 2020 2060 6060 7079  gs.py`:.   ```py
+00000a50: 7468 6f6e 0a20 2020 4d49 4444 4c45 5741  thon.   MIDDLEWA
+00000a60: 5245 203d 2028 0a20 2020 2020 2020 2320  RE = (.       # 
+00000a70: 2e2e 2e0a 2020 2020 2020 2022 646a 616e  ....       "djan
+00000a80: 676f 2e6d 6964 646c 6577 6172 652e 6c6f  go.middleware.lo
+00000a90: 6361 6c65 2e4c 6f63 616c 654d 6964 646c  cale.LocaleMiddl
+00000aa0: 6577 6172 6522 2c0a 2020 2020 2020 2023  eware",.       #
+00000ab0: 202e 2e2e 0a20 2020 290a 2020 2060 6060   ....   ).   ```
+00000ac0: 0a35 2e20 4f70 7469 6f6e 616c 6c79 2c20  .5. Optionally, 
+00000ad0: 6275 7420 7375 6767 7565 7374 6564 2c20  but sugguested, 
+00000ae0: 7468 6520 446a 616e 676f 2773 2043 7572  the Django's Cur
+00000af0: 7265 6e74 2053 6974 6520 6d69 6464 6c65  rent Site middle
+00000b00: 7761 7265 2069 7320 656e 6162 6c65 6420  ware is enabled 
+00000b10: 696e 7369 6465 2060 7365 7474 696e 6773  inside `settings
+00000b20: 2e70 7960 3a0a 2020 2060 6060 7079 7468  .py`:.   ```pyth
+00000b30: 6f6e 0a20 2020 4d49 4444 4c45 5741 5245  on.   MIDDLEWARE
+00000b40: 203d 2028 0a20 2020 2020 2020 2320 2e2e   = (.       # ..
+00000b50: 2e0a 2020 2020 2020 2022 646a 616e 676f  ..       "django
+00000b60: 2e63 6f6e 7472 6962 2e73 6974 6573 2e6d  .contrib.sites.m
+00000b70: 6964 646c 6577 6172 652e 4375 7272 656e  iddleware.Curren
+00000b80: 7453 6974 654d 6964 646c 6577 6172 6522  tSiteMiddleware"
+00000b90: 2c0a 2020 2020 2020 2023 202e 2e2e 0a20  ,.       # .... 
+00000ba0: 2020 290a 2020 2060 6060 0a36 2e20 4d6f    ).   ```.6. Mo
+00000bb0: 6469 6679 2060 7572 6c2e 7079 6020 6279  dify `url.py` by
+00000bc0: 2061 6464 696e 6720 7468 6520 6170 7027   adding the app'
+00000bd0: 7320 7572 6c73 2074 6f20 6075 726c 7061  s urls to `urlpa
+00000be0: 7474 6572 6e73 603a 0a20 2020 6060 6070  tterns`:.   ```p
+00000bf0: 7974 686f 6e0a 2020 2075 726c 7061 7474  ython.   urlpatt
+00000c00: 6572 6e73 202b 3d20 5b0a 2020 2020 2020  erns += [.      
+00000c10: 2070 6174 6828 2222 2c20 696e 636c 7564   path("", includ
+00000c20: 6528 2269 7562 656e 6461 2e75 726c 7322  e("iubenda.urls"
+00000c30: 2929 2c0a 2020 205d 0a20 2020 6060 600a  )),.   ].   ```.
+00000c40: 372e 204d 6f64 6966 7920 6075 726c 2e70  7. Modify `url.p
+00000c50: 7960 2062 7920 6164 6469 6e67 2074 6865  y` by adding the
+00000c60: 2061 7070 2773 2073 6974 656d 6170 7320   app's sitemaps 
+00000c70: 746f 2060 7369 7465 6d61 7073 603a 0a20  to `sitemaps`:. 
+00000c80: 2020 6060 6070 7974 686f 6e0a 2020 2066    ```python.   f
+00000c90: 726f 6d20 6975 6265 6e64 612e 7369 7465  rom iubenda.site
+00000ca0: 6d61 7073 2069 6d70 6f72 7420 5072 6976  maps import Priv
+00000cb0: 6163 7953 6974 656d 6170 2c20 436f 6f6b  acySitemap, Cook
+00000cc0: 6965 5369 7465 6d61 700a 0a20 2020 7369  ieSitemap..   si
+00000cd0: 7465 6d61 7073 203d 207b 0a20 2020 2020  temaps = {.     
+00000ce0: 2020 2320 2e2e 2e0a 2020 2020 2020 2022    # ....       "
+00000cf0: 7072 6976 6163 7922 3a20 5072 6976 6163  privacy": Privac
+00000d00: 7953 6974 656d 6170 2c0a 2020 2020 2020  ySitemap,.      
+00000d10: 2022 636f 6f6b 6965 223a 2043 6f6f 6b69   "cookie": Cooki
+00000d20: 6553 6974 656d 6170 2c0a 2020 2020 2020  eSitemap,.      
+00000d30: 2023 202e 2e2e 0a20 2020 7d0a 2020 2060   # ....   }.   `
+00000d40: 6060 0a38 2e20 4265 2073 7572 6520 7468  ``.8. Be sure th
+00000d50: 6520 7661 7269 6162 6c65 2060 4c41 4e47  e variable `LANG
+00000d60: 5541 4745 5f43 4f44 4560 2069 7320 6176  UAGE_CODE` is av
+00000d70: 6169 6c61 626c 6520 666f 7220 4854 4d4c  ailable for HTML
+00000d80: 2074 656d 706c 6174 6573 3a0a 2020 2060   templates:.   `
+00000d90: 6060 6874 6d6c 0a20 2020 7b25 206c 6f61  ``html.   {% loa
+00000da0: 6420 6931 386e 2025 7d0a 2020 207b 2520  d i18n %}.   {% 
+00000db0: 6765 745f 6375 7272 656e 745f 6c61 6e67  get_current_lang
+00000dc0: 7561 6765 2061 7320 4c41 4e47 5541 4745  uage as LANGUAGE
+00000dd0: 5f43 4f44 4520 257d 0a20 2020 6060 600a  _CODE %}.   ```.
+00000de0: 392e 204d 6f64 6966 7920 796f 7572 2070  9. Modify your p
+00000df0: 726f 6a65 6374 2773 2074 656d 706c 6174  roject's templat
+00000e00: 6520 746f 2061 6464 2070 7269 7661 6379  e to add privacy
+00000e10: 2061 6e64 2063 6f6f 6b69 6520 706f 6c69   and cookie poli
+00000e20: 6369 6573 2e0a 2020 2046 6f72 2065 7861  cies..   For exa
+00000e30: 6d70 6c65 2069 6e73 6964 6520 7468 6520  mple inside the 
+00000e40: 6066 6f6f 7465 722e 6874 6d6c 6020 6164  `footer.html` ad
+00000e50: 6420 666f 6c6c 6f77 696e 6720 636f 6465  d following code
+00000e60: 3a0a 2020 2060 6060 6874 6d6c 0a20 2020  :.   ```html.   
+00000e70: 7b25 2069 6620 6e6f 7420 6465 6275 6720  {% if not debug 
+00000e80: 257d 0a20 2020 2020 2020 7b25 2062 6c6f  %}.       {% blo
+00000e90: 636b 2069 7562 656e 6461 2025 7d7b 2520  ck iubenda %}{% 
+00000ea0: 696e 636c 7564 6520 2269 7562 656e 6461  include "iubenda
+00000eb0: 2f69 6e63 6c75 6465 2d63 6f6e 7465 6e74  /include-content
+00000ec0: 2e68 746d 6c22 2025 7d7b 2520 656e 6462  .html" %}{% endb
+00000ed0: 6c6f 636b 2069 7562 656e 6461 2025 7d0a  lock iubenda %}.
+00000ee0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+00000ef0: 2020 6060 600a 0a23 2320 4f70 7469 6f6e    ```..## Option
+00000f00: 616c 0a0a 2323 2320 4175 746f 626c 6f63  al..### Autobloc
+00000f10: 6b69 6e67 0a49 6620 4975 6265 6e64 6120  king.If Iubenda 
+00000f20: 6175 746f 626c 6f63 6b69 6e67 2773 2063  autoblocking's c
+00000f30: 6f6e 6669 6775 7261 7469 6f6e 7320 6172  onfigurations ar
+00000f40: 6520 696d 706c 656d 656e 7465 6420 696e  e implemented in
+00000f50: 2079 6f75 7220 6163 636f 756e 742c 0a74   your account,.t
+00000f60: 6865 2076 6172 6961 626c 6520 6049 5542  he variable `IUB
+00000f70: 454e 4441 5f41 5554 4f42 4c4f 434b 494e  ENDA_AUTOBLOCKIN
+00000f80: 4760 2063 616e 2062 6520 7365 7420 746f  G` can be set to
+00000f90: 2069 6d70 6f72 7420 7468 6520 7369 7465   import the site
+00000fa0: 2773 2073 6372 6970 742e 0a60 6060 6874  's script..```ht
+00000fb0: 6d6c 0a3c 7363 7269 7074 2074 7970 653d  ml.<script type=
+00000fc0: 2274 6578 742f 6a61 7661 7363 7269 7074  "text/javascript
+00000fd0: 2220 7372 633d 2268 7474 7073 3a2f 2f63  " src="https://c
+00000fe0: 732e 6975 6265 6e64 612e 636f 6d2f 6175  s.iubenda.com/au
+00000ff0: 746f 626c 6f63 6b69 6e67 2f7b 7b20 6378  toblocking/{{ cx
+00001000: 5f69 7562 656e 6461 2e69 7562 5f73 6974  _iubenda.iub_sit
+00001010: 655f 6964 207d 7d2e 6a73 223e 3c2f 7363  e_id }}.js"></sc
+00001020: 7269 7074 3e0a 6060 600a 0a23 2323 2043  ript>.```..### C
+00001030: 6f6e 7465 6e74 2053 6563 7572 6974 7920  ontent Security 
+00001040: 506f 6c69 6379 0a49 6620 436f 6e74 656e  Policy.If Conten
+00001050: 7420 5365 6375 7269 7479 2050 6f6c 6963  t Security Polic
+00001060: 7920 6172 6520 696d 706c 656d 656e 7465  y are implemente
+00001070: 6420 696e 2079 6f75 7220 7365 7276 6572  d in your server
+00001080: 2061 6e64 2069 6e6c 696e 6520 7363 7269   and inline scri
+00001090: 7074 7320 6172 6520 6469 7361 626c 6564  pts are disabled
+000010a0: 2c0a 7468 6520 7661 7269 6162 6c65 2060  ,.the variable `
+000010b0: 4955 4245 4e44 415f 4353 505f 4e4f 4e43  IUBENDA_CSP_NONC
+000010c0: 4560 2063 616e 2062 6520 7365 7420 7769  E` can be set wi
+000010d0: 7468 206e 6f6e 6365 2074 6167 2077 696c  th nonce tag wil
+000010e0: 6c20 6265 2069 6e73 6572 7465 6420 7363  l be inserted sc
+000010f0: 7269 7074 2773 206e 6f6e 6365 2e0a 6060  ript's nonce..``
+00001100: 6068 746d 6c0a 3c73 6372 6970 7420 7479  `html.<script ty
+00001110: 7065 3d22 7465 7874 2f6a 6176 6173 6372  pe="text/javascr
+00001120: 6970 7422 207b 2520 6966 2063 785f 6975  ipt" {% if cx_iu
+00001130: 6265 6e64 615f 6e6f 6e63 6520 257d 6e6f  benda_nonce %}no
+00001140: 6e63 653d 227b 7b20 6378 5f69 7562 656e  nce="{{ cx_iuben
+00001150: 6461 5f6e 6f6e 6365 207d 7d22 7b25 2065  da_nonce }}"{% e
+00001160: 6e64 6966 2025 7d3e 0a60 6060 0a49 6e73  ndif %}>.```.Ins
+00001170: 6964 6520 796f 7572 2077 6562 7365 7276  ide your webserv
+00001180: 6572 2773 2063 6f6e 6669 6775 7261 7469  er's configurati
+00001190: 6f6e 732c 2061 2072 756c 6520 746f 2064  ons, a rule to d
+000011a0: 796e 616d 6963 616c 6c79 2072 6570 6c61  ynamically repla
+000011b0: 6365 2079 6f75 7220 434f 4e53 5441 4e54  ce your CONSTANT
+000011c0: 206e 6f6e 6365 2069 6e20 6120 7261 6e64   nonce in a rand
+000011d0: 6f6d 2073 7472 696e 6720 6973 206e 6565  om string is nee
+000011e0: 6465 642e 0a0a 546f 2061 6c6c 6f77 2020  ded...To allow  
+000011f0: 6578 7465 726e 616c 2073 6f75 7263 6520  external source 
+00001200: 6672 6f6d 2049 7562 656e 6461 2064 6f6d  from Iubenda dom
+00001210: 6169 6e73 2c20 706c 6561 7365 2069 6d70  ains, please imp
+00001220: 6c65 6d65 6e74 2074 6865 7365 2072 756c  lement these rul
+00001230: 6573 3a0a 6060 6065 6469 746f 7263 6f6e  es:.```editorcon
+00001240: 6669 670a 436f 6e74 656e 742d 5365 6375  fig.Content-Secu
+00001250: 7269 7479 2d50 6f6c 6963 793a 0a20 2020  rity-Policy:.   
+00001260: 2073 6372 6970 742d 7372 632d 656c 656d   script-src-elem
+00001270: 2068 7474 7073 3a2f 2f2a 2e69 7562 656e   https://*.iuben
+00001280: 6461 2e63 6f6d 223b 0a20 2020 2069 6d67  da.com";.    img
+00001290: 2d73 7263 2068 7474 7073 3a2f 2f2a 2e69  -src https://*.i
+000012a0: 7562 656e 6461 2e63 6f6d 2064 6174 613a  ubenda.com data:
+000012b0: 223b 0a20 2020 2073 7479 6c65 2d73 7263  ";.    style-src
+000012c0: 2068 7474 7073 3a2f 2f2a 2e69 7562 656e   https://*.iuben
+000012d0: 6461 2e63 6f6d 223b 0a20 2020 2063 6f6e  da.com";.    con
+000012e0: 6e65 6374 2d73 7263 2068 7474 7073 3a2f  nect-src https:/
+000012f0: 2f2a 2e69 7562 656e 6461 2e63 6f6d 223b  /*.iubenda.com";
+00001300: 0a20 2020 2066 7261 6d65 2d73 7263 2068  .    frame-src h
+00001310: 7474 7073 3a2f 2f2a 2e69 7562 656e 6461  ttps://*.iubenda
+00001320: 2e63 6f6d 223b 0a60 6060 0a0a 4966 2079  .com";.```..If y
+00001330: 6f75 2070 7265 6665 7220 746f 206e 6f74  ou prefer to not
+00001340: 2061 6c6c 6f77 202a 2a2a 756e 7361 6665   allow ***unsafe
+00001350: 2d69 6e6c 696e 652a 2a2a 2069 6e73 6964  -inline*** insid
+00001360: 6520 796f 7572 2043 5350 2c20 706c 6561  e your CSP, plea
+00001370: 7365 2061 6c73 6f20 6164 6420 7468 6520  se also add the 
+00001380: 7477 6f20 7370 6563 6966 6963 2068 6173  two specific has
+00001390: 6820 666f 7220 796f 7572 0a73 6372 6970  h for your.scrip
+000013a0: 7420 7072 6f6d 7074 6564 2061 7320 6572  t prompted as er
+000013b0: 726f 7220 696e 204a 6176 6173 6372 6970  ror in Javascrip
+000013c0: 7420 436f 6e73 6f6c 652e 0a60 6060 6564  t Console..```ed
+000013d0: 6974 6f72 636f 6e66 6967 0a23 2049 7562  itorconfig.# Iub
+000013e0: 656e 6461 2050 7269 7661 6379 2041 6e64  enda Privacy And
+000013f0: 2043 6f6f 6b69 6520 506f 6c69 6379 202d   Cookie Policy -
+00001400: 2041 5049 0a43 6f6e 7465 6e74 2d53 6563   API.Content-Sec
+00001410: 7572 6974 792d 506f 6c69 6379 3a0a 2020  urity-Policy:.  
+00001420: 2020 2e2e 2e0a 2020 2020 7363 7269 7074    ....    script
+00001430: 2d73 7263 2d65 6c65 6d20 6874 7470 733a  -src-elem https:
+00001440: 2f2f 2a2e 6975 6265 6e64 612e 636f 6d20  //*.iubenda.com 
+00001450: 2773 6861 3235 362d 594f 5552 2d46 4952  'sha256-YOUR-FIR
+00001460: 5354 2d48 4153 482d 5052 4f4d 5054 4544  ST-HASH-PROMPTED
+00001470: 2d49 4e53 4944 452d 434f 4e53 4f4c 4527  -INSIDE-CONSOLE'
+00001480: 2027 7368 6132 3536 2d59 4f55 522d 5345   'sha256-YOUR-SE
+00001490: 434f 4e44 2d48 4153 482d 5052 4f4d 5054  COND-HASH-PROMPT
+000014a0: 4544 2d49 4e53 4944 452d 434f 4e53 4f4c  ED-INSIDE-CONSOL
+000014b0: 4527 3b0a 2020 2020 2e2e 2e0a 6060 600a  E';.    ....```.
+000014c0: 0a43 6865 636b 2074 6869 7320 6172 7469  .Check this arti
+000014d0: 636c 6520 6672 6f6d 205b 4975 6265 6e64  cle from [Iubend
+000014e0: 6120 6865 6c70 5d28 6874 7470 733a 2f2f  a help](https://
+000014f0: 7777 772e 6975 6265 6e64 612e 636f 6d2f  www.iubenda.com/
+00001500: 6974 2f68 656c 702f 3132 3334 372d 636f  it/help/12347-co
+00001510: 6d65 2d63 6f6e 6669 6775 7261 7265 2d69  me-configurare-i
+00001520: 6c2d 636f 6e74 656e 742d 7365 6375 7269  l-content-securi
+00001530: 7479 2d70 6f6c 6963 792d 7065 722d 636f  ty-policy-per-co
+00001540: 6e73 656e 7469 7265 2d6c 6573 6563 757a  nsentire-lesecuz
+00001550: 696f 6e65 2d64 6567 6c69 2d73 6372 6970  ione-degli-scrip
+00001560: 742d 6469 2d69 7562 656e 6461 290a 0a23  t-di-iubenda)..#
+00001570: 2323 2049 7562 656e 6461 2773 204f 7074  ## Iubenda's Opt
+00001580: 696f 6e73 0a0a 546f 2070 6572 736f 6e61  ions..To persona
+00001590: 6c69 7a65 2074 6865 2049 7562 656e 6461  lize the Iubenda
+000015a0: 2073 6372 6970 7427 7320 6265 6861 7669   script's behavi
+000015b0: 6f75 722c 2074 6865 2064 6963 7420 6049  our, the dict `I
+000015c0: 5542 454e 4441 5f4f 5054 494f 4e53 6020  UBENDA_OPTIONS` 
+000015d0: 6361 6e20 6265 2063 6f6e 6669 6775 7265  can be configure
+000015e0: 6420 696e 7369 6465 2060 7365 7474 696e  d inside `settin
+000015f0: 6773 2e70 7960 0a60 6060 7079 7468 6f6e  gs.py`.```python
+00001600: 0a49 5542 454e 4441 5f4f 5054 494f 4e53  .IUBENDA_OPTIONS
+00001610: 203d 207b 0a20 2020 2022 636f 756e 7472   = {.    "countr
+00001620: 7944 6574 6563 7469 6f6e 223a 2022 7472  yDetection": "tr
+00001630: 7565 222c 0a20 2020 2022 6173 6b43 6f6e  ue",.    "askCon
+00001640: 7365 6e74 4174 436f 6f6b 6965 506f 6c69  sentAtCookiePoli
+00001650: 6379 5570 6461 7465 223a 2022 7472 7565  cyUpdate": "true
+00001660: 222c 0a20 2020 2022 656e 6162 6c65 4661  ",.    "enableFa
+00001670: 6470 223a 2022 7472 7565 222c 0a20 2020  dp": "true",.   
+00001680: 2022 656e 6162 6c65 4c67 7064 223a 2022   "enableLgpd": "
+00001690: 7472 7565 222c 0a20 2020 2022 6c67 7064  true",.    "lgpd
+000016a0: 4170 706c 6965 7347 6c6f 6261 6c6c 7922  AppliesGlobally"
+000016b0: 3a20 2274 7275 6522 2c0a 2020 2020 2265  : "true",.    "e
+000016c0: 6e61 626c 6555 7370 7222 3a20 2274 7275  nableUspr": "tru
+000016d0: 6522 2c0a 2020 2020 2265 6e61 626c 6543  e",.    "enableC
+000016e0: 6370 6122 3a20 2274 7275 6522 2c0a 2020  cpa": "true",.  
+000016f0: 2020 2263 6370 6141 636b 6e6f 776c 6564    "ccpaAcknowled
+00001700: 6765 4f6e 4469 7370 6c61 7922 3a20 2274  geOnDisplay": "t
+00001710: 7275 6522 2c0a 2020 2020 2263 6370 6141  rue",.    "ccpaA
+00001720: 7070 6c69 6573 223a 2022 7472 7565 222c  pplies": "true",
+00001730: 0a20 2020 2022 636f 6e73 656e 744f 6e43  .    "consentOnC
+00001740: 6f6e 7469 6e75 6564 4272 6f77 7369 6e67  ontinuedBrowsing
+00001750: 223a 2022 6661 6c73 6522 2c0a 2020 2020  ": "false",.    
+00001760: 2266 6c6f 6174 696e 6750 7265 6665 7265  "floatingPrefere
+00001770: 6e63 6573 4275 7474 6f6e 4469 7370 6c61  ncesButtonDispla
+00001780: 7922 3a20 2262 6f74 746f 6d2d 6c65 6674  y": "bottom-left
+00001790: 222c 0a20 2020 2022 696e 7661 6c69 6461  ",.    "invalida
+000017a0: 7465 436f 6e73 656e 7457 6974 686f 7574  teConsentWithout
+000017b0: 4c6f 6722 3a20 2274 7275 6522 2c0a 2020  Log": "true",.  
+000017c0: 2020 2270 6572 5075 7270 6f73 6543 6f6e    "perPurposeCon
+000017d0: 7365 6e74 223a 2022 7472 7565 222c 0a20  sent": "true",. 
+000017e0: 2020 2022 7768 6974 656c 6162 656c 223a     "whitelabel":
+000017f0: 2022 6661 6c73 6522 2c0a 2020 2020 2262   "false",.    "b
+00001800: 616e 6e65 7222 3a20 7b0a 2020 2020 2020  anner": {.      
+00001810: 2020 2261 6363 6570 7442 7574 746f 6e44    "acceptButtonD
+00001820: 6973 706c 6179 223a 2022 7472 7565 222c  isplay": "true",
+00001830: 0a20 2020 2020 2020 2022 6261 636b 6772  .        "backgr
+00001840: 6f75 6e64 4f76 6572 6c61 7922 3a20 2274  oundOverlay": "t
+00001850: 7275 6522 2c0a 2020 2020 2020 2020 2263  rue",.        "c
+00001860: 6c6f 7365 4275 7474 6f6e 5265 6a65 6374  loseButtonReject
+00001870: 7322 3a20 2274 7275 6522 2c0a 2020 2020  s": "true",.    
+00001880: 2020 2020 2263 7573 746f 6d69 7a65 4275      "customizeBu
+00001890: 7474 6f6e 4469 7370 6c61 7922 3a20 2274  ttonDisplay": "t
+000018a0: 7275 6522 2c0a 2020 2020 2020 2020 2265  rue",.        "e
+000018b0: 7870 6c69 6369 7457 6974 6864 7261 7761  xplicitWithdrawa
+000018c0: 6c22 3a20 2274 7275 6522 2c0a 2020 2020  l": "true",.    
+000018d0: 2020 2020 2266 6f6e 7453 697a 6522 3a20      "fontSize": 
+000018e0: 2231 3470 7822 2c0a 2020 2020 2020 2020  "14px",.        
+000018f0: 226c 6973 7450 7572 706f 7365 7322 3a20  "listPurposes": 
+00001900: 2274 7275 6522 2c0a 2020 2020 2020 2020  "true",.        
+00001910: 2270 6f73 6974 696f 6e22 3a20 2266 6c6f  "position": "flo
+00001920: 6174 2d63 656e 7465 7222 2c0a 2020 2020  at-center",.    
+00001930: 2020 2020 2272 656a 6563 7442 7574 746f      "rejectButto
+00001940: 6e44 6973 706c 6179 223a 2022 7472 7565  nDisplay": "true
+00001950: 222c 0a20 2020 2020 2020 2022 7368 6f77  ",.        "show
+00001960: 5075 7270 6f73 6573 546f 6767 6c65 7322  PurposesToggles"
+00001970: 3a20 2274 7275 6522 0a20 2020 207d 2c0a  : "true".    },.
+00001980: 7d0a 6060 600a 0a23 2323 2049 6e74 6567  }.```..### Integ
+00001990: 7261 7469 6f6e 2077 6974 6820 476f 6f67  ration with Goog
+000019a0: 6c65 2054 6167 204d 616e 6167 6572 0a49  le Tag Manager.I
+000019b0: 6620 476f 6f67 6c65 2054 6167 204d 616e  f Google Tag Man
+000019c0: 6167 6572 2069 7320 696d 706c 656d 656e  ager is implemen
+000019d0: 7465 6420 696e 2079 6f75 7220 6170 706c  ted in your appl
+000019e0: 6963 6174 696f 6e20 616e 6420 616c 6c20  ication and all 
+000019f0: 6e65 6564 6564 2073 6574 7469 6e67 7320  needed settings 
+00001a00: 7765 7265 2063 6f6e 6669 6775 7265 6420  were configured 
+00001a10: 696e 7369 6465 2074 6865 2063 6f6e 7461  inside the conta
+00001a20: 696e 6572 2c0a 7468 6520 7661 7269 6162  iner,.the variab
+00001a30: 6c65 2060 4955 4245 4e44 415f 4754 4d60  le `IUBENDA_GTM`
+00001a40: 2063 616e 2062 6520 7365 7420 7769 7468   can be set with
+00001a50: 2074 6865 2076 616c 7565 2060 5472 7565   the value `True
+00001a60: 6020 616e 6420 7468 6520 4975 6265 6e64  ` and the Iubend
+00001a70: 6127 7320 6361 6c6c 6261 636b 2077 696c  a's callback wil
+00001a80: 6c20 6265 2069 6e73 6572 7465 6420 696e  l be inserted in
+00001a90: 7369 6465 2074 6865 2073 6372 6970 742e  side the script.
+00001aa0: 0a0a 466f 7220 6e65 6564 6564 2063 6f6e  ..For needed con
+00001ab0: 6669 6775 7261 7469 6f6e 2069 6e73 6964  figuration insid
+00001ac0: 6520 476f 6f67 6c65 2054 6167 204d 616e  e Google Tag Man
+00001ad0: 6167 6572 2063 6f6e 7461 696e 6572 2c20  ager container, 
+00001ae0: 706c 6561 7365 2072 6566 6572 2074 6f20  please refer to 
+00001af0: 7468 6573 6520 6e6f 7465 733a 0a2d 205b  these notes:.- [
+00001b00: 476f 6f67 6c65 2043 6f6e 7365 6e74 204d  Google Consent M
+00001b10: 6f64 655d 2868 7474 7073 3a2f 2f77 7777  ode](https://www
+00001b20: 2e69 7562 656e 6461 2e63 6f6d 2f65 6e2f  .iubenda.com/en/
+00001b30: 6865 6c70 2f32 3731 3337 2d67 6f6f 676c  help/27137-googl
+00001b40: 652d 636f 6e73 656e 742d 6d6f 6465 290a  e-consent-mode).
+00001b50: 2d20 5b47 6f6f 676c 6520 436f 6e73 656e  - [Google Consen
+00001b60: 7420 4d6f 6465 2073 6574 7570 2047 544d  t Mode setup GTM
+00001b70: 2077 6974 6820 4975 6265 6e64 615d 2868   with Iubenda](h
+00001b80: 7474 7073 3a2f 2f77 7777 2e69 7562 656e  ttps://www.iuben
+00001b90: 6461 2e63 6f6d 2f65 6e2f 6865 6c70 2f37  da.com/en/help/7
+00001ba0: 3431 3938 2d67 6f6f 676c 652d 636f 6e73  4198-google-cons
+00001bb0: 656e 742d 6d6f 6465 2d73 6574 2d75 702d  ent-mode-set-up-
+00001bc0: 676f 6f67 6c65 2d74 6167 2d6d 616e 6167  google-tag-manag
+00001bd0: 6572 2d77 6974 682d 6975 6265 6e64 6129  er-with-iubenda)
+00001be0: 0a2d 205b 4754 4d20 426c 6f63 6b69 6e67  .- [GTM Blocking
+00001bf0: 2043 6f6f 6b69 6573 5d28 6874 7470 733a   Cookies](https:
+00001c00: 2f2f 7777 772e 6975 6265 6e64 612e 636f  //www.iubenda.co
+00001c10: 6d2f 656e 2f68 656c 702f 3132 3335 2d67  m/en/help/1235-g
+00001c20: 6f6f 676c 652d 7461 672d 6d61 6e61 6765  oogle-tag-manage
+00001c30: 722d 626c 6f63 6b69 6e67 2d63 6f6f 6b69  r-blocking-cooki
+00001c40: 6573 290a 0a23 2320 5275 6e20 4578 616d  es)..## Run Exam
+00001c50: 706c 6520 5072 6f6a 6563 740a 0a60 6060  ple Project..```
+00001c60: 7368 656c 6c0a 6769 7420 636c 6f6e 6520  shell.git clone 
+00001c70: 2d2d 6465 7074 683d 3530 202d 2d62 7261  --depth=50 --bra
+00001c80: 6e63 683d 646a 616e 676f 2d69 7562 656e  nch=django-iuben
+00001c90: 6461 2068 7474 7073 3a2f 2f67 6974 6875  da https://githu
+00001ca0: 622e 636f 6d2f 444c 5253 502f 6578 616d  b.com/DLRSP/exam
+00001cb0: 706c 652e 6769 7420 444c 5253 502f 6578  ple.git DLRSP/ex
+00001cc0: 616d 706c 650a 6364 2044 4c52 5350 2f65  ample.cd DLRSP/e
+00001cd0: 7861 6d70 6c65 0a70 7974 686f 6e20 6d61  xample.python ma
+00001ce0: 6e61 6765 2e70 7920 7275 6e73 6572 7665  nage.py runserve
+00001cf0: 720a 6060 600a 0a4e 6f77 2062 726f 7773  r.```..Now brows
+00001d00: 6572 2074 6865 2061 7070 2040 2068 7474  er the app @ htt
+00001d10: 703a 2f2f 3132 372e 302e 302e 313a 3830  p://127.0.0.1:80
+00001d20: 3030 0a                                  00.
```

### Comparing `django-iubenda-1.4.1/README.md` & `django-iubenda-1.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,434 +1,572 @@
-00000000: 2320 646a 616e 676f 2d69 7562 656e 6461  # django-iubenda
-00000010: 205b 215b 5079 5069 206c 6963 656e 7365   [![PyPi license
-00000020: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000030: 6965 6c64 732e 696f 2f70 7970 692f 6c2f  ields.io/pypi/l/
-00000040: 646a 616e 676f 2d69 7562 656e 6461 2e73  django-iubenda.s
-00000050: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
-00000060: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-00000070: 692f 646a 616e 676f 2d69 7562 656e 6461  i/django-iubenda
-00000080: 290a 0a5b 215b 5079 5069 2073 7461 7475  )..[![PyPi statu
-00000090: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-000000a0: 6869 656c 6473 2e69 6f2f 7079 7069 2f73  hields.io/pypi/s
-000000b0: 7461 7475 732f 646a 616e 676f 2d69 7562  tatus/django-iub
-000000c0: 656e 6461 2e73 7667 295d 2868 7474 7073  enda.svg)](https
-000000d0: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
-000000e0: 7267 2f70 7970 692f 646a 616e 676f 2d69  rg/pypi/django-i
-000000f0: 7562 656e 6461 290a 5b21 5b50 7950 6920  ubenda).[![PyPi 
-00000100: 7665 7273 696f 6e5d 2868 7474 7073 3a2f  version](https:/
-00000110: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000120: 7079 7069 2f76 2f64 6a61 6e67 6f2d 6975  pypi/v/django-iu
-00000130: 6265 6e64 612e 7376 6729 5d28 6874 7470  benda.svg)](http
-00000140: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
-00000150: 6f72 672f 7079 7069 2f64 6a61 6e67 6f2d  org/pypi/django-
-00000160: 6975 6265 6e64 6129 0a5b 215b 5079 5069  iubenda).[![PyPi
-00000170: 2070 7974 686f 6e20 7665 7273 696f 6e5d   python version]
-00000180: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000190: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-000001a0: 6572 7369 6f6e 732f 646a 616e 676f 2d69  ersions/django-i
-000001b0: 7562 656e 6461 2e73 7667 295d 2868 7474  ubenda.svg)](htt
-000001c0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-000001d0: 2e6f 7267 2f70 7970 692f 646a 616e 676f  .org/pypi/django
-000001e0: 2d69 7562 656e 6461 290a 5b21 5b50 7950  -iubenda).[![PyP
-000001f0: 6920 646f 776e 6c6f 6164 735d 2868 7474  i downloads](htt
-00000200: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000210: 2e69 6f2f 7079 7069 2f64 6d2f 646a 616e  .io/pypi/dm/djan
-00000220: 676f 2d69 7562 656e 6461 2e73 7667 295d  go-iubenda.svg)]
-00000230: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
-00000240: 7468 6f6e 2e6f 7267 2f70 7970 692f 646a  thon.org/pypi/dj
-00000250: 616e 676f 2d69 7562 656e 6461 290a 5b21  ango-iubenda).[!
-00000260: 5b50 7950 6920 646f 776e 6c6f 6164 735d  [PyPi downloads]
-00000270: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000280: 656c 6473 2e69 6f2f 7079 7069 2f64 772f  elds.io/pypi/dw/
-00000290: 646a 616e 676f 2d69 7562 656e 6461 2e73  django-iubenda.s
-000002a0: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
-000002b0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
-000002c0: 692f 646a 616e 676f 2d69 7562 656e 6461  i/django-iubenda
-000002d0: 290a 5b21 5b50 7950 6920 646f 776e 6c6f  ).[![PyPi downlo
-000002e0: 6164 735d 2868 7474 7073 3a2f 2f69 6d67  ads](https://img
-000002f0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00000300: 2f64 642f 646a 616e 676f 2d69 7562 656e  /dd/django-iuben
-00000310: 6461 2e73 7667 295d 2868 7474 7073 3a2f  da.svg)](https:/
-00000320: 2f70 7970 692e 7079 7468 6f6e 2e6f 7267  /pypi.python.org
-00000330: 2f70 7970 692f 646a 616e 676f 2d69 7562  /pypi/django-iub
-00000340: 656e 6461 290a 0a23 2320 4769 7448 7562  enda)..## GitHub
-00000350: 2021 5b47 6974 4875 6220 7265 6c65 6173   ![GitHub releas
-00000360: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-00000370: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000380: 2f74 6167 2f44 4c52 5350 2f64 6a61 6e67  /tag/DLRSP/djang
-00000390: 6f2d 6975 6265 6e64 612e 7376 6729 2021  o-iubenda.svg) !
-000003a0: 5b47 6974 4875 6220 7265 6c65 6173 655d  [GitHub release]
-000003b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000003c0: 656c 6473 2e69 6f2f 6769 7468 7562 2f72  elds.io/github/r
-000003d0: 656c 6561 7365 2f44 4c52 5350 2f64 6a61  elease/DLRSP/dja
-000003e0: 6e67 6f2d 6975 6265 6e64 612e 7376 6729  ngo-iubenda.svg)
-000003f0: 0a0a 2323 2054 6573 7420 5b21 5b63 6f64  ..## Test [![cod
-00000400: 6563 6f76 2e69 6f5d 2868 7474 7073 3a2f  ecov.io](https:/
-00000410: 2f63 6f64 6563 6f76 2e69 6f2f 6769 7468  /codecov.io/gith
-00000420: 7562 2f44 4c52 5350 2f64 6a61 6e67 6f2d  ub/DLRSP/django-
-00000430: 6975 6265 6e64 612f 636f 7665 7261 6765  iubenda/coverage
-00000440: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
-00000450: 295d 2868 7474 7073 3a2f 2f63 6f64 6563  )](https://codec
-00000460: 6f76 2e69 6f2f 6769 7468 7562 2f44 4c52  ov.io/github/DLR
-00000470: 5350 2f64 6a61 6e67 6f2d 6975 6265 6e64  SP/django-iubend
-00000480: 613f 6272 616e 6368 3d6d 6169 6e29 205b  a?branch=main) [
-00000490: 215b 7072 652d 636f 6d6d 6974 2e63 6920  ![pre-commit.ci 
-000004a0: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
-000004b0: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
-000004c0: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
-000004d0: 7562 2f44 4c52 5350 2f64 6a61 6e67 6f2d  ub/DLRSP/django-
-000004e0: 6975 6265 6e64 612f 6d61 696e 2e73 7667  iubenda/main.svg
-000004f0: 295d 2868 7474 7073 3a2f 2f72 6573 756c  )](https://resul
-00000500: 7473 2e70 7265 2d63 6f6d 6d69 742e 6369  ts.pre-commit.ci
-00000510: 2f6c 6174 6573 742f 6769 7468 7562 2f44  /latest/github/D
-00000520: 4c52 5350 2f64 6a61 6e67 6f2d 6975 6265  LRSP/django-iube
-00000530: 6e64 612f 6d61 696e 2920 5b21 5b67 6974  nda/main) [![git
-00000540: 7468 7562 2e63 6f6d 5d28 6874 7470 733a  thub.com](https:
-00000550: 2f2f 6769 7468 7562 2e63 6f6d 2f44 4c52  //github.com/DLR
-00000560: 5350 2f64 6a61 6e67 6f2d 6975 6265 6e64  SP/django-iubend
-00000570: 612f 6163 7469 6f6e 732f 776f 726b 666c  a/actions/workfl
-00000580: 6f77 732f 6369 2e79 616d 6c2f 6261 6467  ows/ci.yaml/badg
-00000590: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-000005a0: 6769 7468 7562 2e63 6f6d 2f44 4c52 5350  github.com/DLRSP
-000005b0: 2f64 6a61 6e67 6f2d 6975 6265 6e64 612f  /django-iubenda/
-000005c0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-000005d0: 732f 6369 2e79 616d 6c29 0a0a 2323 2043  s/ci.yaml)..## C
-000005e0: 6f6d 706c 6961 6e63 6520 666f 7220 7765  ompliance for we
-000005f0: 6273 6974 6573 2061 6e64 2061 7070 730a  bsites and apps.
-00000600: 436c 6963 6b20 5b68 6572 655d 2868 7474  Click [here](htt
-00000610: 703a 2f2f 6975 6265 6e64 612e 7265 6672  p://iubenda.refr
-00000620: 2e63 632f 646c 7273 7061 7069 2920 616e  .cc/dlrspapi) an
-00000630: 6420 6765 7420 3130 2520 6469 7363 6f75  d get 10% discou
-00000640: 6e74 206f 6e20 6669 7273 7420 7965 6172  nt on first year
-00000650: 2061 7420 4975 6265 6e64 610a 5b21 5b49   at Iubenda.[![I
-00000660: 7562 656e 6461 5d28 6874 7470 733a 2f2f  ubenda](https://
-00000670: 636c 6965 6e74 2d61 7373 6574 732e 7265  client-assets.re
-00000680: 6665 7272 616c 6361 6e64 792e 636f 6d2f  ferralcandy.com/
-00000690: 6d64 3659 3436 6a42 5435 7566 5443 4f32  md6Y46jBT5ufTCO2
-000006a0: 7a7a 4774 5f31 3636 3835 3938 3138 362e  zzGt_1668598186.
-000006b0: 706e 6729 5d28 6874 7470 3a2f 2f69 7562  png)](http://iub
-000006c0: 656e 6461 2e72 6566 722e 6363 2f64 6c72  enda.refr.cc/dlr
-000006d0: 7370 6170 6929 0a0a 0a23 2320 4368 6563  spapi)...## Chec
-000006e0: 6b20 4465 6d6f 2050 726f 6a65 6374 0a2a  k Demo Project.*
-000006f0: 2043 6865 636b 2074 6865 2064 656d 6f20   Check the demo 
-00000700: 7265 706f 206f 6e20 5b47 6974 4875 625d  repo on [GitHub]
-00000710: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000720: 636f 6d2f 444c 5253 502f 6578 616d 706c  com/DLRSP/exampl
-00000730: 652f 7472 6565 2f64 6a61 6e67 6f2d 6975  e/tree/django-iu
-00000740: 6265 6e64 6129 0a0a 2323 2052 6571 7569  benda)..## Requi
-00000750: 7265 6d65 6e74 730a 2d20 2020 5079 7468  rements.-   Pyth
-00000760: 6f6e 202b 332e 3820 7375 7070 6f72 7465  on +3.8 supporte
-00000770: 642e 0a2d 2020 2044 6a61 6e67 6f20 2b33  d..-   Django +3
-00000780: 2e32 2073 7570 706f 7274 6564 2e0a 0a23  .2 supported...#
-00000790: 2320 5365 7475 700a 312e 2049 6e73 7461  # Setup.1. Insta
-000007a0: 6c6c 2066 726f 6d20 2a2a 7069 702a 2a3a  ll from **pip**:
-000007b0: 0a20 2020 6060 6073 6865 6c6c 0a20 2020  .   ```shell.   
-000007c0: 7069 7020 696e 7374 616c 6c20 646a 616e  pip install djan
-000007d0: 676f 2d69 7562 656e 6461 0a20 2020 6060  go-iubenda.   ``
-000007e0: 600a 322e 204d 6f64 6966 7920 6073 6574  `.2. Modify `set
-000007f0: 7469 6e67 732e 7079 6020 6279 2061 6464  tings.py` by add
-00000800: 696e 6720 7468 6520 6170 7020 746f 2060  ing the app to `
-00000810: 494e 5354 414c 4c45 445f 4150 5053 603a  INSTALLED_APPS`:
-00000820: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
-00000830: 2049 4e53 5441 4c4c 4544 5f41 5050 5320   INSTALLED_APPS 
-00000840: 3d20 280a 2020 2020 2020 2022 6d6f 6465  = (.       "mode
-00000850: 6c74 7261 6e73 6c61 7469 6f6e 222c 0a20  ltranslation",. 
-00000860: 2020 2020 2020 2320 2e2e 2e0a 2020 2020        # ....    
-00000870: 2020 2022 6975 6265 6e64 6122 2c0a 2020     "iubenda",.  
-00000880: 2020 2020 2023 202e 2e2e 0a20 2020 290a       # ....   ).
-00000890: 2020 2060 6060 0a33 2e20 4d6f 6469 6679     ```.3. Modify
-000008a0: 2060 7365 7474 696e 6773 2e70 7960 2062   `settings.py` b
-000008b0: 7920 6164 6469 6e67 2074 6865 2061 7070  y adding the app
-000008c0: 2773 2063 6f6e 7465 7874 2070 726f 6365  's context proce
-000008d0: 7373 6f72 2074 6f20 6054 454d 504c 4154  ssor to `TEMPLAT
-000008e0: 4553 603a 0a20 2020 6060 6070 7974 686f  ES`:.   ```pytho
-000008f0: 6e0a 2020 2054 454d 504c 4154 4553 203d  n.   TEMPLATES =
-00000900: 205b 0a20 2020 2020 2020 7b0a 2020 2020   [.       {.    
-00000910: 2020 2020 2020 2023 202e 2e2e 0a20 2020         # ....   
-00000920: 2020 2020 2020 2020 224f 5054 494f 4e53          "OPTIONS
-00000930: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000940: 2020 2020 2263 6f6e 7465 7874 5f70 726f      "context_pro
-00000950: 6365 7373 6f72 7322 3a20 5b0a 2020 2020  cessors": [.    
-00000960: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00000970: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00000980: 2020 2020 2020 2020 2269 7562 656e 6461          "iubenda
-00000990: 2e63 6f6e 7465 7874 5f70 726f 6365 7373  .context_process
-000009a0: 6f72 732e 6975 6265 6e64 6122 2c0a 2020  ors.iubenda",.  
-000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 2023 202e 2e2e 0a20 2020 2020 2020 2020   # ....         
-000009d0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-000009e0: 2020 2020 7d2c 0a20 2020 2020 2020 7d2c      },.       },
-000009f0: 0a20 2020 5d0a 2020 2060 6060 0a34 2e20  .   ].   ```.4. 
-00000a00: 4265 2073 7572 6520 7468 6520 446a 616e  Be sure the Djan
-00000a10: 676f 2773 204c 6f63 616c 6520 6d69 6464  go's Locale midd
-00000a20: 6c65 7761 7265 2069 7320 656e 6162 6c65  leware is enable
-00000a30: 6420 696e 7369 6465 2060 7365 7474 696e  d inside `settin
-00000a40: 6773 2e70 7960 3a0a 2020 2060 6060 7079  gs.py`:.   ```py
-00000a50: 7468 6f6e 0a20 2020 4d49 4444 4c45 5741  thon.   MIDDLEWA
-00000a60: 5245 203d 2028 0a20 2020 2020 2020 2320  RE = (.       # 
-00000a70: 2e2e 2e0a 2020 2020 2020 2022 646a 616e  ....       "djan
-00000a80: 676f 2e6d 6964 646c 6577 6172 652e 6c6f  go.middleware.lo
-00000a90: 6361 6c65 2e4c 6f63 616c 654d 6964 646c  cale.LocaleMiddl
-00000aa0: 6577 6172 6522 2c0a 2020 2020 2020 2023  eware",.       #
-00000ab0: 202e 2e2e 0a20 2020 290a 2020 2060 6060   ....   ).   ```
-00000ac0: 0a35 2e20 4f70 7469 6f6e 616c 6c79 2c20  .5. Optionally, 
-00000ad0: 6275 7420 7375 6767 7565 7374 6564 2c20  but sugguested, 
-00000ae0: 7468 6520 446a 616e 676f 2773 2043 7572  the Django's Cur
-00000af0: 7265 6e74 2053 6974 6520 6d69 6464 6c65  rent Site middle
-00000b00: 7761 7265 2069 7320 656e 6162 6c65 6420  ware is enabled 
-00000b10: 696e 7369 6465 2060 7365 7474 696e 6773  inside `settings
-00000b20: 2e70 7960 3a0a 2020 2060 6060 7079 7468  .py`:.   ```pyth
-00000b30: 6f6e 0a20 2020 4d49 4444 4c45 5741 5245  on.   MIDDLEWARE
-00000b40: 203d 2028 0a20 2020 2020 2020 2320 2e2e   = (.       # ..
-00000b50: 2e0a 2020 2020 2020 2022 646a 616e 676f  ..       "django
-00000b60: 2e63 6f6e 7472 6962 2e73 6974 6573 2e6d  .contrib.sites.m
-00000b70: 6964 646c 6577 6172 652e 4375 7272 656e  iddleware.Curren
-00000b80: 7453 6974 654d 6964 646c 6577 6172 6522  tSiteMiddleware"
-00000b90: 2c0a 2020 2020 2020 2023 202e 2e2e 0a20  ,.       # .... 
-00000ba0: 2020 290a 2020 2060 6060 0a36 2e20 4d6f    ).   ```.6. Mo
-00000bb0: 6469 6679 2060 7572 6c2e 7079 6020 6279  dify `url.py` by
-00000bc0: 2061 6464 696e 6720 7468 6520 6170 7027   adding the app'
-00000bd0: 7320 7572 6c73 2074 6f20 6075 726c 7061  s urls to `urlpa
-00000be0: 7474 6572 6e73 603a 0a20 2020 6060 6070  tterns`:.   ```p
-00000bf0: 7974 686f 6e0a 2020 2075 726c 7061 7474  ython.   urlpatt
-00000c00: 6572 6e73 202b 3d20 5b0a 2020 2020 2020  erns += [.      
-00000c10: 2070 6174 6828 2222 2c20 696e 636c 7564   path("", includ
-00000c20: 6528 2269 7562 656e 6461 2e75 726c 7322  e("iubenda.urls"
-00000c30: 2929 2c0a 2020 205d 0a20 2020 6060 600a  )),.   ].   ```.
-00000c40: 372e 204d 6f64 6966 7920 6075 726c 2e70  7. Modify `url.p
-00000c50: 7960 2062 7920 6164 6469 6e67 2074 6865  y` by adding the
-00000c60: 2061 7070 2773 2073 6974 656d 6170 7320   app's sitemaps 
-00000c70: 746f 2060 7369 7465 6d61 7073 603a 0a20  to `sitemaps`:. 
-00000c80: 2020 6060 6070 7974 686f 6e0a 2020 2066    ```python.   f
-00000c90: 726f 6d20 6975 6265 6e64 612e 7369 7465  rom iubenda.site
-00000ca0: 6d61 7073 2069 6d70 6f72 7420 5072 6976  maps import Priv
-00000cb0: 6163 7953 6974 656d 6170 2c20 436f 6f6b  acySitemap, Cook
-00000cc0: 6965 5369 7465 6d61 700a 2020 200a 2020  ieSitemap.   .  
-00000cd0: 2073 6974 656d 6170 7320 3d20 7b0a 2020   sitemaps = {.  
-00000ce0: 2020 2020 2023 202e 2e2e 0a20 2020 2020       # ....     
-00000cf0: 2020 2270 7269 7661 6379 223a 2050 7269    "privacy": Pri
-00000d00: 7661 6379 5369 7465 6d61 702c 0a20 2020  vacySitemap,.   
-00000d10: 2020 2020 2263 6f6f 6b69 6522 3a20 436f      "cookie": Co
-00000d20: 6f6b 6965 5369 7465 6d61 702c 0a20 2020  okieSitemap,.   
-00000d30: 2020 2020 2320 2e2e 2e0a 2020 207d 0a20      # ....   }. 
-00000d40: 2020 6060 600a 382e 2042 6520 7375 7265    ```.8. Be sure
-00000d50: 2074 6865 2076 6172 6961 626c 6520 604c   the variable `L
-00000d60: 414e 4755 4147 455f 434f 4445 6020 6973  ANGUAGE_CODE` is
-00000d70: 2061 7661 696c 6162 6c65 2066 6f72 2048   available for H
-00000d80: 544d 4c20 7465 6d70 6c61 7465 733a 0a20  TML templates:. 
-00000d90: 2020 6060 6068 746d 6c0a 2020 207b 2520    ```html.   {% 
-00000da0: 6c6f 6164 2069 3138 6e20 257d 0a20 2020  load i18n %}.   
-00000db0: 7b25 2067 6574 5f63 7572 7265 6e74 5f6c  {% get_current_l
-00000dc0: 616e 6775 6167 6520 6173 204c 414e 4755  anguage as LANGU
-00000dd0: 4147 455f 434f 4445 2025 7d0a 2020 2060  AGE_CODE %}.   `
-00000de0: 6060 0a39 2e20 4d6f 6469 6679 2079 6f75  ``.9. Modify you
-00000df0: 7220 7072 6f6a 6563 7427 7320 7465 6d70  r project's temp
-00000e00: 6c61 7465 2074 6f20 6164 6420 7072 6976  late to add priv
-00000e10: 6163 7920 616e 6420 636f 6f6b 6965 2070  acy and cookie p
-00000e20: 6f6c 6963 6965 732e 0a20 2020 466f 7220  olicies..   For 
-00000e30: 6578 616d 706c 6520 696e 7369 6465 2074  example inside t
-00000e40: 6865 2060 666f 6f74 6572 2e68 746d 6c60  he `footer.html`
-00000e50: 2061 6464 2066 6f6c 6c6f 7769 6e67 2063   add following c
-00000e60: 6f64 653a 0a20 2020 6060 6068 746d 6c0a  ode:.   ```html.
-00000e70: 2020 207b 2520 6966 206e 6f74 2064 6562     {% if not deb
-00000e80: 7567 2025 7d0a 2020 2020 2020 207b 2520  ug %}.       {% 
-00000e90: 626c 6f63 6b20 6975 6265 6e64 6120 257d  block iubenda %}
-00000ea0: 7b25 2069 6e63 6c75 6465 2022 6975 6265  {% include "iube
-00000eb0: 6e64 612f 696e 636c 7564 652d 636f 6e74  nda/include-cont
-00000ec0: 656e 742e 6874 6d6c 2220 257d 7b25 2065  ent.html" %}{% e
-00000ed0: 6e64 626c 6f63 6b20 6975 6265 6e64 6120  ndblock iubenda 
-00000ee0: 257d 0a20 2020 7b25 2065 6e64 6966 2025  %}.   {% endif %
-00000ef0: 7d0a 2020 2060 6060 0a0a 2323 204f 7074  }.   ```..## Opt
-00000f00: 696f 6e61 6c0a 0a23 2323 2043 6f6e 7465  ional..### Conte
-00000f10: 6e74 2053 6563 7572 6974 7920 506f 6c69  nt Security Poli
-00000f20: 6379 0a49 6620 436f 6e74 656e 7420 5365  cy.If Content Se
-00000f30: 6375 7269 7479 2050 6f6c 6963 7920 6172  curity Policy ar
-00000f40: 6520 696d 706c 656d 656e 7465 6420 696e  e implemented in
-00000f50: 2079 6f75 7220 7365 7276 6572 2061 6e64   your server and
-00000f60: 2069 6e6c 696e 6520 7363 7269 7074 7320   inline scripts 
-00000f70: 6172 6520 6469 7361 626c 6564 2c0a 7468  are disabled,.th
-00000f80: 6520 7661 7269 6162 6c65 2060 4955 4245  e variable `IUBE
-00000f90: 4e44 415f 4353 505f 4e4f 4e43 4560 2063  NDA_CSP_NONCE` c
-00000fa0: 616e 2062 6520 7365 7420 7769 7468 206e  an be set with n
-00000fb0: 6f6e 6365 2074 6167 2077 696c 6c20 6265  once tag will be
-00000fc0: 2069 6e73 6572 7465 6420 7363 7269 7074   inserted script
-00000fd0: 2773 206e 6f6e 6365 2e0a 6060 6068 746d  's nonce..```htm
-00000fe0: 6c0a 3c73 6372 6970 7420 7479 7065 3d22  l.<script type="
-00000ff0: 7465 7874 2f6a 6176 6173 6372 6970 7422  text/javascript"
-00001000: 207b 2520 6966 2063 785f 6975 6265 6e64   {% if cx_iubend
-00001010: 615f 6e6f 6e63 6520 257d 6e6f 6e63 653d  a_nonce %}nonce=
-00001020: 227b 7b20 6378 5f69 7562 656e 6461 5f6e  "{{ cx_iubenda_n
-00001030: 6f6e 6365 207d 7d22 7b25 2065 6e64 6966  once }}"{% endif
-00001040: 2025 7d3e 0a60 6060 0a49 6e73 6964 6520   %}>.```.Inside 
-00001050: 796f 7572 2077 6562 7365 7276 6572 2773  your webserver's
-00001060: 2063 6f6e 6669 6775 7261 7469 6f6e 732c   configurations,
-00001070: 2061 2072 756c 6520 746f 2064 796e 616d   a rule to dynam
-00001080: 6963 616c 6c79 2072 6570 6c61 6365 2079  ically replace y
-00001090: 6f75 7220 434f 4e53 5441 4e54 206e 6f6e  our CONSTANT non
-000010a0: 6365 2069 6e20 6120 7261 6e64 6f6d 2073  ce in a random s
-000010b0: 7472 696e 6720 6973 206e 6565 6465 642e  tring is needed.
-000010c0: 0a0a 546f 2061 6c6c 6f77 2020 6578 7465  ..To allow  exte
-000010d0: 726e 616c 2073 6f75 7263 6520 6672 6f6d  rnal source from
-000010e0: 2049 7562 656e 6461 2064 6f6d 6169 6e73   Iubenda domains
-000010f0: 2c20 706c 6561 7365 2069 6d70 6c65 6d65  , please impleme
-00001100: 6e74 2074 6865 7365 2072 756c 6573 3a0a  nt these rules:.
-00001110: 6060 6065 6469 746f 7263 6f6e 6669 670a  ```editorconfig.
-00001120: 436f 6e74 656e 742d 5365 6375 7269 7479  Content-Security
-00001130: 2d50 6f6c 6963 793a 0a20 2020 2073 6372  -Policy:.    scr
-00001140: 6970 742d 7372 632d 656c 656d 2068 7474  ipt-src-elem htt
-00001150: 7073 3a2f 2f2a 2e69 7562 656e 6461 2e63  ps://*.iubenda.c
-00001160: 6f6d 223b 0a20 2020 2069 6d67 2d73 7263  om";.    img-src
-00001170: 2068 7474 7073 3a2f 2f2a 2e69 7562 656e   https://*.iuben
-00001180: 6461 2e63 6f6d 2064 6174 613a 223b 0a20  da.com data:";. 
-00001190: 2020 2073 7479 6c65 2d73 7263 2068 7474     style-src htt
-000011a0: 7073 3a2f 2f2a 2e69 7562 656e 6461 2e63  ps://*.iubenda.c
-000011b0: 6f6d 223b 0a20 2020 2063 6f6e 6e65 6374  om";.    connect
-000011c0: 2d73 7263 2068 7474 7073 3a2f 2f2a 2e69  -src https://*.i
-000011d0: 7562 656e 6461 2e63 6f6d 223b 0a20 2020  ubenda.com";.   
-000011e0: 2066 7261 6d65 2d73 7263 2068 7474 7073   frame-src https
-000011f0: 3a2f 2f2a 2e69 7562 656e 6461 2e63 6f6d  ://*.iubenda.com
-00001200: 223b 0a60 6060 0a0a 4966 2079 6f75 2070  ";.```..If you p
-00001210: 7265 6665 7220 746f 206e 6f74 2061 6c6c  refer to not all
-00001220: 6f77 202a 2a2a 756e 7361 6665 2d69 6e6c  ow ***unsafe-inl
-00001230: 696e 652a 2a2a 2069 6e73 6964 6520 796f  ine*** inside yo
-00001240: 7572 2043 5350 2c20 706c 6561 7365 2061  ur CSP, please a
-00001250: 6c73 6f20 6164 6420 7468 6520 7477 6f20  lso add the two 
-00001260: 7370 6563 6966 6963 2068 6173 6820 666f  specific hash fo
-00001270: 7220 796f 7572 0a73 6372 6970 7420 7072  r your.script pr
-00001280: 6f6d 7074 6564 2061 7320 6572 726f 7220  ompted as error 
-00001290: 696e 204a 6176 6173 6372 6970 7420 436f  in Javascript Co
-000012a0: 6e73 6f6c 652e 0a60 6060 6564 6974 6f72  nsole..```editor
-000012b0: 636f 6e66 6967 0a23 2049 7562 656e 6461  config.# Iubenda
-000012c0: 2050 7269 7661 6379 2041 6e64 2043 6f6f   Privacy And Coo
-000012d0: 6b69 6520 506f 6c69 6379 202d 2041 5049  kie Policy - API
-000012e0: 0a43 6f6e 7465 6e74 2d53 6563 7572 6974  .Content-Securit
-000012f0: 792d 506f 6c69 6379 3a0a 2020 2020 2e2e  y-Policy:.    ..
-00001300: 2e0a 2020 2020 7363 7269 7074 2d73 7263  ..    script-src
-00001310: 2d65 6c65 6d20 6874 7470 733a 2f2f 2a2e  -elem https://*.
-00001320: 6975 6265 6e64 612e 636f 6d20 2773 6861  iubenda.com 'sha
-00001330: 3235 362d 594f 5552 2d46 4952 5354 2d48  256-YOUR-FIRST-H
-00001340: 4153 482d 5052 4f4d 5054 4544 2d49 4e53  ASH-PROMPTED-INS
-00001350: 4944 452d 434f 4e53 4f4c 4527 2027 7368  IDE-CONSOLE' 'sh
-00001360: 6132 3536 2d59 4f55 522d 5345 434f 4e44  a256-YOUR-SECOND
-00001370: 2d48 4153 482d 5052 4f4d 5054 4544 2d49  -HASH-PROMPTED-I
-00001380: 4e53 4944 452d 434f 4e53 4f4c 4527 3b0a  NSIDE-CONSOLE';.
-00001390: 2020 2020 2e2e 2e0a 6060 600a 0a43 6865      ....```..Che
-000013a0: 636b 2074 6869 7320 6172 7469 636c 6520  ck this article 
-000013b0: 6672 6f6d 205b 4975 6265 6e64 6120 6865  from [Iubenda he
-000013c0: 6c70 5d28 6874 7470 733a 2f2f 7777 772e  lp](https://www.
-000013d0: 6975 6265 6e64 612e 636f 6d2f 6974 2f68  iubenda.com/it/h
-000013e0: 656c 702f 3132 3334 372d 636f 6d65 2d63  elp/12347-come-c
-000013f0: 6f6e 6669 6775 7261 7265 2d69 6c2d 636f  onfigurare-il-co
-00001400: 6e74 656e 742d 7365 6375 7269 7479 2d70  ntent-security-p
-00001410: 6f6c 6963 792d 7065 722d 636f 6e73 656e  olicy-per-consen
-00001420: 7469 7265 2d6c 6573 6563 757a 696f 6e65  tire-lesecuzione
-00001430: 2d64 6567 6c69 2d73 6372 6970 742d 6469  -degli-script-di
-00001440: 2d69 7562 656e 6461 290a 0a23 2323 2049  -iubenda)..### I
-00001450: 7562 656e 6461 2773 204f 7074 696f 6e73  ubenda's Options
-00001460: 0a0a 546f 2070 6572 736f 6e61 6c69 7a65  ..To personalize
-00001470: 2074 6865 2049 7562 656e 6461 2073 6372   the Iubenda scr
-00001480: 6970 7427 7320 6265 6861 7669 6f75 722c  ipt's behaviour,
-00001490: 2074 6865 2064 6963 7420 6049 5542 454e   the dict `IUBEN
-000014a0: 4441 5f4f 5054 494f 4e53 6020 6361 6e20  DA_OPTIONS` can 
-000014b0: 6265 2063 6f6e 6669 6775 7265 6420 696e  be configured in
-000014c0: 7369 6465 2060 7365 7474 696e 6773 2e70  side `settings.p
-000014d0: 7960 0a60 6060 7079 7468 6f6e 0a49 5542  y`.```python.IUB
-000014e0: 454e 4441 5f4f 5054 494f 4e53 203d 207b  ENDA_OPTIONS = {
-000014f0: 0a20 2020 2022 6363 7061 4163 6b6e 6f77  .    "ccpaAcknow
-00001500: 6c65 6467 654f 6e44 6973 706c 6179 223a  ledgeOnDisplay":
-00001510: 2022 7472 7565 222c 0a20 2020 2022 6363   "true",.    "cc
-00001520: 7061 4170 706c 6965 7322 3a20 2274 7275  paApplies": "tru
-00001530: 6522 2c0a 2020 2020 2263 6f6e 7365 6e74  e",.    "consent
-00001540: 4f6e 436f 6e74 696e 7565 6442 726f 7773  OnContinuedBrows
-00001550: 696e 6722 3a20 2266 616c 7365 222c 0a20  ing": "false",. 
-00001560: 2020 2022 656e 6162 6c65 4363 7061 223a     "enableCcpa":
-00001570: 2022 7472 7565 222c 0a20 2020 2022 666c   "true",.    "fl
-00001580: 6f61 7469 6e67 5072 6566 6572 656e 6365  oatingPreference
-00001590: 7342 7574 746f 6e44 6973 706c 6179 223a  sButtonDisplay":
-000015a0: 2022 626f 7474 6f6d 2d6c 6566 7422 2c0a   "bottom-left",.
-000015b0: 2020 2020 2269 6e76 616c 6964 6174 6543      "invalidateC
-000015c0: 6f6e 7365 6e74 5769 7468 6f75 744c 6f67  onsentWithoutLog
-000015d0: 223a 2022 7472 7565 222c 0a20 2020 2022  ": "true",.    "
-000015e0: 7065 7250 7572 706f 7365 436f 6e73 656e  perPurposeConsen
-000015f0: 7422 3a20 2274 7275 6522 2c0a 2020 2020  t": "true",.    
-00001600: 2277 6869 7465 6c61 6265 6c22 3a20 2266  "whitelabel": "f
-00001610: 616c 7365 222c 0a20 2020 2022 6261 6e6e  alse",.    "bann
-00001620: 6572 223a 207b 0a20 2020 2020 2020 2022  er": {.        "
-00001630: 6163 6365 7074 4275 7474 6f6e 4469 7370  acceptButtonDisp
-00001640: 6c61 7922 3a20 2274 7275 6522 2c0a 2020  lay": "true",.  
-00001650: 2020 2020 2020 2262 6163 6b67 726f 756e        "backgroun
-00001660: 644f 7665 726c 6179 223a 2022 7472 7565  dOverlay": "true
-00001670: 222c 0a20 2020 2020 2020 2022 636c 6f73  ",.        "clos
-00001680: 6542 7574 746f 6e52 656a 6563 7473 223a  eButtonRejects":
-00001690: 2022 7472 7565 222c 0a20 2020 2020 2020   "true",.       
-000016a0: 2022 6375 7374 6f6d 697a 6542 7574 746f   "customizeButto
-000016b0: 6e44 6973 706c 6179 223a 2022 7472 7565  nDisplay": "true
-000016c0: 222c 0a20 2020 2020 2020 2022 6578 706c  ",.        "expl
-000016d0: 6963 6974 5769 7468 6472 6177 616c 223a  icitWithdrawal":
-000016e0: 2022 7472 7565 222c 0a20 2020 2020 2020   "true",.       
-000016f0: 2022 666f 6e74 5369 7a65 223a 2022 3134   "fontSize": "14
-00001700: 7078 222c 0a20 2020 2020 2020 2022 6c69  px",.        "li
-00001710: 7374 5075 7270 6f73 6573 223a 2022 7472  stPurposes": "tr
-00001720: 7565 222c 0a20 2020 2020 2020 2022 706f  ue",.        "po
-00001730: 7369 7469 6f6e 223a 2022 666c 6f61 742d  sition": "float-
-00001740: 6365 6e74 6572 222c 0a20 2020 2020 2020  center",.       
-00001750: 2022 7265 6a65 6374 4275 7474 6f6e 4469   "rejectButtonDi
-00001760: 7370 6c61 7922 3a20 2274 7275 6522 2c0a  splay": "true",.
-00001770: 2020 2020 7d2c 0a7d 0a60 6060 0a0a 2323      },.}.```..##
-00001780: 2320 496e 7465 6772 6174 696f 6e20 7769  # Integration wi
-00001790: 7468 2047 6f6f 676c 6520 5461 6720 4d61  th Google Tag Ma
-000017a0: 6e61 6765 720a 4966 2047 6f6f 676c 6520  nager.If Google 
-000017b0: 5461 6720 4d61 6e61 6765 7220 6973 2069  Tag Manager is i
-000017c0: 6d70 6c65 6d65 6e74 6564 2069 6e20 796f  mplemented in yo
-000017d0: 7572 2061 7070 6c69 6361 7469 6f6e 2061  ur application a
-000017e0: 6e64 2061 6c6c 206e 6565 6465 6420 7365  nd all needed se
-000017f0: 7474 696e 6773 2077 6572 6520 636f 6e66  ttings were conf
-00001800: 6967 7572 6564 2069 6e73 6964 6520 7468  igured inside th
-00001810: 6520 636f 6e74 6169 6e65 722c 0a74 6865  e container,.the
-00001820: 2076 6172 6961 626c 6520 6049 5542 454e   variable `IUBEN
-00001830: 4441 5f47 544d 6020 6361 6e20 6265 2073  DA_GTM` can be s
-00001840: 6574 2077 6974 6820 7468 6520 7661 6c75  et with the valu
-00001850: 6520 6054 7275 6560 2061 6e64 2074 6865  e `True` and the
-00001860: 2049 7562 656e 6461 2773 2063 616c 6c62   Iubenda's callb
-00001870: 6163 6b20 7769 6c6c 2062 6520 696e 7365  ack will be inse
-00001880: 7274 6564 2069 6e73 6964 6520 7468 6520  rted inside the 
-00001890: 7363 7269 7074 2e0a 0a46 6f72 206e 6565  script...For nee
-000018a0: 6465 6420 636f 6e66 6967 7572 6174 696f  ded configuratio
-000018b0: 6e20 696e 7369 6465 2047 6f6f 676c 6520  n inside Google 
-000018c0: 5461 6720 4d61 6e61 6765 7220 636f 6e74  Tag Manager cont
-000018d0: 6169 6e65 722c 2070 6c65 6173 6520 7265  ainer, please re
-000018e0: 6665 7220 746f 2074 6865 7365 206e 6f74  fer to these not
-000018f0: 6573 3a0a 2d20 5b47 6f6f 676c 6520 436f  es:.- [Google Co
-00001900: 6e73 656e 7420 4d6f 6465 5d28 6874 7470  nsent Mode](http
-00001910: 733a 2f2f 7777 772e 6975 6265 6e64 612e  s://www.iubenda.
-00001920: 636f 6d2f 656e 2f68 656c 702f 3237 3133  com/en/help/2713
-00001930: 372d 676f 6f67 6c65 2d63 6f6e 7365 6e74  7-google-consent
-00001940: 2d6d 6f64 6529 0a2d 205b 476f 6f67 6c65  -mode).- [Google
-00001950: 2043 6f6e 7365 6e74 204d 6f64 6520 7365   Consent Mode se
-00001960: 7475 7020 4754 4d20 7769 7468 2049 7562  tup GTM with Iub
-00001970: 656e 6461 5d28 6874 7470 733a 2f2f 7777  enda](https://ww
-00001980: 772e 6975 6265 6e64 612e 636f 6d2f 656e  w.iubenda.com/en
-00001990: 2f68 656c 702f 3734 3139 382d 676f 6f67  /help/74198-goog
-000019a0: 6c65 2d63 6f6e 7365 6e74 2d6d 6f64 652d  le-consent-mode-
-000019b0: 7365 742d 7570 2d67 6f6f 676c 652d 7461  set-up-google-ta
-000019c0: 672d 6d61 6e61 6765 722d 7769 7468 2d69  g-manager-with-i
-000019d0: 7562 656e 6461 290a 2d20 5b47 544d 2042  ubenda).- [GTM B
-000019e0: 6c6f 636b 696e 6720 436f 6f6b 6965 735d  locking Cookies]
-000019f0: 2868 7474 7073 3a2f 2f77 7777 2e69 7562  (https://www.iub
-00001a00: 656e 6461 2e63 6f6d 2f65 6e2f 6865 6c70  enda.com/en/help
-00001a10: 2f31 3233 352d 676f 6f67 6c65 2d74 6167  /1235-google-tag
-00001a20: 2d6d 616e 6167 6572 2d62 6c6f 636b 696e  -manager-blockin
-00001a30: 672d 636f 6f6b 6965 7329 0a0a 2323 2052  g-cookies)..## R
-00001a40: 756e 2045 7861 6d70 6c65 2050 726f 6a65  un Example Proje
-00001a50: 6374 0a0a 6060 6073 6865 6c6c 0a67 6974  ct..```shell.git
-00001a60: 2063 6c6f 6e65 202d 2d64 6570 7468 3d35   clone --depth=5
-00001a70: 3020 2d2d 6272 616e 6368 3d64 6a61 6e67  0 --branch=djang
-00001a80: 6f2d 6975 6265 6e64 6120 6874 7470 733a  o-iubenda https:
-00001a90: 2f2f 6769 7468 7562 2e63 6f6d 2f44 4c52  //github.com/DLR
-00001aa0: 5350 2f65 7861 6d70 6c65 2e67 6974 2044  SP/example.git D
-00001ab0: 4c52 5350 2f65 7861 6d70 6c65 0a63 6420  LRSP/example.cd 
-00001ac0: 444c 5253 502f 6578 616d 706c 650a 7079  DLRSP/example.py
-00001ad0: 7468 6f6e 206d 616e 6167 652e 7079 2072  thon manage.py r
-00001ae0: 756e 7365 7276 6572 0a60 6060 0a0a 4e6f  unserver.```..No
-00001af0: 7720 6272 6f77 7365 7220 7468 6520 6170  w browser the ap
-00001b00: 7020 4020 6874 7470 3a2f 2f31 3237 2e30  p @ http://127.0
-00001b10: 2e30 2e31 3a38 3030 300a                 .0.1:8000.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 646a 616e  : 2.1.Name: djan
+00000020: 676f 2d69 7562 656e 6461 0a56 6572 7369  go-iubenda.Versi
+00000030: 6f6e 3a20 312e 352e 300a 5375 6d6d 6172  on: 1.5.0.Summar
+00000040: 793a 2044 6a61 6e67 6f27 2773 2061 7070  y: Django''s app
+00000050: 6c69 6361 7469 6f6e 2066 6f72 2068 616e  lication for han
+00000060: 646c 696e 6720 7072 6976 6163 7920 616e  dling privacy an
+00000070: 6420 636f 6f6b 6965 2070 6f6c 6963 6965  d cookie policie
+00000080: 7320 636f 6e66 6967 7572 6564 2077 6974  s configured wit
+00000090: 6820 4975 6265 6e64 612e 0a48 6f6d 652d  h Iubenda..Home-
+000000a0: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
+000000b0: 7468 7562 2e63 6f6d 2f44 4c52 5350 2f64  thub.com/DLRSP/d
+000000c0: 6a61 6e67 6f2d 6975 6265 6e64 610a 4175  jango-iubenda.Au
+000000d0: 7468 6f72 3a20 444c 5253 500a 4175 7468  thor: DLRSP.Auth
+000000e0: 6f72 2d65 6d61 696c 3a20 646c 7273 702e  or-email: dlrsp.
+000000f0: 6465 7640 676d 6169 6c2e 636f 6d0a 4c69  dev@gmail.com.Li
+00000100: 6365 6e73 653a 204d 4954 204c 6963 656e  cense: MIT Licen
+00000110: 7365 0a4b 6579 776f 7264 733a 2064 6a61  se.Keywords: dja
+00000120: 6e67 6f2c 6975 6265 6e64 612c 7072 6976  ngo,iubenda,priv
+00000130: 6163 792c 636f 6f6b 6965 0a43 6c61 7373  acy,cookie.Class
+00000140: 6966 6965 723a 2044 6576 656c 6f70 6d65  ifier: Developme
+00000150: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
+00000160: 2042 6574 610a 436c 6173 7369 6669 6572   Beta.Classifier
+00000170: 3a20 456e 7669 726f 6e6d 656e 7420 3a3a  : Environment ::
+00000180: 2057 6562 2045 6e76 6972 6f6e 6d65 6e74   Web Environment
+00000190: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
+000001a0: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+000001b0: 0a43 6c61 7373 6966 6965 723a 2046 7261  .Classifier: Fra
+000001c0: 6d65 776f 726b 203a 3a20 446a 616e 676f  mework :: Django
+000001d0: 203a 3a20 332e 320a 436c 6173 7369 6669   :: 3.2.Classifi
+000001e0: 6572 3a20 4672 616d 6577 6f72 6b20 3a3a  er: Framework ::
+000001f0: 2044 6a61 6e67 6f20 3a3a 2034 2e30 0a43   Django :: 4.0.C
+00000200: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
+00000210: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000220: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
+00000230: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000240: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000250: 3a20 4d49 5420 4c69 6365 6e73 650a 436c  : MIT License.Cl
+00000260: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000270: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+00000280: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
+00000290: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002b0: 2050 7974 686f 6e0a 436c 6173 7369 6669   Python.Classifi
+000002c0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002e0: 6f6e 203a 3a20 330a 436c 6173 7369 6669  on :: 3.Classifi
+000002f0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000300: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000310: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790a  on :: 3 :: Only.
+00000320: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000340: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000350: 380a 436c 6173 7369 6669 6572 3a20 5072  8.Classifier: Pr
+00000360: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000370: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000380: 332e 390a 436c 6173 7369 6669 6572 3a20  3.9.Classifier: 
+00000390: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003b0: 3a20 332e 3130 0a43 6c61 7373 6966 6965  : 3.10.Classifie
+000003c0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000003d0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000003e0: 6e20 3a3a 2033 2e31 310a 436c 6173 7369  n :: 3.11.Classi
+000003f0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00000400: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00000410: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00000420: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
+00000430: 7465 726e 6574 203a 3a20 5757 572f 4854  ternet :: WWW/HT
+00000440: 5450 0a43 6c61 7373 6966 6965 723a 2054  TP.Classifier: T
+00000450: 6f70 6963 203a 3a20 496e 7465 726e 6574  opic :: Internet
+00000460: 203a 3a20 5757 572f 4854 5450 203a 3a20   :: WWW/HTTP :: 
+00000470: 4479 6e61 6d69 6320 436f 6e74 656e 740a  Dynamic Content.
+00000480: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+00000490: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
+000004a0: 2057 5757 2f48 5454 5020 3a3a 2057 5347   WWW/HTTP :: WSG
+000004b0: 4920 3a3a 2041 7070 6c69 6361 7469 6f6e  I :: Application
+000004c0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
+000004d0: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
+000004e0: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
+000004f0: 6272 6172 6965 7320 3a3a 2041 7070 6c69  braries :: Appli
+00000500: 6361 7469 6f6e 2046 7261 6d65 776f 726b  cation Framework
+00000510: 730a 436c 6173 7369 6669 6572 3a20 546f  s.Classifier: To
+00000520: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000530: 4465 7665 6c6f 706d 656e 7420 3a3a 204c  Development :: L
+00000540: 6962 7261 7269 6573 0a52 6571 7569 7265  ibraries.Require
+00000550: 732d 5079 7468 6f6e 3a20 3e3d 332e 380a  s-Python: >=3.8.
+00000560: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00000570: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00000580: 6172 6b64 6f77 6e0a 4c69 6365 6e73 652d  arkdown.License-
+00000590: 4669 6c65 3a20 4c49 4345 4e53 450a 5265  File: LICENSE.Re
+000005a0: 7175 6972 6573 2d44 6973 743a 2044 6a61  quires-Dist: Dja
+000005b0: 6e67 6f3e 3d33 2e32 0a50 726f 7669 6465  ngo>=3.2.Provide
+000005c0: 732d 4578 7472 613a 2074 6573 7469 6e67  s-Extra: testing
+000005d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000005e0: 636f 7665 7261 6765 3b20 6578 7472 6120  coverage; extra 
+000005f0: 3d3d 2022 7465 7374 696e 6722 0a52 6571  == "testing".Req
+00000600: 7569 7265 732d 4469 7374 3a20 636f 6465  uires-Dist: code
+00000610: 636f 763b 2065 7874 7261 203d 3d20 2274  cov; extra == "t
+00000620: 6573 7469 6e67 220a 5072 6f76 6964 6573  esting".Provides
+00000630: 2d45 7874 7261 3a20 6c69 6e74 696e 670a  -Extra: linting.
+00000640: 5265 7175 6972 6573 2d44 6973 743a 2066  Requires-Dist: f
+00000650: 6c61 6b65 383b 2065 7874 7261 203d 3d20  lake8; extra == 
+00000660: 226c 696e 7469 6e67 220a 5265 7175 6972  "linting".Requir
+00000670: 6573 2d44 6973 743a 2070 796c 696e 743b  es-Dist: pylint;
+00000680: 2065 7874 7261 203d 3d20 226c 696e 7469   extra == "linti
+00000690: 6e67 220a 0a23 2064 6a61 6e67 6f2d 6975  ng"..# django-iu
+000006a0: 6265 6e64 6120 5b21 5b50 7950 6920 6c69  benda [![PyPi li
+000006b0: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
+000006c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000006d0: 7069 2f6c 2f64 6a61 6e67 6f2d 6975 6265  pi/l/django-iube
+000006e0: 6e64 612e 7376 6729 5d28 6874 7470 733a  nda.svg)](https:
+000006f0: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000700: 672f 7079 7069 2f64 6a61 6e67 6f2d 6975  g/pypi/django-iu
+00000710: 6265 6e64 6129 0a0a 5b21 5b50 7950 6920  benda)..[![PyPi 
+00000720: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
+00000730: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000740: 7970 692f 7374 6174 7573 2f64 6a61 6e67  ypi/status/djang
+00000750: 6f2d 6975 6265 6e64 612e 7376 6729 5d28  o-iubenda.svg)](
+00000760: 6874 7470 733a 2f2f 7079 7069 2e70 7974  https://pypi.pyt
+00000770: 686f 6e2e 6f72 672f 7079 7069 2f64 6a61  hon.org/pypi/dja
+00000780: 6e67 6f2d 6975 6265 6e64 6129 0a5b 215b  ngo-iubenda).[![
+00000790: 5079 5069 2076 6572 7369 6f6e 5d28 6874  PyPi version](ht
+000007a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000007b0: 732e 696f 2f70 7970 692f 762f 646a 616e  s.io/pypi/v/djan
+000007c0: 676f 2d69 7562 656e 6461 2e73 7667 295d  go-iubenda.svg)]
+000007d0: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
+000007e0: 7468 6f6e 2e6f 7267 2f70 7970 692f 646a  thon.org/pypi/dj
+000007f0: 616e 676f 2d69 7562 656e 6461 290a 5b21  ango-iubenda).[!
+00000800: 5b50 7950 6920 7079 7468 6f6e 2076 6572  [PyPi python ver
+00000810: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
+00000820: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000830: 692f 7079 7665 7273 696f 6e73 2f64 6a61  i/pyversions/dja
+00000840: 6e67 6f2d 6975 6265 6e64 612e 7376 6729  ngo-iubenda.svg)
+00000850: 5d28 6874 7470 733a 2f2f 7079 7069 2e70  ](https://pypi.p
+00000860: 7974 686f 6e2e 6f72 672f 7079 7069 2f64  ython.org/pypi/d
+00000870: 6a61 6e67 6f2d 6975 6265 6e64 6129 0a5b  jango-iubenda).[
+00000880: 215b 5079 5069 2064 6f77 6e6c 6f61 6473  ![PyPi downloads
+00000890: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000008a0: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
+000008b0: 2f64 6a61 6e67 6f2d 6975 6265 6e64 612e  /django-iubenda.
+000008c0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
+000008d0: 7069 2e70 7974 686f 6e2e 6f72 672f 7079  pi.python.org/py
+000008e0: 7069 2f64 6a61 6e67 6f2d 6975 6265 6e64  pi/django-iubend
+000008f0: 6129 0a5b 215b 5079 5069 2064 6f77 6e6c  a).[![PyPi downl
+00000900: 6f61 6473 5d28 6874 7470 733a 2f2f 696d  oads](https://im
+00000910: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000920: 692f 6477 2f64 6a61 6e67 6f2d 6975 6265  i/dw/django-iube
+00000930: 6e64 612e 7376 6729 5d28 6874 7470 733a  nda.svg)](https:
+00000940: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
+00000950: 672f 7079 7069 2f64 6a61 6e67 6f2d 6975  g/pypi/django-iu
+00000960: 6265 6e64 6129 0a5b 215b 5079 5069 2064  benda).[![PyPi d
+00000970: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
+00000980: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000990: 2f70 7970 692f 6464 2f64 6a61 6e67 6f2d  /pypi/dd/django-
+000009a0: 6975 6265 6e64 612e 7376 6729 5d28 6874  iubenda.svg)](ht
+000009b0: 7470 733a 2f2f 7079 7069 2e70 7974 686f  tps://pypi.pytho
+000009c0: 6e2e 6f72 672f 7079 7069 2f64 6a61 6e67  n.org/pypi/djang
+000009d0: 6f2d 6975 6265 6e64 6129 0a0a 2323 2047  o-iubenda)..## G
+000009e0: 6974 4875 6220 215b 4769 7448 7562 2072  itHub ![GitHub r
+000009f0: 656c 6561 7365 5d28 6874 7470 733a 2f2f  elease](https://
+00000a00: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00000a10: 6974 6875 622f 7461 672f 444c 5253 502f  ithub/tag/DLRSP/
+00000a20: 646a 616e 676f 2d69 7562 656e 6461 2e73  django-iubenda.s
+00000a30: 7667 2920 215b 4769 7448 7562 2072 656c  vg) ![GitHub rel
+00000a40: 6561 7365 5d28 6874 7470 733a 2f2f 696d  ease](https://im
+00000a50: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000a60: 6875 622f 7265 6c65 6173 652f 444c 5253  hub/release/DLRS
+00000a70: 502f 646a 616e 676f 2d69 7562 656e 6461  P/django-iubenda
+00000a80: 2e73 7667 290a 0a23 2320 5465 7374 205b  .svg)..## Test [
+00000a90: 215b 636f 6465 636f 762e 696f 5d28 6874  ![codecov.io](ht
+00000aa0: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00000ab0: 2f67 6974 6875 622f 444c 5253 502f 646a  /github/DLRSP/dj
+00000ac0: 616e 676f 2d69 7562 656e 6461 2f63 6f76  ango-iubenda/cov
+00000ad0: 6572 6167 652e 7376 673f 6272 616e 6368  erage.svg?branch
+00000ae0: 3d6d 6169 6e29 5d28 6874 7470 733a 2f2f  =main)](https://
+00000af0: 636f 6465 636f 762e 696f 2f67 6974 6875  codecov.io/githu
+00000b00: 622f 444c 5253 502f 646a 616e 676f 2d69  b/DLRSP/django-i
+00000b10: 7562 656e 6461 3f62 7261 6e63 683d 6d61  ubenda?branch=ma
+00000b20: 696e 2920 5b21 5b70 7265 2d63 6f6d 6d69  in) [![pre-commi
+00000b30: 742e 6369 2073 7461 7475 735d 2868 7474  t.ci status](htt
+00000b40: 7073 3a2f 2f72 6573 756c 7473 2e70 7265  ps://results.pre
+00000b50: 2d63 6f6d 6d69 742e 6369 2f62 6164 6765  -commit.ci/badge
+00000b60: 2f67 6974 6875 622f 444c 5253 502f 646a  /github/DLRSP/dj
+00000b70: 616e 676f 2d69 7562 656e 6461 2f6d 6169  ango-iubenda/mai
+00000b80: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
+00000b90: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+00000ba0: 6974 2e63 692f 6c61 7465 7374 2f67 6974  it.ci/latest/git
+00000bb0: 6875 622f 444c 5253 502f 646a 616e 676f  hub/DLRSP/django
+00000bc0: 2d69 7562 656e 6461 2f6d 6169 6e29 205b  -iubenda/main) [
+00000bd0: 215b 6769 7474 6875 622e 636f 6d5d 2868  ![gitthub.com](h
+00000be0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000bf0: 6d2f 444c 5253 502f 646a 616e 676f 2d69  m/DLRSP/django-i
+00000c00: 7562 656e 6461 2f61 6374 696f 6e73 2f77  ubenda/actions/w
+00000c10: 6f72 6b66 6c6f 7773 2f63 692e 7961 6d6c  orkflows/ci.yaml
+00000c20: 2f62 6164 6765 2e73 7667 295d 2868 7474  /badge.svg)](htt
+00000c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000c40: 444c 5253 502f 646a 616e 676f 2d69 7562  DLRSP/django-iub
+00000c50: 656e 6461 2f61 6374 696f 6e73 2f77 6f72  enda/actions/wor
+00000c60: 6b66 6c6f 7773 2f63 692e 7961 6d6c 290a  kflows/ci.yaml).
+00000c70: 0a23 2320 436f 6d70 6c69 616e 6365 2066  .## Compliance f
+00000c80: 6f72 2077 6562 7369 7465 7320 616e 6420  or websites and 
+00000c90: 6170 7073 0a43 6c69 636b 205b 6865 7265  apps.Click [here
+00000ca0: 5d28 6874 7470 3a2f 2f69 7562 656e 6461  ](http://iubenda
+00000cb0: 2e72 6566 722e 6363 2f64 6c72 7370 6170  .refr.cc/dlrspap
+00000cc0: 6929 2061 6e64 2067 6574 2031 3025 2064  i) and get 10% d
+00000cd0: 6973 636f 756e 7420 6f6e 2066 6972 7374  iscount on first
+00000ce0: 2079 6561 7220 6174 2049 7562 656e 6461   year at Iubenda
+00000cf0: 0a5b 215b 4975 6265 6e64 615d 2868 7474  .[![Iubenda](htt
+00000d00: 7073 3a2f 2f63 6c69 656e 742d 6173 7365  ps://client-asse
+00000d10: 7473 2e72 6566 6572 7261 6c63 616e 6479  ts.referralcandy
+00000d20: 2e63 6f6d 2f6d 6436 5934 366a 4254 3575  .com/md6Y46jBT5u
+00000d30: 6654 434f 327a 7a47 745f 3136 3638 3539  fTCO2zzGt_166859
+00000d40: 3831 3836 2e70 6e67 295d 2868 7474 703a  8186.png)](http:
+00000d50: 2f2f 6975 6265 6e64 612e 7265 6672 2e63  //iubenda.refr.c
+00000d60: 632f 646c 7273 7061 7069 290a 0a0a 2323  c/dlrspapi)...##
+00000d70: 2043 6865 636b 2044 656d 6f20 5072 6f6a   Check Demo Proj
+00000d80: 6563 740a 2a20 4368 6563 6b20 7468 6520  ect.* Check the 
+00000d90: 6465 6d6f 2072 6570 6f20 6f6e 205b 4769  demo repo on [Gi
+00000da0: 7448 7562 5d28 6874 7470 733a 2f2f 6769  tHub](https://gi
+00000db0: 7468 7562 2e63 6f6d 2f44 4c52 5350 2f65  thub.com/DLRSP/e
+00000dc0: 7861 6d70 6c65 2f74 7265 652f 646a 616e  xample/tree/djan
+00000dd0: 676f 2d69 7562 656e 6461 290a 0a23 2320  go-iubenda)..## 
+00000de0: 5265 7175 6972 656d 656e 7473 0a2d 2020  Requirements.-  
+00000df0: 2050 7974 686f 6e20 2b33 2e38 2073 7570   Python +3.8 sup
+00000e00: 706f 7274 6564 2e0a 2d20 2020 446a 616e  ported..-   Djan
+00000e10: 676f 202b 332e 3220 7375 7070 6f72 7465  go +3.2 supporte
+00000e20: 642e 0a0a 2323 2053 6574 7570 0a31 2e20  d...## Setup.1. 
+00000e30: 496e 7374 616c 6c20 6672 6f6d 202a 2a70  Install from **p
+00000e40: 6970 2a2a 3a0a 2020 2060 6060 7368 656c  ip**:.   ```shel
+00000e50: 6c0a 2020 2070 6970 2069 6e73 7461 6c6c  l.   pip install
+00000e60: 2064 6a61 6e67 6f2d 6975 6265 6e64 610a   django-iubenda.
+00000e70: 2020 2060 6060 0a32 2e20 4d6f 6469 6679     ```.2. Modify
+00000e80: 2060 7365 7474 696e 6773 2e70 7960 2062   `settings.py` b
+00000e90: 7920 6164 6469 6e67 2074 6865 2061 7070  y adding the app
+00000ea0: 2074 6f20 6049 4e53 5441 4c4c 4544 5f41   to `INSTALLED_A
+00000eb0: 5050 5360 3a0a 2020 2060 6060 7079 7468  PPS`:.   ```pyth
+00000ec0: 6f6e 0a20 2020 494e 5354 414c 4c45 445f  on.   INSTALLED_
+00000ed0: 4150 5053 203d 2028 0a20 2020 2020 2020  APPS = (.       
+00000ee0: 226d 6f64 656c 7472 616e 736c 6174 696f  "modeltranslatio
+00000ef0: 6e22 2c0a 2020 2020 2020 2023 202e 2e2e  n",.       # ...
+00000f00: 0a20 2020 2020 2020 2269 7562 656e 6461  .       "iubenda
+00000f10: 222c 0a20 2020 2020 2020 2320 2e2e 2e0a  ",.       # ....
+00000f20: 2020 2029 0a20 2020 6060 600a 332e 204d     ).   ```.3. M
+00000f30: 6f64 6966 7920 6073 6574 7469 6e67 732e  odify `settings.
+00000f40: 7079 6020 6279 2061 6464 696e 6720 7468  py` by adding th
+00000f50: 6520 6170 7027 7320 636f 6e74 6578 7420  e app's context 
+00000f60: 7072 6f63 6573 736f 7220 746f 2060 5445  processor to `TE
+00000f70: 4d50 4c41 5445 5360 3a0a 2020 2060 6060  MPLATES`:.   ```
+00000f80: 7079 7468 6f6e 0a20 2020 5445 4d50 4c41  python.   TEMPLA
+00000f90: 5445 5320 3d20 5b0a 2020 2020 2020 207b  TES = [.       {
+00000fa0: 0a20 2020 2020 2020 2020 2020 2320 2e2e  .           # ..
+00000fb0: 2e0a 2020 2020 2020 2020 2020 2022 4f50  ..           "OP
+00000fc0: 5449 4f4e 5322 3a20 7b0a 2020 2020 2020  TIONS": {.      
+00000fd0: 2020 2020 2020 2020 2022 636f 6e74 6578           "contex
+00000fe0: 745f 7072 6f63 6573 736f 7273 223a 205b  t_processors": [
+00000ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001000: 2020 2020 2320 2e2e 2e0a 2020 2020 2020      # ....      
+00001010: 2020 2020 2020 2020 2020 2020 2022 6975               "iu
+00001020: 6265 6e64 612e 636f 6e74 6578 745f 7072  benda.context_pr
+00001030: 6f63 6573 736f 7273 2e69 7562 656e 6461  ocessors.iubenda
+00001040: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001050: 2020 2020 2020 2320 2e2e 2e0a 2020 2020        # ....    
+00001060: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+00001070: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00001080: 2020 207d 2c0a 2020 205d 0a20 2020 6060     },.   ].   ``
+00001090: 600a 342e 2042 6520 7375 7265 2074 6865  `.4. Be sure the
+000010a0: 2044 6a61 6e67 6f27 7320 4c6f 6361 6c65   Django's Locale
+000010b0: 206d 6964 646c 6577 6172 6520 6973 2065   middleware is e
+000010c0: 6e61 626c 6564 2069 6e73 6964 6520 6073  nabled inside `s
+000010d0: 6574 7469 6e67 732e 7079 603a 0a20 2020  ettings.py`:.   
+000010e0: 6060 6070 7974 686f 6e0a 2020 204d 4944  ```python.   MID
+000010f0: 444c 4557 4152 4520 3d20 280a 2020 2020  DLEWARE = (.    
+00001100: 2020 2023 202e 2e2e 0a20 2020 2020 2020     # ....       
+00001110: 2264 6a61 6e67 6f2e 6d69 6464 6c65 7761  "django.middlewa
+00001120: 7265 2e6c 6f63 616c 652e 4c6f 6361 6c65  re.locale.Locale
+00001130: 4d69 6464 6c65 7761 7265 222c 0a20 2020  Middleware",.   
+00001140: 2020 2020 2320 2e2e 2e0a 2020 2029 0a20      # ....   ). 
+00001150: 2020 6060 600a 352e 204f 7074 696f 6e61    ```.5. Optiona
+00001160: 6c6c 792c 2062 7574 2073 7567 6775 6573  lly, but suggues
+00001170: 7465 642c 2074 6865 2044 6a61 6e67 6f27  ted, the Django'
+00001180: 7320 4375 7272 656e 7420 5369 7465 206d  s Current Site m
+00001190: 6964 646c 6577 6172 6520 6973 2065 6e61  iddleware is ena
+000011a0: 626c 6564 2069 6e73 6964 6520 6073 6574  bled inside `set
+000011b0: 7469 6e67 732e 7079 603a 0a20 2020 6060  tings.py`:.   ``
+000011c0: 6070 7974 686f 6e0a 2020 204d 4944 444c  `python.   MIDDL
+000011d0: 4557 4152 4520 3d20 280a 2020 2020 2020  EWARE = (.      
+000011e0: 2023 202e 2e2e 0a20 2020 2020 2020 2264   # ....       "d
+000011f0: 6a61 6e67 6f2e 636f 6e74 7269 622e 7369  jango.contrib.si
+00001200: 7465 732e 6d69 6464 6c65 7761 7265 2e43  tes.middleware.C
+00001210: 7572 7265 6e74 5369 7465 4d69 6464 6c65  urrentSiteMiddle
+00001220: 7761 7265 222c 0a20 2020 2020 2020 2320  ware",.       # 
+00001230: 2e2e 2e0a 2020 2029 0a20 2020 6060 600a  ....   ).   ```.
+00001240: 362e 204d 6f64 6966 7920 6075 726c 2e70  6. Modify `url.p
+00001250: 7960 2062 7920 6164 6469 6e67 2074 6865  y` by adding the
+00001260: 2061 7070 2773 2075 726c 7320 746f 2060   app's urls to `
+00001270: 7572 6c70 6174 7465 726e 7360 3a0a 2020  urlpatterns`:.  
+00001280: 2060 6060 7079 7468 6f6e 0a20 2020 7572   ```python.   ur
+00001290: 6c70 6174 7465 726e 7320 2b3d 205b 0a20  lpatterns += [. 
+000012a0: 2020 2020 2020 7061 7468 2822 222c 2069        path("", i
+000012b0: 6e63 6c75 6465 2822 6975 6265 6e64 612e  nclude("iubenda.
+000012c0: 7572 6c73 2229 292c 0a20 2020 5d0a 2020  urls")),.   ].  
+000012d0: 2060 6060 0a37 2e20 4d6f 6469 6679 2060   ```.7. Modify `
+000012e0: 7572 6c2e 7079 6020 6279 2061 6464 696e  url.py` by addin
+000012f0: 6720 7468 6520 6170 7027 7320 7369 7465  g the app's site
+00001300: 6d61 7073 2074 6f20 6073 6974 656d 6170  maps to `sitemap
+00001310: 7360 3a0a 2020 2060 6060 7079 7468 6f6e  s`:.   ```python
+00001320: 0a20 2020 6672 6f6d 2069 7562 656e 6461  .   from iubenda
+00001330: 2e73 6974 656d 6170 7320 696d 706f 7274  .sitemaps import
+00001340: 2050 7269 7661 6379 5369 7465 6d61 702c   PrivacySitemap,
+00001350: 2043 6f6f 6b69 6553 6974 656d 6170 0a0a   CookieSitemap..
+00001360: 2020 2073 6974 656d 6170 7320 3d20 7b0a     sitemaps = {.
+00001370: 2020 2020 2020 2023 202e 2e2e 0a20 2020         # ....   
+00001380: 2020 2020 2270 7269 7661 6379 223a 2050      "privacy": P
+00001390: 7269 7661 6379 5369 7465 6d61 702c 0a20  rivacySitemap,. 
+000013a0: 2020 2020 2020 2263 6f6f 6b69 6522 3a20        "cookie": 
+000013b0: 436f 6f6b 6965 5369 7465 6d61 702c 0a20  CookieSitemap,. 
+000013c0: 2020 2020 2020 2320 2e2e 2e0a 2020 207d        # ....   }
+000013d0: 0a20 2020 6060 600a 382e 2042 6520 7375  .   ```.8. Be su
+000013e0: 7265 2074 6865 2076 6172 6961 626c 6520  re the variable 
+000013f0: 604c 414e 4755 4147 455f 434f 4445 6020  `LANGUAGE_CODE` 
+00001400: 6973 2061 7661 696c 6162 6c65 2066 6f72  is available for
+00001410: 2048 544d 4c20 7465 6d70 6c61 7465 733a   HTML templates:
+00001420: 0a20 2020 6060 6068 746d 6c0a 2020 207b  .   ```html.   {
+00001430: 2520 6c6f 6164 2069 3138 6e20 257d 0a20  % load i18n %}. 
+00001440: 2020 7b25 2067 6574 5f63 7572 7265 6e74    {% get_current
+00001450: 5f6c 616e 6775 6167 6520 6173 204c 414e  _language as LAN
+00001460: 4755 4147 455f 434f 4445 2025 7d0a 2020  GUAGE_CODE %}.  
+00001470: 2060 6060 0a39 2e20 4d6f 6469 6679 2079   ```.9. Modify y
+00001480: 6f75 7220 7072 6f6a 6563 7427 7320 7465  our project's te
+00001490: 6d70 6c61 7465 2074 6f20 6164 6420 7072  mplate to add pr
+000014a0: 6976 6163 7920 616e 6420 636f 6f6b 6965  ivacy and cookie
+000014b0: 2070 6f6c 6963 6965 732e 0a20 2020 466f   policies..   Fo
+000014c0: 7220 6578 616d 706c 6520 696e 7369 6465  r example inside
+000014d0: 2074 6865 2060 666f 6f74 6572 2e68 746d   the `footer.htm
+000014e0: 6c60 2061 6464 2066 6f6c 6c6f 7769 6e67  l` add following
+000014f0: 2063 6f64 653a 0a20 2020 6060 6068 746d   code:.   ```htm
+00001500: 6c0a 2020 207b 2520 6966 206e 6f74 2064  l.   {% if not d
+00001510: 6562 7567 2025 7d0a 2020 2020 2020 207b  ebug %}.       {
+00001520: 2520 626c 6f63 6b20 6975 6265 6e64 6120  % block iubenda 
+00001530: 257d 7b25 2069 6e63 6c75 6465 2022 6975  %}{% include "iu
+00001540: 6265 6e64 612f 696e 636c 7564 652d 636f  benda/include-co
+00001550: 6e74 656e 742e 6874 6d6c 2220 257d 7b25  ntent.html" %}{%
+00001560: 2065 6e64 626c 6f63 6b20 6975 6265 6e64   endblock iubend
+00001570: 6120 257d 0a20 2020 7b25 2065 6e64 6966  a %}.   {% endif
+00001580: 2025 7d0a 2020 2060 6060 0a0a 2323 204f   %}.   ```..## O
+00001590: 7074 696f 6e61 6c0a 0a23 2323 2041 7574  ptional..### Aut
+000015a0: 6f62 6c6f 636b 696e 670a 4966 2049 7562  oblocking.If Iub
+000015b0: 656e 6461 2061 7574 6f62 6c6f 636b 696e  enda autoblockin
+000015c0: 6727 7320 636f 6e66 6967 7572 6174 696f  g's configuratio
+000015d0: 6e73 2061 7265 2069 6d70 6c65 6d65 6e74  ns are implement
+000015e0: 6564 2069 6e20 796f 7572 2061 6363 6f75  ed in your accou
+000015f0: 6e74 2c0a 7468 6520 7661 7269 6162 6c65  nt,.the variable
+00001600: 2060 4955 4245 4e44 415f 4155 544f 424c   `IUBENDA_AUTOBL
+00001610: 4f43 4b49 4e47 6020 6361 6e20 6265 2073  OCKING` can be s
+00001620: 6574 2074 6f20 696d 706f 7274 2074 6865  et to import the
+00001630: 2073 6974 6527 7320 7363 7269 7074 2e0a   site's script..
+00001640: 6060 6068 746d 6c0a 3c73 6372 6970 7420  ```html.<script 
+00001650: 7479 7065 3d22 7465 7874 2f6a 6176 6173  type="text/javas
+00001660: 6372 6970 7422 2073 7263 3d22 6874 7470  cript" src="http
+00001670: 733a 2f2f 6373 2e69 7562 656e 6461 2e63  s://cs.iubenda.c
+00001680: 6f6d 2f61 7574 6f62 6c6f 636b 696e 672f  om/autoblocking/
+00001690: 7b7b 2063 785f 6975 6265 6e64 612e 6975  {{ cx_iubenda.iu
+000016a0: 625f 7369 7465 5f69 6420 7d7d 2e6a 7322  b_site_id }}.js"
+000016b0: 3e3c 2f73 6372 6970 743e 0a60 6060 0a0a  ></script>.```..
+000016c0: 2323 2320 436f 6e74 656e 7420 5365 6375  ### Content Secu
+000016d0: 7269 7479 2050 6f6c 6963 790a 4966 2043  rity Policy.If C
+000016e0: 6f6e 7465 6e74 2053 6563 7572 6974 7920  ontent Security 
+000016f0: 506f 6c69 6379 2061 7265 2069 6d70 6c65  Policy are imple
+00001700: 6d65 6e74 6564 2069 6e20 796f 7572 2073  mented in your s
+00001710: 6572 7665 7220 616e 6420 696e 6c69 6e65  erver and inline
+00001720: 2073 6372 6970 7473 2061 7265 2064 6973   scripts are dis
+00001730: 6162 6c65 642c 0a74 6865 2076 6172 6961  abled,.the varia
+00001740: 626c 6520 6049 5542 454e 4441 5f43 5350  ble `IUBENDA_CSP
+00001750: 5f4e 4f4e 4345 6020 6361 6e20 6265 2073  _NONCE` can be s
+00001760: 6574 2077 6974 6820 6e6f 6e63 6520 7461  et with nonce ta
+00001770: 6720 7769 6c6c 2062 6520 696e 7365 7274  g will be insert
+00001780: 6564 2073 6372 6970 7427 7320 6e6f 6e63  ed script's nonc
+00001790: 652e 0a60 6060 6874 6d6c 0a3c 7363 7269  e..```html.<scri
+000017a0: 7074 2074 7970 653d 2274 6578 742f 6a61  pt type="text/ja
+000017b0: 7661 7363 7269 7074 2220 7b25 2069 6620  vascript" {% if 
+000017c0: 6378 5f69 7562 656e 6461 5f6e 6f6e 6365  cx_iubenda_nonce
+000017d0: 2025 7d6e 6f6e 6365 3d22 7b7b 2063 785f   %}nonce="{{ cx_
+000017e0: 6975 6265 6e64 615f 6e6f 6e63 6520 7d7d  iubenda_nonce }}
+000017f0: 227b 2520 656e 6469 6620 257d 3e0a 6060  "{% endif %}>.``
+00001800: 600a 496e 7369 6465 2079 6f75 7220 7765  `.Inside your we
+00001810: 6273 6572 7665 7227 7320 636f 6e66 6967  bserver's config
+00001820: 7572 6174 696f 6e73 2c20 6120 7275 6c65  urations, a rule
+00001830: 2074 6f20 6479 6e61 6d69 6361 6c6c 7920   to dynamically 
+00001840: 7265 706c 6163 6520 796f 7572 2043 4f4e  replace your CON
+00001850: 5354 414e 5420 6e6f 6e63 6520 696e 2061  STANT nonce in a
+00001860: 2072 616e 646f 6d20 7374 7269 6e67 2069   random string i
+00001870: 7320 6e65 6564 6564 2e0a 0a54 6f20 616c  s needed...To al
+00001880: 6c6f 7720 2065 7874 6572 6e61 6c20 736f  low  external so
+00001890: 7572 6365 2066 726f 6d20 4975 6265 6e64  urce from Iubend
+000018a0: 6120 646f 6d61 696e 732c 2070 6c65 6173  a domains, pleas
+000018b0: 6520 696d 706c 656d 656e 7420 7468 6573  e implement thes
+000018c0: 6520 7275 6c65 733a 0a60 6060 6564 6974  e rules:.```edit
+000018d0: 6f72 636f 6e66 6967 0a43 6f6e 7465 6e74  orconfig.Content
+000018e0: 2d53 6563 7572 6974 792d 506f 6c69 6379  -Security-Policy
+000018f0: 3a0a 2020 2020 7363 7269 7074 2d73 7263  :.    script-src
+00001900: 2d65 6c65 6d20 6874 7470 733a 2f2f 2a2e  -elem https://*.
+00001910: 6975 6265 6e64 612e 636f 6d22 3b0a 2020  iubenda.com";.  
+00001920: 2020 696d 672d 7372 6320 6874 7470 733a    img-src https:
+00001930: 2f2f 2a2e 6975 6265 6e64 612e 636f 6d20  //*.iubenda.com 
+00001940: 6461 7461 3a22 3b0a 2020 2020 7374 796c  data:";.    styl
+00001950: 652d 7372 6320 6874 7470 733a 2f2f 2a2e  e-src https://*.
+00001960: 6975 6265 6e64 612e 636f 6d22 3b0a 2020  iubenda.com";.  
+00001970: 2020 636f 6e6e 6563 742d 7372 6320 6874    connect-src ht
+00001980: 7470 733a 2f2f 2a2e 6975 6265 6e64 612e  tps://*.iubenda.
+00001990: 636f 6d22 3b0a 2020 2020 6672 616d 652d  com";.    frame-
+000019a0: 7372 6320 6874 7470 733a 2f2f 2a2e 6975  src https://*.iu
+000019b0: 6265 6e64 612e 636f 6d22 3b0a 6060 600a  benda.com";.```.
+000019c0: 0a49 6620 796f 7520 7072 6566 6572 2074  .If you prefer t
+000019d0: 6f20 6e6f 7420 616c 6c6f 7720 2a2a 2a75  o not allow ***u
+000019e0: 6e73 6166 652d 696e 6c69 6e65 2a2a 2a20  nsafe-inline*** 
+000019f0: 696e 7369 6465 2079 6f75 7220 4353 502c  inside your CSP,
+00001a00: 2070 6c65 6173 6520 616c 736f 2061 6464   please also add
+00001a10: 2074 6865 2074 776f 2073 7065 6369 6669   the two specifi
+00001a20: 6320 6861 7368 2066 6f72 2079 6f75 720a  c hash for your.
+00001a30: 7363 7269 7074 2070 726f 6d70 7465 6420  script prompted 
+00001a40: 6173 2065 7272 6f72 2069 6e20 4a61 7661  as error in Java
+00001a50: 7363 7269 7074 2043 6f6e 736f 6c65 2e0a  script Console..
+00001a60: 6060 6065 6469 746f 7263 6f6e 6669 670a  ```editorconfig.
+00001a70: 2320 4975 6265 6e64 6120 5072 6976 6163  # Iubenda Privac
+00001a80: 7920 416e 6420 436f 6f6b 6965 2050 6f6c  y And Cookie Pol
+00001a90: 6963 7920 2d20 4150 490a 436f 6e74 656e  icy - API.Conten
+00001aa0: 742d 5365 6375 7269 7479 2d50 6f6c 6963  t-Security-Polic
+00001ab0: 793a 0a20 2020 202e 2e2e 0a20 2020 2073  y:.    ....    s
+00001ac0: 6372 6970 742d 7372 632d 656c 656d 2068  cript-src-elem h
+00001ad0: 7474 7073 3a2f 2f2a 2e69 7562 656e 6461  ttps://*.iubenda
+00001ae0: 2e63 6f6d 2027 7368 6132 3536 2d59 4f55  .com 'sha256-YOU
+00001af0: 522d 4649 5253 542d 4841 5348 2d50 524f  R-FIRST-HASH-PRO
+00001b00: 4d50 5445 442d 494e 5349 4445 2d43 4f4e  MPTED-INSIDE-CON
+00001b10: 534f 4c45 2720 2773 6861 3235 362d 594f  SOLE' 'sha256-YO
+00001b20: 5552 2d53 4543 4f4e 442d 4841 5348 2d50  UR-SECOND-HASH-P
+00001b30: 524f 4d50 5445 442d 494e 5349 4445 2d43  ROMPTED-INSIDE-C
+00001b40: 4f4e 534f 4c45 273b 0a20 2020 202e 2e2e  ONSOLE';.    ...
+00001b50: 0a60 6060 0a0a 4368 6563 6b20 7468 6973  .```..Check this
+00001b60: 2061 7274 6963 6c65 2066 726f 6d20 5b49   article from [I
+00001b70: 7562 656e 6461 2068 656c 705d 2868 7474  ubenda help](htt
+00001b80: 7073 3a2f 2f77 7777 2e69 7562 656e 6461  ps://www.iubenda
+00001b90: 2e63 6f6d 2f69 742f 6865 6c70 2f31 3233  .com/it/help/123
+00001ba0: 3437 2d63 6f6d 652d 636f 6e66 6967 7572  47-come-configur
+00001bb0: 6172 652d 696c 2d63 6f6e 7465 6e74 2d73  are-il-content-s
+00001bc0: 6563 7572 6974 792d 706f 6c69 6379 2d70  ecurity-policy-p
+00001bd0: 6572 2d63 6f6e 7365 6e74 6972 652d 6c65  er-consentire-le
+00001be0: 7365 6375 7a69 6f6e 652d 6465 676c 692d  secuzione-degli-
+00001bf0: 7363 7269 7074 2d64 692d 6975 6265 6e64  script-di-iubend
+00001c00: 6129 0a0a 2323 2320 4975 6265 6e64 6127  a)..### Iubenda'
+00001c10: 7320 4f70 7469 6f6e 730a 0a54 6f20 7065  s Options..To pe
+00001c20: 7273 6f6e 616c 697a 6520 7468 6520 4975  rsonalize the Iu
+00001c30: 6265 6e64 6120 7363 7269 7074 2773 2062  benda script's b
+00001c40: 6568 6176 696f 7572 2c20 7468 6520 6469  ehaviour, the di
+00001c50: 6374 2060 4955 4245 4e44 415f 4f50 5449  ct `IUBENDA_OPTI
+00001c60: 4f4e 5360 2063 616e 2062 6520 636f 6e66  ONS` can be conf
+00001c70: 6967 7572 6564 2069 6e73 6964 6520 6073  igured inside `s
+00001c80: 6574 7469 6e67 732e 7079 600a 6060 6070  ettings.py`.```p
+00001c90: 7974 686f 6e0a 4955 4245 4e44 415f 4f50  ython.IUBENDA_OP
+00001ca0: 5449 4f4e 5320 3d20 7b0a 2020 2020 2263  TIONS = {.    "c
+00001cb0: 6f75 6e74 7279 4465 7465 6374 696f 6e22  ountryDetection"
+00001cc0: 3a20 2274 7275 6522 2c0a 2020 2020 2261  : "true",.    "a
+00001cd0: 736b 436f 6e73 656e 7441 7443 6f6f 6b69  skConsentAtCooki
+00001ce0: 6550 6f6c 6963 7955 7064 6174 6522 3a20  ePolicyUpdate": 
+00001cf0: 2274 7275 6522 2c0a 2020 2020 2265 6e61  "true",.    "ena
+00001d00: 626c 6546 6164 7022 3a20 2274 7275 6522  bleFadp": "true"
+00001d10: 2c0a 2020 2020 2265 6e61 626c 654c 6770  ,.    "enableLgp
+00001d20: 6422 3a20 2274 7275 6522 2c0a 2020 2020  d": "true",.    
+00001d30: 226c 6770 6441 7070 6c69 6573 476c 6f62  "lgpdAppliesGlob
+00001d40: 616c 6c79 223a 2022 7472 7565 222c 0a20  ally": "true",. 
+00001d50: 2020 2022 656e 6162 6c65 5573 7072 223a     "enableUspr":
+00001d60: 2022 7472 7565 222c 0a20 2020 2022 656e   "true",.    "en
+00001d70: 6162 6c65 4363 7061 223a 2022 7472 7565  ableCcpa": "true
+00001d80: 222c 0a20 2020 2022 6363 7061 4163 6b6e  ",.    "ccpaAckn
+00001d90: 6f77 6c65 6467 654f 6e44 6973 706c 6179  owledgeOnDisplay
+00001da0: 223a 2022 7472 7565 222c 0a20 2020 2022  ": "true",.    "
+00001db0: 6363 7061 4170 706c 6965 7322 3a20 2274  ccpaApplies": "t
+00001dc0: 7275 6522 2c0a 2020 2020 2263 6f6e 7365  rue",.    "conse
+00001dd0: 6e74 4f6e 436f 6e74 696e 7565 6442 726f  ntOnContinuedBro
+00001de0: 7773 696e 6722 3a20 2266 616c 7365 222c  wsing": "false",
+00001df0: 0a20 2020 2022 666c 6f61 7469 6e67 5072  .    "floatingPr
+00001e00: 6566 6572 656e 6365 7342 7574 746f 6e44  eferencesButtonD
+00001e10: 6973 706c 6179 223a 2022 626f 7474 6f6d  isplay": "bottom
+00001e20: 2d6c 6566 7422 2c0a 2020 2020 2269 6e76  -left",.    "inv
+00001e30: 616c 6964 6174 6543 6f6e 7365 6e74 5769  alidateConsentWi
+00001e40: 7468 6f75 744c 6f67 223a 2022 7472 7565  thoutLog": "true
+00001e50: 222c 0a20 2020 2022 7065 7250 7572 706f  ",.    "perPurpo
+00001e60: 7365 436f 6e73 656e 7422 3a20 2274 7275  seConsent": "tru
+00001e70: 6522 2c0a 2020 2020 2277 6869 7465 6c61  e",.    "whitela
+00001e80: 6265 6c22 3a20 2266 616c 7365 222c 0a20  bel": "false",. 
+00001e90: 2020 2022 6261 6e6e 6572 223a 207b 0a20     "banner": {. 
+00001ea0: 2020 2020 2020 2022 6163 6365 7074 4275         "acceptBu
+00001eb0: 7474 6f6e 4469 7370 6c61 7922 3a20 2274  ttonDisplay": "t
+00001ec0: 7275 6522 2c0a 2020 2020 2020 2020 2262  rue",.        "b
+00001ed0: 6163 6b67 726f 756e 644f 7665 726c 6179  ackgroundOverlay
+00001ee0: 223a 2022 7472 7565 222c 0a20 2020 2020  ": "true",.     
+00001ef0: 2020 2022 636c 6f73 6542 7574 746f 6e52     "closeButtonR
+00001f00: 656a 6563 7473 223a 2022 7472 7565 222c  ejects": "true",
+00001f10: 0a20 2020 2020 2020 2022 6375 7374 6f6d  .        "custom
+00001f20: 697a 6542 7574 746f 6e44 6973 706c 6179  izeButtonDisplay
+00001f30: 223a 2022 7472 7565 222c 0a20 2020 2020  ": "true",.     
+00001f40: 2020 2022 6578 706c 6963 6974 5769 7468     "explicitWith
+00001f50: 6472 6177 616c 223a 2022 7472 7565 222c  drawal": "true",
+00001f60: 0a20 2020 2020 2020 2022 666f 6e74 5369  .        "fontSi
+00001f70: 7a65 223a 2022 3134 7078 222c 0a20 2020  ze": "14px",.   
+00001f80: 2020 2020 2022 6c69 7374 5075 7270 6f73       "listPurpos
+00001f90: 6573 223a 2022 7472 7565 222c 0a20 2020  es": "true",.   
+00001fa0: 2020 2020 2022 706f 7369 7469 6f6e 223a       "position":
+00001fb0: 2022 666c 6f61 742d 6365 6e74 6572 222c   "float-center",
+00001fc0: 0a20 2020 2020 2020 2022 7265 6a65 6374  .        "reject
+00001fd0: 4275 7474 6f6e 4469 7370 6c61 7922 3a20  ButtonDisplay": 
+00001fe0: 2274 7275 6522 2c0a 2020 2020 2020 2020  "true",.        
+00001ff0: 2273 686f 7750 7572 706f 7365 7354 6f67  "showPurposesTog
+00002000: 676c 6573 223a 2022 7472 7565 220a 2020  gles": "true".  
+00002010: 2020 7d2c 0a7d 0a60 6060 0a0a 2323 2320    },.}.```..### 
+00002020: 496e 7465 6772 6174 696f 6e20 7769 7468  Integration with
+00002030: 2047 6f6f 676c 6520 5461 6720 4d61 6e61   Google Tag Mana
+00002040: 6765 720a 4966 2047 6f6f 676c 6520 5461  ger.If Google Ta
+00002050: 6720 4d61 6e61 6765 7220 6973 2069 6d70  g Manager is imp
+00002060: 6c65 6d65 6e74 6564 2069 6e20 796f 7572  lemented in your
+00002070: 2061 7070 6c69 6361 7469 6f6e 2061 6e64   application and
+00002080: 2061 6c6c 206e 6565 6465 6420 7365 7474   all needed sett
+00002090: 696e 6773 2077 6572 6520 636f 6e66 6967  ings were config
+000020a0: 7572 6564 2069 6e73 6964 6520 7468 6520  ured inside the 
+000020b0: 636f 6e74 6169 6e65 722c 0a74 6865 2076  container,.the v
+000020c0: 6172 6961 626c 6520 6049 5542 454e 4441  ariable `IUBENDA
+000020d0: 5f47 544d 6020 6361 6e20 6265 2073 6574  _GTM` can be set
+000020e0: 2077 6974 6820 7468 6520 7661 6c75 6520   with the value 
+000020f0: 6054 7275 6560 2061 6e64 2074 6865 2049  `True` and the I
+00002100: 7562 656e 6461 2773 2063 616c 6c62 6163  ubenda's callbac
+00002110: 6b20 7769 6c6c 2062 6520 696e 7365 7274  k will be insert
+00002120: 6564 2069 6e73 6964 6520 7468 6520 7363  ed inside the sc
+00002130: 7269 7074 2e0a 0a46 6f72 206e 6565 6465  ript...For neede
+00002140: 6420 636f 6e66 6967 7572 6174 696f 6e20  d configuration 
+00002150: 696e 7369 6465 2047 6f6f 676c 6520 5461  inside Google Ta
+00002160: 6720 4d61 6e61 6765 7220 636f 6e74 6169  g Manager contai
+00002170: 6e65 722c 2070 6c65 6173 6520 7265 6665  ner, please refe
+00002180: 7220 746f 2074 6865 7365 206e 6f74 6573  r to these notes
+00002190: 3a0a 2d20 5b47 6f6f 676c 6520 436f 6e73  :.- [Google Cons
+000021a0: 656e 7420 4d6f 6465 5d28 6874 7470 733a  ent Mode](https:
+000021b0: 2f2f 7777 772e 6975 6265 6e64 612e 636f  //www.iubenda.co
+000021c0: 6d2f 656e 2f68 656c 702f 3237 3133 372d  m/en/help/27137-
+000021d0: 676f 6f67 6c65 2d63 6f6e 7365 6e74 2d6d  google-consent-m
+000021e0: 6f64 6529 0a2d 205b 476f 6f67 6c65 2043  ode).- [Google C
+000021f0: 6f6e 7365 6e74 204d 6f64 6520 7365 7475  onsent Mode setu
+00002200: 7020 4754 4d20 7769 7468 2049 7562 656e  p GTM with Iuben
+00002210: 6461 5d28 6874 7470 733a 2f2f 7777 772e  da](https://www.
+00002220: 6975 6265 6e64 612e 636f 6d2f 656e 2f68  iubenda.com/en/h
+00002230: 656c 702f 3734 3139 382d 676f 6f67 6c65  elp/74198-google
+00002240: 2d63 6f6e 7365 6e74 2d6d 6f64 652d 7365  -consent-mode-se
+00002250: 742d 7570 2d67 6f6f 676c 652d 7461 672d  t-up-google-tag-
+00002260: 6d61 6e61 6765 722d 7769 7468 2d69 7562  manager-with-iub
+00002270: 656e 6461 290a 2d20 5b47 544d 2042 6c6f  enda).- [GTM Blo
+00002280: 636b 696e 6720 436f 6f6b 6965 735d 2868  cking Cookies](h
+00002290: 7474 7073 3a2f 2f77 7777 2e69 7562 656e  ttps://www.iuben
+000022a0: 6461 2e63 6f6d 2f65 6e2f 6865 6c70 2f31  da.com/en/help/1
+000022b0: 3233 352d 676f 6f67 6c65 2d74 6167 2d6d  235-google-tag-m
+000022c0: 616e 6167 6572 2d62 6c6f 636b 696e 672d  anager-blocking-
+000022d0: 636f 6f6b 6965 7329 0a0a 2323 2052 756e  cookies)..## Run
+000022e0: 2045 7861 6d70 6c65 2050 726f 6a65 6374   Example Project
+000022f0: 0a0a 6060 6073 6865 6c6c 0a67 6974 2063  ..```shell.git c
+00002300: 6c6f 6e65 202d 2d64 6570 7468 3d35 3020  lone --depth=50 
+00002310: 2d2d 6272 616e 6368 3d64 6a61 6e67 6f2d  --branch=django-
+00002320: 6975 6265 6e64 6120 6874 7470 733a 2f2f  iubenda https://
+00002330: 6769 7468 7562 2e63 6f6d 2f44 4c52 5350  github.com/DLRSP
+00002340: 2f65 7861 6d70 6c65 2e67 6974 2044 4c52  /example.git DLR
+00002350: 5350 2f65 7861 6d70 6c65 0a63 6420 444c  SP/example.cd DL
+00002360: 5253 502f 6578 616d 706c 650a 7079 7468  RSP/example.pyth
+00002370: 6f6e 206d 616e 6167 652e 7079 2072 756e  on manage.py run
+00002380: 7365 7276 6572 0a60 6060 0a0a 4e6f 7720  server.```..Now 
+00002390: 6272 6f77 7365 7220 7468 6520 6170 7020  browser the app 
+000023a0: 4020 6874 7470 3a2f 2f31 3237 2e30 2e30  @ http://127.0.0
+000023b0: 2e31 3a38 3030 300a                      .1:8000.
```

### Comparing `django-iubenda-1.4.1/mkdocs.yml` & `django-iubenda-1.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/pyproject.toml` & `django-iubenda-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   { name = "Vendored Libraries",        directory = "vendor",  showcontent = true },
   { name = "Improved Documentation",    directory = "doc",     showcontent = true },
   { name = "Trivial Changes",           directory = "trivial", showcontent = false },
 ]
 
 # bump-my-version
 [tool.bumpversion]
-current_version = "1.4.1"
+current_version = "1.5.0"
 allow_dirty = true
 
 [[tool.bumpversion.files]]
 filename = "./setup.cfg"
 
 [[tool.bumpversion.files]]
 filename = "./src/iubenda/__init__.py"
```

### Comparing `django-iubenda-1.4.1/requirements/docs.txt` & `django-iubenda-1.5.0/requirements/docs.txt`

 * *Files 2% similar despite different names*

```diff
@@ -216,17 +216,17 @@
     # via
     #   -r requirements/docs.in
     #   mkdocs-git-revision-date-plugin
     #   mkdocs-material
 mkdocs-git-revision-date-plugin==0.3.2 \
     --hash=sha256:2e67956cb01823dd2418e2833f3623dee8604cdf223bddd005fe36226a56f6ef
     # via -r requirements/docs.in
-mkdocs-material==9.5.15 \
-    --hash=sha256:39f03cca45e82bf54eb7456b5a18bd252eabfdd67f237a229471484a0a4d4635 \
-    --hash=sha256:e5c96dec3d19491de49ca643fc1dbb92b278e43cdb816c775bc47db77d9b62fb
+mkdocs-material==9.5.17 \
+    --hash=sha256:06ae1275a72db1989cf6209de9e9ecdfbcfdbc24c58353877b2bb927dbe413e4 \
+    --hash=sha256:14a2a60119a785e70e765dd033e6211367aca9fc70230e577c1cf6a326949571
     # via -r requirements/docs.in
 mkdocs-material-extensions==1.3.1 \
     --hash=sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443 \
     --hash=sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31
     # via mkdocs-material
 packaging==24.0 \
     --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
```

### Comparing `django-iubenda-1.4.1/requirements/py310-dev.txt` & `django-iubenda-1.5.0/requirements/py310-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/requirements/py310-django32.txt` & `django-iubenda-1.5.0/requirements/py310-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,17 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py310-django42.txt` & `django-iubenda-1.5.0/requirements/py310-django42.txt`

 * *Files 2% similar despite different names*

```diff
@@ -181,17 +181,17 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py311-dev.txt` & `django-iubenda-1.5.0/requirements/py311-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/requirements/py311-django32.txt` & `django-iubenda-1.5.0/requirements/py311-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py311-django42.txt` & `django-iubenda-1.5.0/requirements/py311-django42.txt`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py38-dev.txt` & `django-iubenda-1.5.0/requirements/py38-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/requirements/py38-django32.txt` & `django-iubenda-1.5.0/requirements/py38-django32.txt`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,17 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py38-django42.txt` & `django-iubenda-1.5.0/requirements/py38-django42.txt`

 * *Files 1% similar despite different names*

```diff
@@ -199,17 +199,17 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py39-dev.txt` & `django-iubenda-1.5.0/requirements/py39-dev.txt`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/requirements/py39-django32.txt` & `django-iubenda-1.5.0/requirements/py39-django32.txt`

 * *Files 3% similar despite different names*

```diff
@@ -185,17 +185,17 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/requirements/py39-django42.txt` & `django-iubenda-1.5.0/requirements/py39-django42.txt`

 * *Files 3% similar despite different names*

```diff
@@ -181,17 +181,17 @@
     --hash=sha256:f0895b360dccf7e2d6af8762a52985e3fbaa56778de1bf6b20dbc96134253807 \
     --hash=sha256:f7cd33602ec0f393a0058e883284496bb4dbbdd34e0bbe23b594c8933ddf9b65
     # via django-compressor
 sqlparse==0.4.4 \
     --hash=sha256:5430a4fe2ac7d0f93e66f1efc6e1338a41884b7ddf2a350cedd20ccc4d9d28f3 \
     --hash=sha256:d446183e84b8349fa3061f0fe7f06ca94ba65b426946ffebe6e3e8295332420c
     # via django
-typing-extensions==4.10.0 \
-    --hash=sha256:69b1a937c3a517342112fb4c6df7e72fc39a38e7891a5730ed4985b5214b5475 \
-    --hash=sha256:b0abd7c89e8fb96f98db18d86106ff1d90ab692004eb746cf6eda2682f91b3cb
+typing-extensions==4.11.0 \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
     # via
     #   asgiref
     #   django-modeltranslation
 urllib3==2.2.1 \
     --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
     --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
     # via requests
```

### Comparing `django-iubenda-1.4.1/runtests.py` & `django-iubenda-1.5.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/setup.cfg` & `django-iubenda-1.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-iubenda
-version = 1.4.1
+version = 1.5.0
 url = https://github.com/DLRSP/django-iubenda
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django''s application for handling privacy and cookie policies configured with Iubenda.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-iubenda-1.4.1/setup.py` & `django-iubenda-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/django_iubenda.egg-info/PKG-INFO` & `django-iubenda-1.5.0/src/django_iubenda.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-iubenda
-Version: 1.4.1
+Version: 1.5.0
 Summary: Django''s application for handling privacy and cookie policies configured with Iubenda.
 Home-page: https://github.com/DLRSP/django-iubenda
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,iubenda,privacy,cookie
 Classifier: Development Status :: 4 - Beta
@@ -114,15 +114,15 @@
    urlpatterns += [
        path("", include("iubenda.urls")),
    ]
    ```
 7. Modify `url.py` by adding the app's sitemaps to `sitemaps`:
    ```python
    from iubenda.sitemaps import PrivacySitemap, CookieSitemap
-   
+
    sitemaps = {
        # ...
        "privacy": PrivacySitemap,
        "cookie": CookieSitemap,
        # ...
    }
    ```
@@ -137,14 +137,21 @@
    {% if not debug %}
        {% block iubenda %}{% include "iubenda/include-content.html" %}{% endblock iubenda %}
    {% endif %}
    ```
 
 ## Optional
 
+### Autoblocking
+If Iubenda autoblocking's configurations are implemented in your account,
+the variable `IUBENDA_AUTOBLOCKING` can be set to import the site's script.
+```html
+<script type="text/javascript" src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
+```
+
 ### Content Security Policy
 If Content Security Policy are implemented in your server and inline scripts are disabled,
 the variable `IUBENDA_CSP_NONCE` can be set with nonce tag will be inserted script's nonce.
 ```html
 <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
 ```
 Inside your webserver's configurations, a rule to dynamically replace your CONSTANT nonce in a random string is needed.
@@ -172,32 +179,39 @@
 Check this article from [Iubenda help](https://www.iubenda.com/it/help/12347-come-configurare-il-content-security-policy-per-consentire-lesecuzione-degli-script-di-iubenda)
 
 ### Iubenda's Options
 
 To personalize the Iubenda script's behaviour, the dict `IUBENDA_OPTIONS` can be configured inside `settings.py`
 ```python
 IUBENDA_OPTIONS = {
+    "countryDetection": "true",
+    "askConsentAtCookiePolicyUpdate": "true",
+    "enableFadp": "true",
+    "enableLgpd": "true",
+    "lgpdAppliesGlobally": "true",
+    "enableUspr": "true",
+    "enableCcpa": "true",
     "ccpaAcknowledgeOnDisplay": "true",
     "ccpaApplies": "true",
     "consentOnContinuedBrowsing": "false",
-    "enableCcpa": "true",
     "floatingPreferencesButtonDisplay": "bottom-left",
     "invalidateConsentWithoutLog": "true",
     "perPurposeConsent": "true",
     "whitelabel": "false",
     "banner": {
         "acceptButtonDisplay": "true",
         "backgroundOverlay": "true",
         "closeButtonRejects": "true",
         "customizeButtonDisplay": "true",
         "explicitWithdrawal": "true",
         "fontSize": "14px",
         "listPurposes": "true",
         "position": "float-center",
         "rejectButtonDisplay": "true",
+        "showPurposesToggles": "true"
     },
 }
 ```
 
 ### Integration with Google Tag Manager
 If Google Tag Manager is implemented in your application and all needed settings were configured inside the container,
 the variable `IUBENDA_GTM` can be set with the value `True` and the Iubenda's callback will be inserted inside the script.
```

### Comparing `django-iubenda-1.4.1/src/django_iubenda.egg-info/SOURCES.txt` & `django-iubenda-1.5.0/src/django_iubenda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,13 +51,16 @@
 src/iubenda/templates/iubenda/cookie.html
 src/iubenda/templates/iubenda/include-content.html
 src/iubenda/templates/iubenda/privacy-compress.html
 src/iubenda/templates/iubenda/privacy.html
 tests/__init__.py
 tests/settings.py
 tests/test_iubenda.py
+tests/test_iubenda_custom_options.py
+tests/test_iubenda_default_options.py
+tests/test_iubenda_settings.py
 tests/test_iubenda_template.py
 tests/test_iubenda_urls.py
 tests/urls.py
 tests/views.py
 tests/fixtures/data.json
 tests/templates/base.html
```

### Comparing `django-iubenda-1.4.1/src/iubenda/context_processors.py` & `django-iubenda-1.5.0/src/iubenda/context_processors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Context processors for Iubenda app
 """
 
+import logging
+
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.sites.shortcuts import get_current_site
 from django.core.cache import cache
 
 from .models import Iubenda
 
+logger = logging.getLogger(__name__)
+
 
 def iubenda(request):
     """Returns the info for:
     - iub_site_id: Iubenda Site ID
     - iub_policy_id: Iubenda Policy ID
     """
 
@@ -40,12 +44,16 @@
             if cx_iubenda_gtm:
                 context.update({"cx_iubenda_gtm": cx_iubenda_gtm})
 
             cx_iubenda_nonce = getattr(settings, "IUBENDA_CSP_NONCE", False)
             if cx_iubenda_nonce:
                 context.update({"cx_iubenda_nonce": cx_iubenda_nonce})
 
+            cx_iubenda_autoblocking = getattr(settings, "IUBENDA_AUTOBLOCKING", False)
+            if cx_iubenda_nonce:
+                context.update({"cx_iubenda_autoblocking": cx_iubenda_autoblocking})
+
             context_cache = cache.set(cache_key, context, timeout=86400)
             return context
         except Exception as err:
-            messages.error(request, err)
+            logger.error("iubenda: %s", err)
     return context_cache
```

### Comparing `django-iubenda-1.4.1/src/iubenda/locale/it/LC_MESSAGES/django.po` & `django-iubenda-1.5.0/src/iubenda/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/migrations/0001_initial.py` & `django-iubenda-1.5.0/src/iubenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/models.py` & `django-iubenda-1.5.0/src/iubenda/models.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/static/iubenda/css/iubenda_badge.css` & `django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_badge.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/static/iubenda/css/iubenda_policy.css` & `django-iubenda-1.5.0/src/iubenda/static/iubenda/css/iubenda_policy.css`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/templates/iubenda/cookie-compress.html` & `django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie-compress.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/templates/iubenda/cookie.html` & `django-iubenda-1.5.0/src/iubenda/templates/iubenda/cookie.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/templates/iubenda/include-content.html` & `django-iubenda-1.5.0/src/iubenda/templates/iubenda/include-content.html`

 * *Files 18% similar despite different names*

```diff
@@ -11,32 +11,39 @@
 <!-- JS Cookie Solution -->
 <script type="text/javascript" {% if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}>
     var _iub = _iub || [];
     _iub.csConfiguration = {
         "lang": "{{ LANGUAGE_CODE }}",
         "siteId": {{ cx_iubenda.iub_site_id }},
         "cookiePolicyId": {{ cx_iubenda.iub_policy_id }},
+        "countryDetection": {{ cx_iubenda_options.countryDetection|default:'true' }},
+        "askConsentAtCookiePolicyUpdate": {{ cx_iubenda_options.askConsentAtCookiePolicyUpdate|default:'true' }},
+        "enableFadp": {{ cx_iubenda_options.enableFadp|default:'true' }},
+        "enableLgpd": {{ cx_iubenda_options.enableLgpd|default:'true' }},
+        "lgpdAppliesGlobally": {{ cx_iubenda_options.lgpdAppliesGlobally|default:'false' }},
+        "enableUspr": {{ cx_iubenda_options.enableUspr|default:'true' }},
+        "enableCcpa": {{ cx_iubenda_options.enableCcpa|default:'true' }},
         "ccpaAcknowledgeOnDisplay": {{ cx_iubenda_options.ccpaAcknowledgeOnDisplay|default:'true' }},
         "ccpaApplies": {{ cx_iubenda_options.ccpaApplies|default:'true' }},
         "consentOnContinuedBrowsing": {{ cx_iubenda_options.consentOnContinuedBrowsing|default:'false' }},
-        "enableCcpa": {{ cx_iubenda_options.enableCcpa|default:'true' }},
         "floatingPreferencesButtonDisplay": "{{ cx_iubenda_options.floatingPreferencesButtonDisplay|default:'bottom-left' }}",
         "invalidateConsentWithoutLog": {{ cx_iubenda_options.invalidateConsentWithoutLog|default:'true' }},
         "perPurposeConsent": {{ cx_iubenda_options.perPurposeConsent|default:'true' }},
         "whitelabel": {{ cx_iubenda_options.whitelabel|default:'false' }},
         "banner": {
             "acceptButtonDisplay": {{ cx_iubenda_options.banner.acceptButtonDisplay|default:'true' }},
             "backgroundOverlay": {{ cx_iubenda_options.banner.backgroundOverlay|default:'true' }},
             "closeButtonRejects": {{ cx_iubenda_options.banner.closeButtonRejects|default:'true' }},
             "customizeButtonDisplay": {{ cx_iubenda_options.banner.customizeButtonDisplay|default:'true' }},
             "explicitWithdrawal": {{ cx_iubenda_options.banner.explicitWithdrawal|default:'true' }},
             "fontSize": "{{ cx_iubenda_options.banner.fontSize|default:'14px' }}",
             "listPurposes": {{ cx_iubenda_options.banner.listPurposes|default:'true' }},
             "position": "{{ cx_iubenda_options.banner.position|default:'float-center' }}",
-            "rejectButtonDisplay": {{ cx_iubenda_options.rejectButtonDisplay|default:'true' }}
+            "rejectButtonDisplay": {{ cx_iubenda_options.rejectButtonDisplay|default:'true' }},
+            "showPurposesToggles": {{ cx_iubenda_options.showPurposesToggles|default:'true' }}
         }{% if cx_iubenda_gtm %}
         ,"googleConsentMode": "{{ cx_iubenda_options.googleConsentMode|default:'template' }}",
         "callback": {
             onPreferenceExpressedOrNotNeeded: function(preference) {
                 dataLayer.push({
                     iubenda_ccpa_opted_out: _iub.cs.api.isCcpaOptedOut()
                 });
@@ -65,9 +72,12 @@
                 }
             }
         }{% endif %}
     };
 </script>
 
 <!-- JS Iubenda -->
+{% if cx_iubenda_autoblocking %}
+<script type="text/javascript" src="https://cs.iubenda.com/autoblocking/{{ cx_iubenda.iub_site_id }}.js"></script>
+{% endif %}
 <script type="text/javascript" src="https://cdn.iubenda.com/cs/ccpa/stub.js"></script>
 <script type="text/javascript" src="https://cdn.iubenda.com/cs/iubenda_cs.js" charset="UTF-8" async></script>
```

#### html2text {}

```diff
@@ -1,17 +1,23 @@
 _P_r_i_v_a_c_y_ _P_o_l_i_c_y - _C_o_o_k_i_e_ _P_o_l_i_c_y
 % if cx_iubenda_nonce %}nonce="{{ cx_iubenda_nonce }}"{% endif %}> var _iub =
 _iub || []; _iub.csConfiguration = { "lang": "{{ LANGUAGE_CODE }}", "siteId": {
 { cx_iubenda.iub_site_id }}, "cookiePolicyId": {{ cx_iubenda.iub_policy_id }},
-"ccpaAcknowledgeOnDisplay": {
-{ cx_iubenda_options.ccpaAcknowledgeOnDisplay|default:'true' }}, "ccpaApplies":
-{{ cx_iubenda_options.ccpaApplies|default:'true' }},
+"countryDetection": {{ cx_iubenda_options.countryDetection|default:'true' }},
+"askConsentAtCookiePolicyUpdate": {
+{ cx_iubenda_options.askConsentAtCookiePolicyUpdate|default:'true' }},
+"enableFadp": {{ cx_iubenda_options.enableFadp|default:'true' }}, "enableLgpd":
+{{ cx_iubenda_options.enableLgpd|default:'true' }}, "lgpdAppliesGlobally": {
+{ cx_iubenda_options.lgpdAppliesGlobally|default:'false' }}, "enableUspr": {
+{ cx_iubenda_options.enableUspr|default:'true' }}, "enableCcpa": {
+{ cx_iubenda_options.enableCcpa|default:'true' }}, "ccpaAcknowledgeOnDisplay":
+{{ cx_iubenda_options.ccpaAcknowledgeOnDisplay|default:'true' }},
+"ccpaApplies": {{ cx_iubenda_options.ccpaApplies|default:'true' }},
 "consentOnContinuedBrowsing": {
 { cx_iubenda_options.consentOnContinuedBrowsing|default:'false' }},
-"enableCcpa": {{ cx_iubenda_options.enableCcpa|default:'true' }},
 "floatingPreferencesButtonDisplay": "{
 { cx_iubenda_options.floatingPreferencesButtonDisplay|default:'bottom-left'
 }}", "invalidateConsentWithoutLog": {
 { cx_iubenda_options.invalidateConsentWithoutLog|default:'true' }},
 "perPurposeConsent": {{ cx_iubenda_options.perPurposeConsent|default:'true' }},
 "whitelabel": {{ cx_iubenda_options.whitelabel|default:'false' }}, "banner":
 { "acceptButtonDisplay": {
@@ -22,18 +28,22 @@
 "customizeButtonDisplay": {
 { cx_iubenda_options.banner.customizeButtonDisplay|default:'true' }},
 "explicitWithdrawal": {{ cx_iubenda_options.banner.explicitWithdrawal|default:
 'true' }}, "fontSize": "{{ cx_iubenda_options.banner.fontSize|default:'14px'
 }}", "listPurposes": {{ cx_iubenda_options.banner.listPurposes|default:'true'
 }}, "position": "{{ cx_iubenda_options.banner.position|default:'float-center'
 }}", "rejectButtonDisplay": {{ cx_iubenda_options.rejectButtonDisplay|default:
-'true' }} }{% if cx_iubenda_gtm %} ,"googleConsentMode": "{
+'true' }}, "showPurposesToggles": {
+{ cx_iubenda_options.showPurposesToggles|default:'true' }} }{% if
+cx_iubenda_gtm %} ,"googleConsentMode": "{
 { cx_iubenda_options.googleConsentMode|default:'template' }}", "callback":
 { onPreferenceExpressedOrNotNeeded: function(preference) { dataLayer.push(
 { iubenda_ccpa_opted_out: _iub.cs.api.isCcpaOptedOut() }); if (!preference)
 { dataLayer.push({ event: "iubenda_preference_not_needed" }); } else { if
 (preference.consent === true) { dataLayer.push({ event: "iubenda_consent_given"
 }); } else if (preference.consent === false) { dataLayer.push({ event:
 "iubenda_consent_rejected" }); } else if (preference.purposes) { for (var
 purposeId in preference.purposes) { if (preference.purposes[purposeId])
 { dataLayer.push({ event: "iubenda_consent_given_purpose_" + purposeId }); } }
 } } } }{% endif %} };
+{% if cx_iubenda_autoblocking %}
+{% endif %}
```

### Comparing `django-iubenda-1.4.1/src/iubenda/templates/iubenda/privacy-compress.html` & `django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy-compress.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/templates/iubenda/privacy.html` & `django-iubenda-1.5.0/src/iubenda/templates/iubenda/privacy.html`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/urls.py` & `django-iubenda-1.5.0/src/iubenda/urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/src/iubenda/views.py` & `django-iubenda-1.5.0/src/iubenda/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+"""
+Views for Iubenda app
+"""
+
 import json
+import logging
 
 import requests
 from django.conf import settings
-from django.contrib import messages
 from django.contrib.sites.models import Site
 from django.core.cache import cache
 from django.shortcuts import render
 from django.views.decorators.http import require_http_methods
 from django.views.decorators.vary import vary_on_headers
 
 from .models import Iubenda
 
+logger = logging.getLogger(__name__)
+
 
 @require_http_methods(["GET"])
 @vary_on_headers("User-Agent", "Cookie")
 def privacy(request):
     context = {}
     context_cache = {}
 
     cache_key = f"api_iubenda_privacy_{request.LANGUAGE_CODE}"
     try:
         context_cache = cache.get(cache_key)
     except Exception as err:
-        messages.warning(request, err)
+        logger.warning("iubenda: %s", err)
 
     if not context_cache or context_cache is None:
         try:
             iubenda = (
                 Iubenda.objects.filter(site=Site.objects.get_current())
                 .values("iub_policy_id")
                 .get()
@@ -38,15 +44,16 @@
             if r.status_code == 200:
                 context = {"req_privacy": json.loads(r.content)}
 
             cache.set(cache_key, context, timeout=86400)
             context_cache = cache.get(cache_key)
 
         except Exception as err:
-            messages.error(request, err)
+            logger.error("iubenda: %s", err)
+
     if getattr(settings, "IUBENDA_USE_COMPRESS", True):
         return render(request, "iubenda/privacy-compress.html", context_cache)
     return render(request, "iubenda/privacy.html", context_cache)
 
 
 @require_http_methods(["GET"])
 @vary_on_headers("User-Agent", "Cookie")
@@ -54,15 +61,15 @@
     context = {}
     context_cache = {}
 
     cache_key = f"api_iubenda_cookie_{request.LANGUAGE_CODE}"
     try:
         context_cache = cache.get(cache_key)
     except Exception as err:
-        messages.warning(request, err)
+        logger.warning("iubenda: %s", err)
 
     if not context_cache or context_cache is None:
         try:
             iubenda = (
                 Iubenda.objects.filter(site=Site.objects.get_current())
                 .values("iub_policy_id")
                 .get()
@@ -74,11 +81,11 @@
             if r.status_code == 200:
                 context = {"req_cookie": json.loads(r.content)}
 
             cache.set(cache_key, context, timeout=86400)
             context_cache = cache.get(cache_key)
 
         except Exception as err:
-            messages.error(request, err)
+            logger.error("iubenda: %s", err)
     if getattr(settings, "IUBENDA_USE_COMPRESS", True):
         return render(request, "iubenda/cookie-compress.html", context_cache)
     return render(request, "iubenda/cookie.html", context_cache)
```

### Comparing `django-iubenda-1.4.1/tests/settings.py` & `django-iubenda-1.5.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/tests/test_iubenda_template.py` & `django-iubenda-1.5.0/tests/test_iubenda_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 
     def tearDown(self):
         """Remove Test Data"""
         LOGGER.debug("Tests tearDown")
 
     def test_privacy_template_with_compress(self):
         """Test that render Privacy page using compress."""
-        LOGGER.debug("Render Privacy page")
+        LOGGER.debug("Render Compressed Privacy page")
         response = self.client.get("/privacy-policy/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(200, response.status_code)
         self.assertTemplateUsed(response, "iubenda/privacy-compress.html")
 
     def test_cookie_template_with_compress(self):
         """Test that render Cookie page using compress."""
-        LOGGER.debug("Render Cookie page")
+        LOGGER.debug("Render Compressed Cookie page")
         response = self.client.get("/cookie-policy/", follow=True)
         LOGGER.debug(response)
         self.assertEqual(200, response.status_code)
         self.assertTemplateUsed(response, "iubenda/cookie-compress.html")
 
     @override_settings(IUBENDA_USE_COMPRESS=False)
     def test_privacy_template(self):
```

### Comparing `django-iubenda-1.4.1/tests/test_iubenda_urls.py` & `django-iubenda-1.5.0/tests/test_iubenda_urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/tests/urls.py` & `django-iubenda-1.5.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-iubenda-1.4.1/tox.ini` & `django-iubenda-1.5.0/tox.ini`

 * *Files identical despite different names*

