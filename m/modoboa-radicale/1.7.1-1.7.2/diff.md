# Comparing `tmp/modoboa-radicale-1.7.1.tar.gz` & `tmp/modoboa-radicale-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modoboa-radicale-1.7.1.tar", last modified: Fri Feb 16 10:29:29 2024, max compression
+gzip compressed data, was "modoboa-radicale-1.7.2.tar", last modified: Tue Apr  9 08:26:47 2024, max compression
```

## Comparing `modoboa-radicale-1.7.1.tar` & `modoboa-radicale-1.7.2.tar`

### file list

```diff
@@ -1,195 +1,653 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.176837 modoboa-radicale-1.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.152837 modoboa-radicale-1.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.152837 modoboa-radicale-1.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/.github/workflows/plugin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.152837 modoboa-radicale-1.7.1/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-16 10:29:29.176837 modoboa-radicale-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/docs/setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/.browserslistrc
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/babel.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/br/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/en/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/es/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/fr/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/it/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/ro_RO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/ro_RO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/ro_RO/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/ru/LC_MESSAGES/app.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/locale/zh_TW/LC_MESSAGES/app.po
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.156837 modoboa-radicale-1.7.1/frontend/public/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/App.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/api.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/Calendar.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/CalendarAccessRulesForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/CalendarDetail.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/CalendarForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/CreateEventForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/EventForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/ImportEventsForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/components/Modal.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/main.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/src/router/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/router/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/src/store/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/store/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/src/store/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/store/modules/calendar.js
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/store/modules/event.js
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/store/mutation-types.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/src/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/tools/permissions.js
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/src/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.144837 modoboa-radicale-1.7.1/frontend/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.160837 modoboa-radicale-1.7.1/frontend/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/tests/unit/example.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/frontend/vue.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.164837 modoboa-radicale-1.7.1/modoboa_radicale/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.164837 modoboa-radicale-1.7.1/modoboa_radicale/backends/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/backends/caldav_.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/br/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/nl_NL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/ro_RO/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/ro_RO/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.168837 modoboa-radicale-1.7.1/modoboa_radicale/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.148837 modoboa-radicale-1.7.1/modoboa_radicale/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-16 10:29:26.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/management/commands/generate_rights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/migrations/0002_auto_20170831_1721.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/migrations/0003_auto_20180324_1834.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/migrations/0004_auto_20200220_1816.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/migrations/0005_auto_20200220_1819.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/modo_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.152837 modoboa-radicale-1.7.1/modoboa_radicale/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/templates/modoboa_radicale/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/templates/modoboa_radicale/calendar_display.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/test_data/events.ics
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/urls_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/modoboa_radicale/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-02-16 10:29:29.000000 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-02-16 10:29:29.000000 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 10:29:29.000000 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 10:29:29.000000 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-16 10:29:29.000000 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-16 10:29:29.000000 modoboa-radicale-1.7.1/modoboa_radicale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-16 10:29:29.176837 modoboa-radicale-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/test_project/
--rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test_project/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 10:29:29.172837 modoboa-radicale-1.7.1/test_project/test_project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test_project/test_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test_project/test_project/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test_project/test_project/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test_project/test_project/webpack-stats.json
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-16 10:28:57.000000 modoboa-radicale-1.7.1/test_project/test_project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/.github/workflows/plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/docs/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/.browserslistrc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/babel.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/br/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/en/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/es/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/fr/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/it/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/ro_RO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/ro_RO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/ro_RO/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/ru/LC_MESSAGES/app.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.058550 modoboa-radicale-1.7.2/frontend/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/locale/zh_TW/LC_MESSAGES/app.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/App.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/api.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/Calendar.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/CalendarAccessRulesForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/CalendarDetail.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/CalendarForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/CreateEventForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/EventForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/ImportEventsForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/components/Modal.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/main.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/src/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/router/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/src/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/store/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/src/store/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/store/modules/calendar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/store/modules/event.js
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/store/mutation-types.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/src/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/tools/permissions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/src/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/frontend/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.062550 modoboa-radicale-1.7.2/frontend/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/tests/unit/example.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/frontend/vue.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.066550 modoboa-radicale-1.7.2/modoboa_radicale/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.066550 modoboa-radicale-1.7.2/modoboa_radicale/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/backends/caldav_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/modoboa_radicale/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.066550 modoboa-radicale-1.7.2/modoboa_radicale/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/br/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/modoboa_radicale/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.066550 modoboa-radicale-1.7.2/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/modoboa_radicale/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.066550 modoboa-radicale-1.7.2/modoboa_radicale/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/modoboa_radicale/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.050550 modoboa-radicale-1.7.2/modoboa_radicale/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/nl_NL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/ro_RO/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/ro_RO/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-09 08:26:44.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.070550 modoboa-radicale-1.7.2/modoboa_radicale/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/management/commands/generate_rights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.074550 modoboa-radicale-1.7.2/modoboa_radicale/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/migrations/0002_auto_20170831_1721.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/migrations/0003_auto_20180324_1834.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/migrations/0004_auto_20200220_1816.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/migrations/0005_auto_20200220_1819.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/modo_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.074550 modoboa-radicale-1.7.2/modoboa_radicale/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19590 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.074550 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.074550 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/css/app.0eea5313.css
+-rw-r--r--   0 runner    (1001) docker     (127)    56280 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/css/chunk-vendors.d61f3f7b.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.146550 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    56520 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/app.fb41e528.js
+-rw-r--r--   0 runner    (1001) docker     (127)   165192 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/app.fb41e528.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a34bd.2628118b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a34bd.2628118b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a34e9.9993b39f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a34e9.9993b39f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a370a.bbeaf256.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a370a.bbeaf256.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a3756.1b1dfeef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a3756.1b1dfeef.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a3839.33311de0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a3839.33311de0.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a38b9.2a434d88.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a38b9.2a434d88.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a3a89.d4f1af28.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a3a89.d4f1af28.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a4056.52628a5f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a4056.52628a5f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a4b53.e179c223.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0a4b53.e179c223.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aa178.f9cbdd2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aa178.f9cbdd2f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aa5ef.c26a461d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aa5ef.c26a461d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aaf78.79faf48b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aaf78.79faf48b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ab68b.90ce37b8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ab68b.90ce37b8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ab6c4.63a0aed6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ab6c4.63a0aed6.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ab6f5.0a6978b9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ab6f5.0a6978b9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0abc94.233ddcb2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0abc94.233ddcb2.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ac20b.ea3b6dde.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ac20b.ea3b6dde.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ac5cb.68bac91e.js
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ac5cb.68bac91e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ac96c.039eb97c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ac96c.039eb97c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aec9e.33ccd7b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aec9e.33ccd7b7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aecae.d0f91bf2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aecae.d0f91bf2.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aed68.ed2f300c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0aed68.ed2f300c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0af42a.913b9775.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0af42a.913b9775.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0af467.4d7652fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0af467.4d7652fd.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0af8a4.56dae351.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0af8a4.56dae351.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0afa0e.8cfa1c98.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0afa0e.8cfa1c98.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0afa88.b6b56262.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0afa88.b6b56262.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b16b4.f43a264a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b16b4.f43a264a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b1df4.3c459438.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b1df4.3c459438.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b1e62.ed85c2ce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b1e62.ed85c2ce.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b2119.43862396.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b2119.43862396.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b2346.5d99b3c4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b2346.5d99b3c4.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b255b.1f099761.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b255b.1f099761.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b2758.ccb3af13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b2758.ccb3af13.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b28df.4a5de19e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b28df.4a5de19e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b28e9.d8c3c26b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b28e9.d8c3c26b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b306e.2017dfb5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b306e.2017dfb5.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b324c.fe18d977.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b324c.fe18d977.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b32bc.79e25796.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b32bc.79e25796.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b384e.1025431f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b384e.1025431f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b3e07.7508f090.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b3e07.7508f090.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b5fc8.2dfaa5b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b5fc8.2dfaa5b7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b66f7.6dbf9393.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b66f7.6dbf9393.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b8a58.738aabc9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b8a58.738aabc9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b8b22.401dd832.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b8b22.401dd832.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b92a3.90a41767.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b92a3.90a41767.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b991c.12fa7ea8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b991c.12fa7ea8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b9f58.d9bfbcaf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0b9f58.d9bfbcaf.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ba0d8.6eb5ae9d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ba0d8.6eb5ae9d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ba6cd.132075fb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ba6cd.132075fb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0bdb93.f49359c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0bdb93.f49359c6.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0bdf0b.8117060f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0bdf0b.8117060f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0bdf1c.c3441ccd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0bdf1c.c3441ccd.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0303.7189c4d4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0303.7189c4d4.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c04d4.c5b31bd8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c04d4.c5b31bd8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0614.98ea3729.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0614.98ea3729.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0665.eb9f9507.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0665.eb9f9507.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0ab4.cb579544.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0ab4.cb579544.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0e57.8f0341f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c0e57.8f0341f9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c1749.23ed4908.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c1749.23ed4908.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c18df.c6c05155.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c18df.c6c05155.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c1cfa.9420681c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c1cfa.9420681c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c2137.f9986c70.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c2137.f9986c70.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4244.9f4a40dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4244.9f4a40dc.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4255.5a06e5a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4255.5a06e5a1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c42c4.d624cff7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c42c4.d624cff7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c42fd.26c3ebaf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c42fd.26c3ebaf.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c49a7.b3472f2d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c49a7.b3472f2d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4a06.406ddd61.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4a06.406ddd61.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4c45.8901ba27.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4c45.8901ba27.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4fa7.58ce19fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4fa7.58ce19fd.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4fd5.add327e0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4fd5.add327e0.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4fd8.28c21dd4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c4fd8.28c21dd4.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c5579.0dc559bc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c5579.0dc559bc.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c78c6.4d7b64a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c78c6.4d7b64a6.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c792f.5d0a6516.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c792f.5d0a6516.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c7cc5.789b094b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c7cc5.789b094b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c7cf3.be6247d8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c7cf3.be6247d8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c8256.f7741c6a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c8256.f7741c6a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c87ca.ccb3b944.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c87ca.ccb3b944.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c8a71.28f83cb1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c8a71.28f83cb1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c8d7e.3dbb4a3f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c8d7e.3dbb4a3f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c91c4.897ade79.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c91c4.897ade79.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c932c.51ff62dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c932c.51ff62dd.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c9589.bd57b971.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0c9589.bd57b971.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cb6c7.15cd28ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cb6c7.15cd28ee.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cc477.0b74a51c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cc477.0b74a51c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cc668.d1ba2f52.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cc668.d1ba2f52.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ced71.70c4a8d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ced71.70c4a8d0.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cf667.dc10a6da.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cf667.dc10a6da.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cf866.4613f4bf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cf866.4613f4bf.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfa5b.c3fb9baf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfa5b.c3fb9baf.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfaa5.b555ef44.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfaa5.b555ef44.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfac5.71f3801c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfac5.71f3801c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfaf6.8e087c14.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfaf6.8e087c14.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfaff.cb9d62bb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfaff.cb9d62bb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfe68.143ffeca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0cfe68.143ffeca.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d2fce.42d4161e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d2fce.42d4161e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d3299.81fd2779.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d3299.81fd2779.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d3307.dd7e1968.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d3307.dd7e1968.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d34e2.90aef66f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d34e2.90aef66f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d622d.c19d0e6a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d622d.c19d0e6a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d63c2.9c7f9ee6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d63c2.9c7f9ee6.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d641c.fa147524.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d641c.fa147524.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d65b1.b1e3279e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d65b1.b1e3279e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d6922.90e51d45.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d6922.90e51d45.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d7882.cf5c1828.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d7882.cf5c1828.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d7aa2.91412459.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d7aa2.91412459.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d7c47.94ce7409.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0d7c47.94ce7409.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0da019.6ea430af.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0da019.6ea430af.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0da953.d21234d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0da953.d21234d0.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dab13.7984958e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dab13.7984958e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dace2.629d8629.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dace2.629d8629.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0db8a3.3ac0c0df.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0db8a3.3ac0c0df.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dd10d.a3734a45.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dd10d.a3734a45.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dd3d3.f44a765f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dd3d3.f44a765f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dd623.8fd1247f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0dd623.8fd1247f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ddc12.b42b7ea7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ddc12.b42b7ea7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ddfa4.151e88ba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ddfa4.151e88ba.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0de2b8.05e67fd8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0de2b8.05e67fd8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0de2f2.9eb1877a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0de2f2.9eb1877a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0de3cd.3cbb3d0e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0de3cd.3cbb3d0e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0df06b.afcb70fe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0df06b.afcb70fe.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0df0c0.90220854.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0df0c0.90220854.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e1f93.0c63608b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e1f93.0c63608b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e290e.4137bbf4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e290e.4137bbf4.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e2c86.f15c5b55.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e2c86.f15c5b55.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e44ef.8279bed9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e44ef.8279bed9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e502b.df8d2879.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e502b.df8d2879.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e5230.34a6e027.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e5230.34a6e027.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e528a.dbd4d00d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e528a.dbd4d00d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e675f.85eb0f2a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e675f.85eb0f2a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e68a5.f28ef4ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e68a5.f28ef4ca.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e6cd5.2cdd3032.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e6cd5.2cdd3032.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e88af.c12ccf53.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e88af.c12ccf53.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e8fe5.d723b587.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e8fe5.d723b587.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e9367.48e8ed96.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0e9367.48e8ed96.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ea117.892010b6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0ea117.892010b6.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f04bb.d395e73c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f04bb.d395e73c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f050c.5a487b7e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f050c.5a487b7e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f064b.af108237.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f064b.af108237.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f0654.4242baf2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f0654.4242baf2.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f15bf.bab4bf17.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d0f15bf.bab4bf17.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d207328.6f0ebf77.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d207328.6f0ebf77.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d207d87.6930ccf9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d207d87.6930ccf9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d207f0b.87417590.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d207f0b.87417590.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d208e1c.44d2ed6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d208e1c.44d2ed6e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d209617.528d97d7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d209617.528d97d7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20f909.5e1463db.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20f909.5e1463db.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fa70.94dfe94d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fa70.94dfe94d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fa99.4f5e5f1c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fa99.4f5e5f1c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fb2b.efcaf3c9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fb2b.efcaf3c9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fb61.fa3a1aca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20fb61.fa3a1aca.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20ff21.cd60c17d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d20ff21.cd60c17d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2101ea.e00f2199.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2101ea.e00f2199.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d210259.9ad07522.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d210259.9ad07522.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21049c.7f594989.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21049c.7f594989.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d210669.fa43ccf9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d210669.fa43ccf9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d210feb.3039ace7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d210feb.3039ace7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2131a1.8d0879ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2131a1.8d0879ee.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d213ad4.631395b6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d213ad4.631395b6.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d213c88.915d39d7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d213c88.915d39d7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d215ca3.4e5a6c91.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d215ca3.4e5a6c91.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d216442.51eace81.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d216442.51eace81.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d216446.6fd022d4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d216446.6fd022d4.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21648f.a9a54d03.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21648f.a9a54d03.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2165f9.255ba923.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2165f9.255ba923.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d216d3b.93bab4f0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d216d3b.93bab4f0.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21769d.09e0781d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21769d.09e0781d.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d217860.2ba2c2d8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d217860.2ba2c2d8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d217a1d.7d33da47.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d217a1d.7d33da47.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21a3aa.763c35b9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21a3aa.763c35b9.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21acef.ba63ca43.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21acef.ba63ca43.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21aec0.c9492eb3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21aec0.c9492eb3.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21d12f.7e5ffc41.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21d12f.7e5ffc41.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21d4c1.df794199.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21d4c1.df794199.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21d873.50e1cc6f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21d873.50e1cc6f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21de06.889ed8e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21de06.889ed8e2.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21f0be.7817c0df.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d21f0be.7817c0df.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    47164 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d221e50.eb35c9d3.js
+-rw-r--r--   0 runner    (1001) docker     (127)   145114 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d221e50.eb35c9d3.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22252c.8afe0103.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22252c.8afe0103.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2227e1.094d418c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2227e1.094d418c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22290e.318ffc27.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22290e.318ffc27.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d222d37.e49681b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d222d37.e49681b7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22579a.f8afa6dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22579a.f8afa6dc.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225b2c.6ff299c7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225b2c.6ff299c7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225c72.33585116.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225c72.33585116.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225df8.32dbfd73.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225df8.32dbfd73.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225f65.3a8ab879.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d225f65.3a8ab879.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d226318.63e926e3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d226318.63e926e3.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d226585.27c15f6c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d226585.27c15f6c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2266cb.5c0372ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2266cb.5c0372ed.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2288d7.2265048a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2288d7.2265048a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d228922.9599b4f5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d228922.9599b4f5.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d228cd2.5b80dfe8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d228cd2.5b80dfe8.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229007.d1c06f15.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229007.d1c06f15.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2290fe.3344800f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2290fe.3344800f.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229b4b.f339d510.js
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229b4b.f339d510.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229b94.5a078c43.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229b94.5a078c43.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229da7.83faf5af.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d229da7.83faf5af.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22b985.2ab5a9c1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22b985.2ab5a9c1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22c868.a029e027.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22c868.a029e027.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22cfa9.c3ad84e5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22cfa9.c3ad84e5.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22d045.49742fba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22d045.49742fba.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22d465.bda8f4fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22d465.bda8f4fd.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22d73b.dfa038b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22d73b.dfa038b7.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22dd78.22451f1a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d22dd78.22451f1a.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230072.2a923e1e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230072.2a923e1e.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230133.4d593b1b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230133.4d593b1b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230542.ac480dbb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230542.ac480dbb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230e18.622c5bd1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d230e18.622c5bd1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d231232.002ed967.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d231232.002ed967.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d231616.d12dd813.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d231616.d12dd813.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237512.d6876b95.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237512.d6876b95.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237570.ab2c204b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237570.ab2c204b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237b1e.a4be70a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237b1e.a4be70a0.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237f2f.181cd3c1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d237f2f.181cd3c1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d238064.a771cc06.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d238064.a771cc06.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d238263.93599bee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d238263.93599bee.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d238609.1478f5d1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d238609.1478f5d1.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2386b5.6a9c92e4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-2d2386b5.6a9c92e4.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-7490c82a.ef9f624c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-7490c82a.ef9f624c.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-74b4d726.8521d79b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-74b4d726.8521d79b.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   891145 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-vendors.ddbc9dcb.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3578835 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/js/chunk-vendors.ddbc9dcb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   161713 2024-04-09 08:26:15.000000 modoboa-radicale-1.7.2/modoboa_radicale/static/modoboa_radicale/webpack-stats.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.054550 modoboa-radicale-1.7.2/modoboa_radicale/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.150550 modoboa-radicale-1.7.2/modoboa_radicale/templates/modoboa_radicale/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/templates/modoboa_radicale/calendar_display.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/modoboa_radicale/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/test_data/events.ics
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/urls_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/modoboa_radicale/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-09 08:26:46.000000 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37420 2024-04-09 08:26:47.000000 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:26:46.000000 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:26:46.000000 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 08:26:46.000000 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 08:26:46.000000 modoboa-radicale-1.7.2/modoboa_radicale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/test_project/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test_project/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:26:47.154550 modoboa-radicale-1.7.2/test_project/test_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test_project/test_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8142 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test_project/test_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test_project/test_project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test_project/test_project/webpack-stats.json
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-09 08:25:26.000000 modoboa-radicale-1.7.2/test_project/test_project/wsgi.py
```

### Comparing `modoboa-radicale-1.7.1/.github/workflows/plugin.yml` & `modoboa-radicale-1.7.2/.github/workflows/plugin.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 name: Modoboa radicale plugin
 
 on:
   push:
     branches: [ master ]
+    paths-ignore:
+      - 'modoboa_radicale/**.po'
+      - 'frontend/**'
   pull_request:
     branches: [ master ]
+    paths-ignore:
+      - 'modoboa_radicale/**.po'
+      - 'frontend/**'
   release:
     branches: [ master ]
     types: [ published ]
 
 env:
   POSTGRES_HOST: localhost
 
@@ -24,23 +30,23 @@
           POSTGRES_DB: postgres
         ports:
         # will assign a random free host port
         - 5432/tcp
         # needed because the postgres container does not provide a healthcheck
         options: --health-cmd pg_isready --health-interval 10s --health-timeout 5s --health-retries 5
       mysql:
-        image: mysql:8.0
+        image: mariadb:11
         env:
-          MYSQL_ROOT_PASSWORD: root
-          MYSQL_USER: modoboa
-          MYSQL_PASSWORD: modoboa
-          MYSQL_DATABASE: modoboa
+          MARIADB_ROOT_PASSWORD: root
+          MARIADB_USER: modoboa
+          MARIADB_PASSWORD: modoboa
+          MARIADB_DATABASE: modoboa
         ports:
           - 3306/tcp
-        options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
+        options: --health-cmd="mariadb-admin ping" --health-interval=10s --health-timeout=5s --health-retries=3
       redis:
         image: redis
         ports:
           - 6379/tcp
         options: >-
           --health-cmd "redis-cli ping"
           --health-interval 10s
@@ -50,17 +56,17 @@
     strategy:
       matrix:
         database: ['postgres', 'mysql']
         python-version: [3.8, 3.9, '3.10', '3.11']
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           sudo apt-get update -y && sudo apt-get install -y librrd-dev rrdtool redis-server
           python -m pip install --upgrade pip
           pip install -r requirements.txt
@@ -82,30 +88,30 @@
           pip install coverage
           echo "DB=postgres" >> $GITHUB_ENV
       - name: Install mysql requirements
         if: ${{ matrix.database == 'mysql' }}
         run: |
           echo "DB=mysql" >> $GITHUB_ENV
       - name: Test with pytest
-        if: ${{ matrix.python-version != '3.10' || matrix.database != 'postgres' }}
+        if: ${{ matrix.python-version != '3.11' || matrix.database != 'postgres' }}
         run: |
           cd test_project
           python3 manage.py test modoboa_radicale
         env:
           # use localhost for the host here because we are running the job on the VM.
           # If we were running the job on in a container this would be postgres
           POSTGRES_PORT: ${{ job.services.postgres.ports[5432] }} # get randomly assigned published port
           MYSQL_HOST: 127.0.0.1
           MYSQL_PORT: ${{ job.services.mysql.ports[3306] }} # get randomly assigned published port
           MYSQL_USER: root
           REDIS_HOST: localhost
           REDIS_PORT: ${{ job.services.redis.ports[6379] }}
 
       - name: Test with pytest and coverage
-        if: ${{ matrix.python-version == '3.10' && matrix.database == 'postgres' }}
+        if: ${{ matrix.python-version == '3.11' && matrix.database == 'postgres' }}
         run: |
           cd test_project
           coverage run --source ../modoboa_radicale manage.py test modoboa_radicale
           coverage xml
           coverage report
         env:
           # use localhost for the host here because we are running the job on the VM.
@@ -113,71 +119,77 @@
           POSTGRES_PORT: ${{ job.services.postgres.ports[5432] }} # get randomly assigned published port
           MYSQL_HOST: 127.0.0.1
           MYSQL_PORT: ${{ job.services.mysql.ports[3306] }} # get randomly assigned published port
           MYSQL_USER: root
           REDIS_HOST: localhost
           REDIS_PORT: ${{ job.services.redis.ports[6379] }}
       - name: Upload coverage result
-        if: ${{ matrix.python-version == '3.10' }}
-        uses: actions/upload-artifact@v3
+        if: ${{ matrix.python-version == '3.11' && matrix.database == 'postgres' }}
+        uses: actions/upload-artifact@v4
         with:
           name: coverage-results
           path: test_project/coverage.xml
 
   coverage:
     needs: test
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Download coverage results
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: coverage-results
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           files: ./coverage.xml
 
   release:
     if: github.event_name != 'pull_request'
     needs: coverage
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
+    environment:
+      name: pypi
+      url: https://pypi.org/p/modoboa-radicale
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - name: Set up Python 3.10
-        uses: actions/setup-python@v4
+      - name: Set up Python 3.11
+        uses: actions/setup-python@v5
         with:
-          python-version: '3.10'
+          python-version: '3.11'
       - name: Build frontend
         shell: bash -l {0}
         run: |
           cd frontend
-          nvm install 10.15
+          nvm install 14
           npm install
           npm run build
           cd ..
       - name: Build packages
         run: |
           sudo apt-get install librrd-dev rrdtool libssl-dev gettext
           python -m pip install --upgrade pip setuptools wheel
           pip install -r requirements.txt
-          cd modoboa_radicale
+          cd ..
+          git clone https://github.com/modoboa/modoboa.git
+          cd modoboa
+          python setup.py develop
+          cd ../modoboa-radicale/modoboa_radicale
           django-admin compilemessages
           cd ..
           python setup.py sdist bdist_wheel
       - name: Publish to Test PyPI
         if: endsWith(github.event.ref, '/master')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
-          password: ${{ secrets.test_pypi_password }}
-          repository_url: https://test.pypi.org/legacy/
-          skip_existing: true
+          repository-url: https://test.pypi.org/legacy/
+          skip-existing: true
       - name: Publish distribution to PyPI
         if: startsWith(github.event.ref, 'refs/tags') || github.event_name == 'release'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          user: __token__
-          password: ${{ secrets.pypi_password }}
-          skip_existing: true
+          skip-existing: true
```

### Comparing `modoboa-radicale-1.7.1/.gitignore` & `modoboa-radicale-1.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/LICENSE` & `modoboa-radicale-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/PKG-INFO` & `modoboa-radicale-1.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: modoboa-radicale
-Version: 1.7.1
+Version: 1.7.2
 Summary: The Radicale frontend of Modoboa
 Home-page: http://modoboa.org/
 Author: Antoine Nguyen
 Author-email: tonio@ngyn.org
 License: MIT
 Keywords: modoboa email radicale calendar caldav
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
-Requires-Dist: django-filter==23.5
 Requires-Dist: drf-nested-routers
 Requires-Dist: django-webpack-loader==2.0.1
+Requires-Dist: lxml==4.9.4
 Requires-Dist: caldav==1.3.9
 
 modoboa-radicale
 ================
 
 |gha| |codecov|
```

### Comparing `modoboa-radicale-1.7.1/README.rst` & `modoboa-radicale-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/docs/Makefile` & `modoboa-radicale-1.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/docs/conf.py` & `modoboa-radicale-1.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/docs/index.rst` & `modoboa-radicale-1.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/docs/setup.rst` & `modoboa-radicale-1.7.2/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/.eslintrc.js` & `modoboa-radicale-1.7.2/frontend/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/Makefile` & `modoboa-radicale-1.7.2/frontend/Makefile`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/br/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/br/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/en/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/en/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/es/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/es/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/fr/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/fr/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/it/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/it/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/ro_RO/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/ro_RO/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/ru/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/ru/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/locale/zh_TW/LC_MESSAGES/app.po` & `modoboa-radicale-1.7.2/frontend/locale/zh_TW/LC_MESSAGES/app.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/package.json` & `modoboa-radicale-1.7.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/public/favicon.ico` & `modoboa-radicale-1.7.2/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/public/index.html` & `modoboa-radicale-1.7.2/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/App.vue` & `modoboa-radicale-1.7.2/frontend/src/App.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/api.js` & `modoboa-radicale-1.7.2/frontend/src/api.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/Calendar.vue` & `modoboa-radicale-1.7.2/frontend/src/components/Calendar.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/CalendarAccessRulesForm.vue` & `modoboa-radicale-1.7.2/frontend/src/components/CalendarAccessRulesForm.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/CalendarDetail.vue` & `modoboa-radicale-1.7.2/frontend/src/components/CalendarDetail.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/CalendarForm.vue` & `modoboa-radicale-1.7.2/frontend/src/components/CalendarForm.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/CreateEventForm.vue` & `modoboa-radicale-1.7.2/frontend/src/components/CreateEventForm.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/EventForm.vue` & `modoboa-radicale-1.7.2/frontend/src/components/EventForm.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/ImportEventsForm.vue` & `modoboa-radicale-1.7.2/frontend/src/components/ImportEventsForm.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/components/Modal.vue` & `modoboa-radicale-1.7.2/frontend/src/components/Modal.vue`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/main.js` & `modoboa-radicale-1.7.2/frontend/src/main.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/router/index.js` & `modoboa-radicale-1.7.2/frontend/src/router/index.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/store/modules/calendar.js` & `modoboa-radicale-1.7.2/frontend/src/store/modules/calendar.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/store/modules/event.js` & `modoboa-radicale-1.7.2/frontend/src/store/modules/event.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/store/mutation-types.js` & `modoboa-radicale-1.7.2/frontend/src/store/mutation-types.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/tools/permissions.js` & `modoboa-radicale-1.7.2/frontend/src/tools/permissions.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/src/translations.json` & `modoboa-radicale-1.7.2/frontend/src/translations.json`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/frontend/vue.config.js` & `modoboa-radicale-1.7.2/frontend/vue.config.js`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/backends/__init__.py` & `modoboa-radicale-1.7.2/modoboa_radicale/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/backends/caldav_.py` & `modoboa-radicale-1.7.2/modoboa_radicale/backends/caldav_.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/factories.py` & `modoboa-radicale-1.7.2/modoboa_radicale/factories.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/forms.py` & `modoboa-radicale-1.7.2/modoboa_radicale/forms.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/handlers.py` & `modoboa-radicale-1.7.2/modoboa_radicale/handlers.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/br/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/br/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/de/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/de/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/en/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/es/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/es/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/fr/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/fr/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/it/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/it/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/ro_RO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/ru/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/ru/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/sv/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/sv/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.mo` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.po` & `modoboa-radicale-1.7.2/modoboa_radicale/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/management/commands/generate_rights.py` & `modoboa-radicale-1.7.2/modoboa_radicale/management/commands/generate_rights.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/migrations/0001_initial.py` & `modoboa-radicale-1.7.2/modoboa_radicale/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/migrations/0002_auto_20170831_1721.py` & `modoboa-radicale-1.7.2/modoboa_radicale/migrations/0002_auto_20170831_1721.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/migrations/0003_auto_20180324_1834.py` & `modoboa-radicale-1.7.2/modoboa_radicale/migrations/0003_auto_20180324_1834.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/migrations/0004_auto_20200220_1816.py` & `modoboa-radicale-1.7.2/modoboa_radicale/migrations/0004_auto_20200220_1816.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/migrations/0005_auto_20200220_1819.py` & `modoboa-radicale-1.7.2/modoboa_radicale/migrations/0005_auto_20200220_1819.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/mocks.py` & `modoboa-radicale-1.7.2/modoboa_radicale/mocks.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/models.py` & `modoboa-radicale-1.7.2/modoboa_radicale/models.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/modo_extension.py` & `modoboa-radicale-1.7.2/modoboa_radicale/modo_extension.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/serializers.py` & `modoboa-radicale-1.7.2/modoboa_radicale/serializers.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/settings.py` & `modoboa-radicale-1.7.2/modoboa_radicale/settings.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/templates/modoboa_radicale/calendar_display.html` & `modoboa-radicale-1.7.2/modoboa_radicale/templates/modoboa_radicale/calendar_display.html`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/test_data/events.ics` & `modoboa-radicale-1.7.2/modoboa_radicale/test_data/events.ics`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/tests.py` & `modoboa-radicale-1.7.2/modoboa_radicale/tests.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/urls_api.py` & `modoboa-radicale-1.7.2/modoboa_radicale/urls_api.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/views.py` & `modoboa-radicale-1.7.2/modoboa_radicale/views.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale/viewsets.py` & `modoboa-radicale-1.7.2/modoboa_radicale/viewsets.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/modoboa_radicale.egg-info/PKG-INFO` & `modoboa-radicale-1.7.2/modoboa_radicale.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: modoboa-radicale
-Version: 1.7.1
+Version: 1.7.2
 Summary: The Radicale frontend of Modoboa
 Home-page: http://modoboa.org/
 Author: Antoine Nguyen
 Author-email: tonio@ngyn.org
 License: MIT
 Keywords: modoboa email radicale calendar caldav
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 2.2
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Internet :: WWW/HTTP
 License-File: LICENSE
-Requires-Dist: django-filter==23.5
 Requires-Dist: drf-nested-routers
 Requires-Dist: django-webpack-loader==2.0.1
+Requires-Dist: lxml==4.9.4
 Requires-Dist: caldav==1.3.9
 
 modoboa-radicale
 ================
 
 |gha| |codecov|
```

### Comparing `modoboa-radicale-1.7.1/pylintrc` & `modoboa-radicale-1.7.2/pylintrc`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/setup.py` & `modoboa-radicale-1.7.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,22 @@
                     if req.link:
                         dependencies.append(str(req.link))
             except AttributeError:
                 requirements.append(req.requirement)
     return requirements, dependencies
 
 
+def local_scheme(version):
+    """
+    Skip the local version (eg. +xyz of 0.6.1.dev4+gdf99fe2)
+    to be able to upload to Test PyPI
+    """
+    return ""
+
+
 if __name__ == "__main__":
     HERE = path.abspath(path.dirname(__file__))
     INSTALL_REQUIRES, DEPENDENCY_LINKS = (
         get_requirements(path.join(HERE, "requirements.txt")))
 
     with io.open(path.join(HERE, "README.rst"), encoding="utf-8") as readme:
         LONG_DESCRIPTION = readme.read()
@@ -60,22 +68,23 @@
             "Development Status :: 5 - Production/Stable",
             "Environment :: Web Environment",
             "Framework :: Django :: 2.2",
             "Intended Audience :: System Administrators",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
             "Programming Language :: Python :: 3",
-            "Programming Language :: Python :: 3.5",
-            "Programming Language :: Python :: 3.6",
-            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Topic :: Communications :: Email",
             "Topic :: Internet :: WWW/HTTP",
         ],
         keywords="modoboa email radicale calendar caldav",
         packages=find_packages(exclude=["docs", "test_project"]),
         include_package_data=True,
         zip_safe=False,
         install_requires=INSTALL_REQUIRES,
         dependency_links=DEPENDENCY_LINKS,
-        use_scm_version=True,
+        use_scm_version={"local_scheme": local_scheme},
         setup_requires=["setuptools_scm"],
     )
```

### Comparing `modoboa-radicale-1.7.1/test_project/manage.py` & `modoboa-radicale-1.7.2/test_project/manage.py`

 * *Files identical despite different names*

### Comparing `modoboa-radicale-1.7.1/test_project/test_project/settings.py` & `modoboa-radicale-1.7.2/test_project/test_project/settings.py`

 * *Files identical despite different names*

