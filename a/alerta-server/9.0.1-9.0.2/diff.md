# Comparing `tmp/alerta-server-9.0.1.tar.gz` & `tmp/alerta-server-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alerta-server-9.0.1.tar", last modified: Thu Jun 22 20:25:37 2023, max compression
+gzip compressed data, was "alerta-server-9.0.2.tar", last modified: Tue Apr  9 09:50:11 2024, max compression
```

## Comparing `alerta-server-9.0.1.tar` & `alerta-server-9.0.2.tar`

### file list

```diff
@@ -1,184 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.316700 alerta-server-9.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 20:25:26.000000 alerta-server-9.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 20:25:26.000000 alerta-server-9.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-22 20:25:26.000000 alerta-server-9.0.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-22 20:25:37.316700 alerta-server-9.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-22 20:25:26.000000 alerta-server-9.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 20:25:26.000000 alerta-server-9.0.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.284699 alerta-server-9.0.1/alerta/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/app.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.288699 alerta-server-9.0.1/alerta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/basic_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/userinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.288699 alerta-server-9.0.1/alerta/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.288699 alerta-server-9.0.1/alerta/database/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.292700 alerta-server-9.0.1/alerta/database/backends/mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71239 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7592 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/queryparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/mongodb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.292700 alerta-server-9.0.1/alerta/database/backends/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70404 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/queryparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17235 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/backends/postgres/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/database/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.292700 alerta-server-9.0.1/alerta/management/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/management/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/models/alarms/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alarms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alarms/alerta.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alarms/isa_18_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25626 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/blackout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/acked_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/blackout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/escalate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/reject.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/remote_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/plugins/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/sql/
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/sql/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/static/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/static/embed.js
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/templates/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/auth/saml2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.296700 alerta-server-9.0.1/alerta/templates/management/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/management/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/management/switchboard.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.300700 alerta-server-9.0.1/alerta/templates/oembed/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/templates/oembed/counts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.300700 alerta-server-9.0.1/alerta/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/mailer.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/paging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/utils/webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.304700 alerta-server-9.0.1/alerta/views/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22749 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/oembed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.308700 alerta-server-9.0.1/alerta/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/grafana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/graylog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/newrelic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/pagerduty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/pingdom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/riemann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/serverdensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/stackdriver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-22 20:25:26.000000 alerta-server-9.0.1/alerta/webhooks/telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.308700 alerta-server-9.0.1/alerta_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 20:25:37.000000 alerta-server-9.0.1/alerta_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 20:25:37.316700 alerta-server-9.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-22 20:25:26.000000 alerta-server-9.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.316700 alerta-server-9.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:37.316700 alerta-server-9.0.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (123)    39105 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23677 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_authproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    35064 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_blackouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_cors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_customers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10866 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    40388 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_isa_18_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26434 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)   113133 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_queryparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9088 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    29127 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_shelving.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    57492 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-22 20:25:26.000000 alerta-server-9.0.1/tests/test_zrouting.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 20:25:26.000000 alerta-server-9.0.1/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 09:50:08.000000 alerta-server-9.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 09:50:08.000000 alerta-server-9.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 09:50:08.000000 alerta-server-9.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-09 09:50:11.876413 alerta-server-9.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-09 09:50:08.000000 alerta-server-9.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 09:50:08.000000 alerta-server-9.0.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/app.wsgi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/basic_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/userinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/database/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.856413 alerta-server-9.0.2/alerta/database/backends/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71239 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16836 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/mongodb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/database/backends/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70404 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17681 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/backends/postgres/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/database/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/management/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.860413 alerta-server-9.0.2/alerta/models/alarms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alarms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10983 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alarms/alerta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alarms/isa_18_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25626 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/acked_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/blackout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/escalate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/reject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/remote_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/plugins/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/sql/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/static/embed.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/auth/saml2.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/management/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/management/switchboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.864413 alerta-server-9.0.2/alerta/templates/oembed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/templates/oembed/counts.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.868413 alerta-server-9.0.2/alerta/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7913 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/mailer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/paging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/utils/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.868413 alerta-server-9.0.2/alerta/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22749 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/oembed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.872413 alerta-server-9.0.2/alerta/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/grafana.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/graylog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/newrelic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/pagerduty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/pingdom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/riemann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/serverdensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/stackdriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-09 09:50:08.000000 alerta-server-9.0.2/alerta/webhooks/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/alerta_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 09:50:11.000000 alerta-server-9.0.2/alerta_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 09:50:11.880413 alerta-server-9.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-09 09:50:08.000000 alerta-server-9.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:11.876413 alerta-server-9.0.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39105 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23677 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_authproxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35064 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_blackouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17393 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17811 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40388 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_isa_18_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13243 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113133 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19021 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_severity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_shelving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57492 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-09 09:50:08.000000 alerta-server-9.0.2/tests/test_zrouting.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 09:50:08.000000 alerta-server-9.0.2/wsgi.py
```

### Comparing `alerta-server-9.0.1/LICENSE` & `alerta-server-9.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/NOTICE` & `alerta-server-9.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/PKG-INFO` & `alerta-server-9.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 Metadata-Version: 2.1
 Name: alerta-server
-Version: 9.0.1
+Version: 9.0.2
 Summary: Alerta server WSGI application
 Home-page: https://github.com/guardian/alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alert monitoring system wsgi application api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Plugins
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: mongodb
-Provides-Extra: postgres
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: bcrypt
+Requires-Dist: blinker
+Requires-Dist: cryptography
+Requires-Dist: Flask>=2.0.1
+Requires-Dist: Flask-Compress>=1.4.0
+Requires-Dist: Flask-Cors>=3.0.2
+Requires-Dist: mohawk
+Requires-Dist: PyJWT>=2.0.0
+Requires-Dist: pyparsing
+Requires-Dist: python-dateutil
+Requires-Dist: pytz
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: requests-hawk
+Requires-Dist: sentry-sdk[flask]>=0.10.2
+Provides-Extra: mongodb
+Requires-Dist: pymongo; extra == "mongodb"
+Provides-Extra: postgres
+Requires-Dist: psycopg2; extra == "postgres"
 
-Alerta Release 9.0
+Alerta Release 9.1
 ==================
 
 [![Actions Status](https://github.com/alerta/alerta/workflows/CI%20Tests/badge.svg)](https://github.com/alerta/alerta/actions)
 [![Slack chat](https://img.shields.io/badge/chat-on%20slack-blue?logo=slack)](https://slack.alerta.dev)
 [![Coverage Status](https://coveralls.io/repos/github/alerta/alerta/badge.svg?branch=master)](https://coveralls.io/github/alerta/alerta?branch=master)
 [![Docker Pulls](https://img.shields.io/docker/pulls/alerta/alerta-web.svg)](https://hub.docker.com/r/alerta/alerta-web)
 
@@ -44,20 +61,20 @@
 ![webui](/docs/images/alerta-webui-v7.jpg?raw=true)
 
 ----
 
 Requirements
 ------------
 
-Release 9 only supports Python 3.8 or higher.
+Release 9 only supports Python 3.9 or higher.
 
 The only mandatory dependency is MongoDB or PostgreSQL. Everything else is optional.
 
-- Postgres version 11 or better
-- MongoDB version 4.4 or better
+- Postgres version 13 or better
+- MongoDB version 6.0 or better
 
 Installation
 ------------
 
 To install MongoDB on Debian/Ubuntu run:
 
     $ sudo apt-get install -y mongodb-org
```

### Comparing `alerta-server-9.0.1/README.md` & `alerta-server-9.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Alerta Release 9.0
+Alerta Release 9.1
 ==================
 
 [![Actions Status](https://github.com/alerta/alerta/workflows/CI%20Tests/badge.svg)](https://github.com/alerta/alerta/actions)
 [![Slack chat](https://img.shields.io/badge/chat-on%20slack-blue?logo=slack)](https://slack.alerta.dev)
 [![Coverage Status](https://coveralls.io/repos/github/alerta/alerta/badge.svg?branch=master)](https://coveralls.io/github/alerta/alerta?branch=master)
 [![Docker Pulls](https://img.shields.io/docker/pulls/alerta/alerta-web.svg)](https://hub.docker.com/r/alerta/alerta-web)
 
@@ -15,20 +15,20 @@
 ![webui](/docs/images/alerta-webui-v7.jpg?raw=true)
 
 ----
 
 Requirements
 ------------
 
-Release 9 only supports Python 3.8 or higher.
+Release 9 only supports Python 3.9 or higher.
 
 The only mandatory dependency is MongoDB or PostgreSQL. Everything else is optional.
 
-- Postgres version 11 or better
-- MongoDB version 4.4 or better
+- Postgres version 13 or better
+- MongoDB version 6.0 or better
 
 Installation
 ------------
 
 To install MongoDB on Debian/Ubuntu run:
 
     $ sudo apt-get install -y mongodb-org
```

### Comparing `alerta-server-9.0.1/alerta/app.py` & `alerta-server-9.0.2/alerta/app.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/auth/__init__.py` & `alerta-server-9.0.2/alerta/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 
 class AuthBlueprint(Blueprint):
 
     def register(self, app, options):
         if app.config['AUTH_PROVIDER'] == 'ldap':
             try:
                 import ldap  # noqa
+
                 from . import basic_ldap  # noqa
             except ImportError:
                 raise RuntimeError('Must install python-ldap to use LDAP authentication module')
         else:
             from . import basic  # noqa
 
         if app.config['AUTH_PROVIDER'] == 'saml2':
             try:
                 import saml2  # noqa
+
                 from . import saml  # noqa
             except ImportError:
                 raise RuntimeError('Must install pysaml2 to use SAML2 authentication module')
 
         if app.config['AUTH_PROVIDER'] in ['openid', 'azure', 'cognito', 'gitlab', 'keycloak']:
             try:
                 oidc_config, _ = oidc.get_oidc_configuration(app)
```

### Comparing `alerta-server-9.0.1/alerta/auth/basic.py` & `alerta-server-9.0.2/alerta/auth/basic.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/auth/basic_ldap.py` & `alerta-server-9.0.2/alerta/auth/basic_ldap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ldap  # pylint: disable=import-error
+import ldap.filter
 from flask import current_app, jsonify, request
 
 from alerta.auth.utils import create_token, get_customers, not_authorized
 from alerta.exceptions import ApiError
 from alerta.models.permission import Permission
 from alerta.models.user import User
 from alerta.utils.audit import auth_audit_trail
@@ -83,37 +84,39 @@
     #   Set the DN as the one found in LDAP_DOMAINS variable
     user_filter = current_app.config['LDAP_USER_FILTER']
     user_base_dn = current_app.config['LDAP_USER_BASEDN']
     user_attrs = [
         current_app.config['LDAP_USER_NAME_ATTR'],
         current_app.config['LDAP_USER_EMAIL_ATTR']
     ]
+    safe_username = ldap.filter.escape_filter_chars(username)
+    safe_domain = ldap.filter.escape_filter_chars(domain)
     if user_filter:
         result = [r for r in ldap_connection.search_s(
             base=user_base_dn or base_dn,
             scope=ldap.SCOPE_SUBTREE,
-            filterstr=user_filter.format(username=username),
+            filterstr=user_filter.format(username=safe_username),
             attrlist=user_attrs
         ) if None not in r]
 
         if len(result) > 1:
             raise ApiError(f'invalid search query for domain "{domain}"', 500)
         elif len(result) == 0:
             raise ApiError('invalid username or password', 401)
         user_dn = result[0][0]
         name = result[0][1][current_app.config['LDAP_USER_NAME_ATTR']][0].decode('utf-8', 'ignore')
         email = result[0][1][current_app.config['LDAP_USER_EMAIL_ATTR']][0].decode('utf-8', 'ignore')
         email_verified = bool(email)
     else:
         if '%' in current_app.config['LDAP_DOMAINS'][domain]:
-            user_dn = current_app.config['LDAP_DOMAINS'][domain] % username
+            user_dn = current_app.config['LDAP_DOMAINS'][domain] % safe_username
         else:
-            user_dn = current_app.config['LDAP_DOMAINS'][domain].format(username)
-        name = username
-        email = f'{username}@{domain}'
+            user_dn = current_app.config['LDAP_DOMAINS'][domain].format(safe_username)
+        name = safe_username
+        email = f'{safe_username}@{safe_domain}'
         email_verified = False
 
     # Authenticate user logging in
     try:
         ldap_connection.simple_bind_s(user_dn, password)
     except ldap.INVALID_CREDENTIALS:
         raise ApiError('invalid username or password', 401)
@@ -137,15 +140,15 @@
     group_filter = current_app.config['LDAP_GROUP_FILTER']
     group_base_dn = current_app.config['LDAP_GROUP_BASEDN']
     groups = list()
     if group_filter:
         result = ldap_connection.search_s(
             base=group_base_dn or base_dn,
             scope=ldap.SCOPE_SUBTREE,
-            filterstr=group_filter.format(username=username, email=email, userdn=user_dn),
+            filterstr=group_filter.format(username=safe_username, email=email, userdn=user_dn),
             attrlist=[current_app.config['LDAP_GROUP_NAME_ATTR']]
         )
         for group_dn, group_attrs in result:
             if current_app.config['LDAP_GROUP_NAME_ATTR'] in group_attrs.keys():
                 groups.extend([g.decode('utf-8', 'ignore') for g in group_attrs[current_app.config['LDAP_GROUP_NAME_ATTR']]])
             else:
                 groups.append(group_dn)
```

### Comparing `alerta-server-9.0.1/alerta/auth/decorators.py` & `alerta-server-9.0.2/alerta/auth/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from alerta.models.enums import ADMIN_SCOPES
 from alerta.models.key import ApiKey
 from alerta.models.permission import Permission
 from alerta.models.token import Jwt
 from alerta.models.user import User
 
 if TYPE_CHECKING:
-    from typing import List   # noqa
+    from typing import List  # noqa
+
     from alerta.models.enums import Scope  # noqa
 
 
 def permission(scope=None):
     def decorated(f):
         @wraps(f)
         def wrapped(*args, **kwargs):
```

### Comparing `alerta-server-9.0.1/alerta/auth/github.py` & `alerta-server-9.0.2/alerta/auth/github.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/auth/hmac.py` & `alerta-server-9.0.2/alerta/auth/hmac.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/auth/oidc.py` & `alerta-server-9.0.2/alerta/auth/oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         'code': request.json['code'],
         'redirect_uri': request.json['redirectUri'],
     }
 
     token_endpoint_auth_methods = oidc_configuration.get(
         'token_endpoint_auth_methods_supported',
         ['client_secret_basic'])
-    if type(token_endpoint_auth_methods) != list:
+    if not isinstance(token_endpoint_auth_methods, list):
         token_endpoint_auth_methods = [token_endpoint_auth_methods]
 
     preferred_token_auth_method = 'client_secret_post'
     for token_auth_method in current_app.config['OIDC_TOKEN_AUTH_METHODS']:
         if token_auth_method in token_endpoint_auth_methods:
             preferred_token_auth_method = token_auth_method
             break
```

### Comparing `alerta-server-9.0.1/alerta/auth/saml.py` & `alerta-server-9.0.2/alerta/auth/saml.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/auth/userinfo.py` & `alerta-server-9.0.2/alerta/auth/userinfo.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/auth/utils.py` & `alerta-server-9.0.2/alerta/auth/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
             password = password.encode('utf-8')
         return bcrypt.hashpw(password, bcrypt.gensalt(prefix=b'2a')).decode('utf-8')
 
     def check_password_hash(pwhash: str, password: Any) -> bool:
         return bcrypt.checkpw(password.encode('utf-8'), pwhash.encode('utf-8'))
 
 except ImportError:  # Google App Engine
-    from werkzeug.security import generate_password_hash, check_password_hash  # noqa
+    from werkzeug.security import check_password_hash  # noqa
+    from werkzeug.security import generate_password_hash  # noqa
 
 
 def not_authorized(allowed_setting: str, groups: List[str]) -> bool:
     return (current_app.config['AUTH_REQUIRED']
             and not ('*' in current_app.config[allowed_setting]
                      or set(current_app.config[allowed_setting]).intersection(set(groups))))
```

### Comparing `alerta-server-9.0.1/alerta/commands.py` & `alerta-server-9.0.2/alerta/commands.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/database/backends/mongodb/base.py` & `alerta-server-9.0.2/alerta/database/backends/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/database/backends/mongodb/queryparser.py` & `alerta-server-9.0.2/alerta/database/backends/mongodb/queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/database/backends/mongodb/utils.py` & `alerta-server-9.0.2/alerta/database/backends/mongodb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import re
 from collections import namedtuple
 from datetime import datetime
-from typing import Any, Dict, List
+from typing import Any, Dict, List  # noqa
 
 import pytz
 from pyparsing import ParseException
 from werkzeug.datastructures import ImmutableMultiDict, MultiDict
 
 from alerta.exceptions import ApiError
 from alerta.models.blackout import BlackoutStatus
@@ -216,17 +216,30 @@
         'createTime': ('createTime', 'createTime', -1),
         'text': ('text', 'text', 1),
     }
 
     @staticmethod
     def from_params(params: ImmutableMultiDict, customers=None, query_time=None):
 
-        query = dict()  # type: Dict[str, Any]
         params = MultiDict(params)  # type: ignore
 
+        # ?q=
+        if params.get('q', None):
+            try:
+                parser = QueryParser()
+                query = json.loads(parser.parse(
+                    query=params['q'],
+                    default_field=params.get('q.df'),
+                    default_operator=params.get('q.op')
+                ))
+            except ParseException as e:
+                raise ApiError('Failed to parse query string.', 400, [e])
+        else:
+            query = dict()
+
         # customer
         if customers:
             customer_query = {'customer': {'$in': customers}}
         else:
             customer_query = None  # type: ignore
 
         # status
```

### Comparing `alerta-server-9.0.1/alerta/database/backends/postgres/base.py` & `alerta-server-9.0.2/alerta/database/backends/postgres/base.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/database/backends/postgres/queryparser.py` & `alerta-server-9.0.2/alerta/database/backends/postgres/queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/database/backends/postgres/utils.py` & `alerta-server-9.0.2/alerta/database/backends/postgres/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,18 +220,31 @@
         'createTime': ('create_time', 'create_time', -1),
         'text': ('text', 'text', 1),
     }
 
     @staticmethod
     def from_params(params: MultiDict, customers=None, query_time=None):
 
-        query = ['1=1']
-        qvars = dict()
         params = MultiDict(params)
 
+        # ?q=
+        if params.get('q', None):
+            try:
+                parser = QueryParser()
+                query = [parser.parse(
+                    query=params['q'],
+                    default_field=params.get('q.df')
+                )]
+                qvars = dict()  # type: Dict[str, Any]
+            except ParseException as e:
+                raise ApiError('Failed to parse query string.', 400, [e])
+        else:
+            query = ['1=1']
+            qvars = dict()
+
         # customer
         if customers:
             query.append('AND customer=ANY(%(customers)s)')
             qvars['customers'] = customers
 
         # status
         status = params.poplist('status')
```

### Comparing `alerta-server-9.0.1/alerta/database/base.py` & `alerta-server-9.0.2/alerta/database/base.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/exceptions.py` & `alerta-server-9.0.2/alerta/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,17 @@
 def handle_exception(error: Exception) -> Union[Tuple[Response, int], Exception]:
     # RoutingExceptions are used internally to trigger routing
     # actions, such as slash redirects raising RequestRedirect.
     if isinstance(error, RoutingException):
         return error
 
     current_app.logger.exception(error)
+    current_app.logger.exception(traceback.format_exc())
     return jsonify({
         'status': 'error',
-        'message': str(error),
+        'message': 'An internal error has occurred!',
         'code': 500,
         'errors': [
-            traceback.format_exc()
+            str(error)
         ],
         'requestId': g.request_id
     }), 500
```

### Comparing `alerta-server-9.0.1/alerta/management/views.py` & `alerta-server-9.0.2/alerta/management/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,16 @@
         for heartbeat in heartbeats:
             delta = datetime.datetime.utcnow() - heartbeat.receive_time
             threshold = int(heartbeat.timeout) * 4
             if delta.seconds > threshold:
                 return f'HEARTBEAT_STALE: {heartbeat.origin}', 503
 
     except Exception as e:
-        return f'HEALTH_CHECK_FAILED: {e}', 503
+        current_app.logger.exception(e)
+        return 'HEALTH_CHECK_FAILED: Internal Error!', 503
 
     return 'OK'
 
 
 @mgmt.route('/management/housekeeping', methods=['OPTIONS', 'GET', 'POST'])
 @cross_origin()
 @permission(Scope.admin_management)
```

### Comparing `alerta-server-9.0.1/alerta/models/alarms/__init__.py` & `alerta-server-9.0.2/alerta/models/alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/alarms/alerta.py` & `alerta-server-9.0.2/alerta/models/alarms/alerta.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/alarms/isa_18_2.py` & `alerta-server-9.0.2/alerta/models/alarms/isa_18_2.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/alert.py` & `alerta-server-9.0.2/alerta/models/alert.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/blackout.py` & `alerta-server-9.0.2/alerta/models/blackout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import datetime, timedelta
-from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import uuid4
 
 from flask import current_app
+from strenum import StrEnum
 
 from alerta.app import db
 from alerta.database.base import Query
 from alerta.utils.format import DateTime
 from alerta.utils.response import absolute_url
 
 JSON = Dict[str, Any]
 
 
-class BlackoutStatus(str, Enum):
+class BlackoutStatus(StrEnum):
 
     Pending = 'pending'
     Active = 'active'
     Expired = 'expired'
 
 
 class Blackout:
```

### Comparing `alerta-server-9.0.1/alerta/models/customer.py` & `alerta-server-9.0.2/alerta/models/customer.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/enums.py` & `alerta-server-9.0.2/alerta/models/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
-from enum import Enum
 
+from strenum import StrEnum
 
-class Severity(str, Enum):
+
+class Severity(StrEnum):
 
     Security = 'security'
     Critical = 'critical'
     Major = 'major'
     Minor = 'minor'
     Warning = 'warning'
     Indeterminate = 'indeterminate'
@@ -15,41 +16,41 @@
     Ok = 'ok'
     Cleared = 'cleared'
     Debug = 'debug'
     Trace = 'trace'
     Unknown = 'unknown'
 
 
-class Status(str, Enum):
+class Status(StrEnum):
 
     Open = 'open'
     Assign = 'assign'
     Ack = 'ack'
     Shelved = 'shelved'
     Blackout = 'blackout'
     Closed = 'closed'
     Expired = 'expired'
     Unknown = 'unknown'
     Not_Valid = 'notValid'
 
 
-class Action(str, Enum):
+class Action(StrEnum):
 
     OPEN = 'open'
     ASSIGN = 'assign'
     ACK = 'ack'
     UNACK = 'unack'
     SHELVE = 'shelve'
     UNSHELVE = 'unshelve'
     CLOSE = 'close'
     EXPIRED = 'expired'
     TIMEOUT = 'timeout'
 
 
-class TrendIndication(str, Enum):
+class TrendIndication(StrEnum):
 
     More_Severe = 'moreSevere'
     No_Change = 'noChange'
     Less_Severe = 'lessSevere'
 
 
 class Scope(str):
@@ -139,15 +140,15 @@
         else:
             return Scope(action)
 
 
 ADMIN_SCOPES = [Scope.admin, Scope.read, Scope.write]
 
 
-class ChangeType(str, Enum):
+class ChangeType(StrEnum):
 
     open = 'open'
     assign = 'assign'
     ack = 'ack'
     unack = 'unack'
     shelve = 'shelve'
     unshelve = 'unshelve'
@@ -160,15 +161,15 @@
     severity = 'severity'
     note = 'note'
     dismiss = 'dismiss'  # note dismissed
     timeout = 'timeout'
     expired = 'expired'
 
 
-class NoteType(str, Enum):
+class NoteType(StrEnum):
 
     alert = 'alert'
     blackout = 'blackout'
     customer = 'customer'
     group = 'group'
     heartbeat = 'heartbeat'
     key = 'api-key'
```

### Comparing `alerta-server-9.0.1/alerta/models/group.py` & `alerta-server-9.0.2/alerta/models/group.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/heartbeat.py` & `alerta-server-9.0.2/alerta/models/heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import platform
 import sys
 from datetime import datetime
-from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import uuid4
 
 from flask import current_app
+from strenum import StrEnum
 
 from alerta.app import db
 from alerta.database.base import Query
 from alerta.utils.format import DateTime
 from alerta.utils.response import absolute_url
 
 JSON = Dict[str, Any]
 
 
-class HeartbeatStatus(str, Enum):
+class HeartbeatStatus(StrEnum):
 
     OK = 'ok'
     Slow = 'slow'
     Expired = 'expired'  # aka 'stale'
 
 
 class Heartbeat:
```

### Comparing `alerta-server-9.0.1/alerta/models/history.py` & `alerta-server-9.0.2/alerta/models/history.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/key.py` & `alerta-server-9.0.2/alerta/models/key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from datetime import datetime, timedelta
-from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import uuid4
 
+from strenum import StrEnum
+
 from alerta.app import db, key_helper
 from alerta.database.base import Query
 from alerta.models.enums import Scope
 from alerta.utils.format import DateTime
 from alerta.utils.response import absolute_url
 
 JSON = Dict[str, Any]
 
 
-class ApiKeyStatus(str, Enum):
+class ApiKeyStatus(StrEnum):
 
     Active = 'active'
     Expired = 'expired'
 
 
 class ApiKey:
```

### Comparing `alerta-server-9.0.1/alerta/models/metrics.py` & `alerta-server-9.0.2/alerta/models/metrics.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/note.py` & `alerta-server-9.0.2/alerta/models/note.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/permission.py` & `alerta-server-9.0.2/alerta/models/permission.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/switch.py` & `alerta-server-9.0.2/alerta/models/switch.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/token.py` & `alerta-server-9.0.2/alerta/models/token.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/models/user.py` & `alerta-server-9.0.2/alerta/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime
-from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import uuid4
 
 from flask import current_app
+from strenum import StrEnum
 
 from alerta.app import db
 from alerta.auth import utils
 from alerta.database.base import Query
 from alerta.models.group import Group
 from alerta.utils.response import absolute_url
 
 JSON = Dict[str, Any]
 
 
-class UserStatus(str, Enum):
+class UserStatus(StrEnum):
 
     Active = 'active'
     Inactive = 'inactive'
     Unknown = 'unknown'  # aka 'stale'
 
 
 class User:
```

### Comparing `alerta-server-9.0.1/alerta/plugins/__init__.py` & `alerta-server-9.0.2/alerta/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/acked_by.py` & `alerta-server-9.0.2/alerta/plugins/acked_by.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/blackout.py` & `alerta-server-9.0.2/alerta/plugins/blackout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/escalate.py` & `alerta-server-9.0.2/alerta/plugins/escalate.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/forwarder.py` & `alerta-server-9.0.2/alerta/plugins/forwarder.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/heartbeat.py` & `alerta-server-9.0.2/alerta/plugins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/reject.py` & `alerta-server-9.0.2/alerta/plugins/reject.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         ORIGIN_BLACKLIST_REGEX = [re.compile(x) for x in ORIGIN_BLACKLIST]
         ALLOWED_ENVIRONMENT_REGEX = [re.compile(x) for x in ALLOWED_ENVIRONMENTS]
 
         if any(regex.match(alert.origin) for regex in ORIGIN_BLACKLIST_REGEX):
             LOG.warning("[POLICY] Alert origin '%s' has been blacklisted", alert.origin)
             raise RejectException(f"[POLICY] Alert origin '{alert.origin}' has been blacklisted")
 
-        if not any(regex.match(alert.environment) for regex in ALLOWED_ENVIRONMENT_REGEX):
+        if not any(regex.fullmatch(alert.environment) for regex in ALLOWED_ENVIRONMENT_REGEX):
             LOG.warning('[POLICY] Alert environment does not match one of %s', ', '.join(ALLOWED_ENVIRONMENTS))
             raise RejectException('[POLICY] Alert environment does not match one of %s' %
                                   ', '.join(ALLOWED_ENVIRONMENTS))
 
         if not alert.service:
             LOG.warning('[POLICY] Alert must define a service')
             raise RejectException('[POLICY] Alert must define a service')
```

### Comparing `alerta-server-9.0.1/alerta/plugins/remote_ip.py` & `alerta-server-9.0.2/alerta/plugins/remote_ip.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/plugins/timeout.py` & `alerta-server-9.0.2/alerta/plugins/timeout.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/settings.py` & `alerta-server-9.0.2/alerta/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,7 +283,11 @@
     # ('http://localhost:9000', {'token': 'bearer-token'}, ['alerts', 'actions']),  # Bearer token
 ]  # type: List[Tuple]
 
 # valid actions=['*', 'alerts', 'actions', 'open', 'assign', 'ack', 'unack', 'shelve', 'unshelve', 'close', 'delete']
 
 # Webhooks
 DEFAULT_ENVIRONMENT = 'Production'  # default environment used by webhooks, value must be in ALLOWED_ENVIRONMENTS
+
+# Grafana webhook keep legacy behavior by default
+GRAFANA_TAGS_AS_ATTRIBUTES = True
+GRAFANA_TAGS_AS_TAGS = False
```

### Comparing `alerta-server-9.0.1/alerta/sql/schema.sql` & `alerta-server-9.0.2/alerta/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/static/embed.js` & `alerta-server-9.0.2/alerta/static/embed.js`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/tasks.py` & `alerta-server-9.0.2/alerta/tasks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/templates/index.html` & `alerta-server-9.0.2/alerta/templates/index.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/templates/management/switchboard.html` & `alerta-server-9.0.2/alerta/templates/management/switchboard.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/templates/oembed/counts.html` & `alerta-server-9.0.2/alerta/templates/oembed/counts.html`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/api.py` & `alerta-server-9.0.2/alerta/utils/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
 
 def process_action(alert: Alert, action: str, text: str, timeout: int = None) -> Tuple[Alert, str, str, Optional[int]]:
 
     wanted_plugins, wanted_config = plugins.routing(alert)
 
     updated = None
+    alert_was_updated = False
     for plugin in wanted_plugins:
         if alert.is_suppressed:
             break
         try:
             updated = plugin.take_action(alert, action, text, timeout=timeout, config=wanted_config)
         except NotImplementedError:
             pass  # plugin does not support action() method
@@ -115,27 +116,30 @@
         if isinstance(updated, Alert):
             updated = updated, action, text, timeout
         if isinstance(updated, tuple):
             if len(updated) == 4:
                 alert, action, text, timeout = updated
             elif len(updated) == 3:
                 alert, action, text = updated
+        if updated:
+            alert_was_updated = True
 
-    if updated:
+    if alert_was_updated:
         alert.update_tags(alert.tags)
         alert.attributes = alert.update_attributes(alert.attributes)
 
     return alert, action, text, timeout
 
 
 def process_note(alert: Alert, text: str) -> Tuple[Alert, str]:
 
     wanted_plugins, wanted_config = plugins.routing(alert)
 
     updated = None
+    alert_was_updated = False
     for plugin in wanted_plugins:
         try:
             updated = plugin.take_note(alert, text, config=wanted_config)
         except NotImplementedError:
             pass  # plugin does not support take_note() method
         except (RejectException, ForwardingLoop, AlertaException):
             raise
@@ -145,27 +149,30 @@
             else:
                 logging.error(f"Error while running note plugin '{plugin.name}': {str(e)}")
 
         if isinstance(updated, Alert):
             updated = updated, text
         if isinstance(updated, tuple) and len(updated) == 2:
             alert, text = updated
+        if updated:
+            alert_was_updated = True
 
-    if updated:
+    if alert_was_updated:
         alert.update_tags(alert.tags)
         alert.update_attributes(alert.attributes)
 
     return alert, text
 
 
 def process_status(alert: Alert, status: str, text: str) -> Tuple[Alert, str, str]:
 
     wanted_plugins, wanted_config = plugins.routing(alert)
 
     updated = None
+    alert_was_updated = False
     for plugin in wanted_plugins:
         if alert.is_suppressed:
             break
         try:
             updated = plugin.status_change(alert, status, text, config=wanted_config)
         except TypeError:
             updated = plugin.status_change(alert, status, text)  # for backward compatibility
@@ -173,20 +180,21 @@
             raise
         except Exception as e:
             if current_app.config['PLUGINS_RAISE_ON_ERROR']:
                 raise ApiError(f"Error while running status plugin '{plugin.name}': {str(e)}")
             else:
                 logging.error(f"Error while running status plugin '{plugin.name}': {str(e)}")
         if updated:
+            alert_was_updated = True
             try:
                 alert, status, text = updated
             except Exception:
                 alert = updated
 
-    if updated:
+    if alert_was_updated:
         alert.update_tags(alert.tags)
         alert.attributes = alert.update_attributes(alert.attributes)
 
     return alert, status, text
 
 
 def process_delete(alert: Alert) -> bool:
```

### Comparing `alerta-server-9.0.1/alerta/utils/audit.py` & `alerta-server-9.0.2/alerta/utils/audit.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/client.py` & `alerta-server-9.0.2/alerta/utils/client.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/config.py` & `alerta-server-9.0.2/alerta/utils/config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/format.py` & `alerta-server-9.0.2/alerta/utils/format.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/hooks.py` & `alerta-server-9.0.2/alerta/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/key.py` & `alerta-server-9.0.2/alerta/utils/key.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/logging.py` & `alerta-server-9.0.2/alerta/utils/logging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/mailer.py` & `alerta-server-9.0.2/alerta/utils/mailer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from flask import Flask, current_app
 
 try:
     import smtplib
     import socket
     import ssl
-
-    from smtplib import SMTP  # noqa
-    from email.mime.text import MIMEText
     from email.mime.multipart import MIMEMultipart
+    from email.mime.text import MIMEText
+    from smtplib import SMTP  # noqa
 except ImportError:
     pass
 
 
 class Mailer:
 
     def __init__(self, app: Flask = None) -> None:
```

### Comparing `alerta-server-9.0.1/alerta/utils/paging.py` & `alerta-server-9.0.2/alerta/utils/paging.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/plugin.py` & `alerta-server-9.0.2/alerta/utils/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from alerta.plugins import app
 
 LOG = logging.getLogger('alerta.plugins')
 
 if TYPE_CHECKING:
     from typing import Iterable, Tuple  # noqa
+
     from alerta.models.alert import Alert  # noqa
     from alerta.plugins import PluginBase  # noqa
 
 
 class Plugins:
 
     def __init__(self) -> None:
```

### Comparing `alerta-server-9.0.1/alerta/utils/response.py` & `alerta-server-9.0.2/alerta/utils/response.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/tracing.py` & `alerta-server-9.0.2/alerta/utils/tracing.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/utils/webhook.py` & `alerta-server-9.0.2/alerta/utils/webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import TYPE_CHECKING, Iterator
 
 from flask import Flask
 from pkg_resources import iter_entry_points
 
 if TYPE_CHECKING:
     from typing import Dict  # noqa
+
     from alerta.webhooks import WebhookBase  # noqa
 
 
 class WebhookRule:
 
     def __init__(self, rule, endpoint, methods):
         self.rule = rule
```

### Comparing `alerta-server-9.0.1/alerta/views/__init__.py` & `alerta-server-9.0.2/alerta/views/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/alerts.py` & `alerta-server-9.0.2/alerta/views/alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/blackouts.py` & `alerta-server-9.0.2/alerta/views/blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/bulk.py` & `alerta-server-9.0.2/alerta/views/bulk.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/config.py` & `alerta-server-9.0.2/alerta/views/config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/customers.py` & `alerta-server-9.0.2/alerta/views/customers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/groups.py` & `alerta-server-9.0.2/alerta/views/groups.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/heartbeats.py` & `alerta-server-9.0.2/alerta/views/heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/keys.py` & `alerta-server-9.0.2/alerta/views/keys.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/oembed.py` & `alerta-server-9.0.2/alerta/views/oembed.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/permissions.py` & `alerta-server-9.0.2/alerta/views/permissions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/views/users.py` & `alerta-server-9.0.2/alerta/views/users.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/__init__.py` & `alerta-server-9.0.2/alerta/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/cloudwatch.py` & `alerta-server-9.0.2/alerta/webhooks/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/custom.py` & `alerta-server-9.0.2/alerta/webhooks/custom.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/grafana.py` & `alerta-server-9.0.2/alerta/webhooks/grafana.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from . import WebhookBase
 
 JSON = Dict[str, Any]
 
 
 def parse_grafana(args: ImmutableMultiDict, alert: JSON, match: Dict[str, Any]) -> Alert:
 
+    # default to setting attributes from tags for backwards compat. with users using legacy behavior
+    grafana_tags_as_attributes = current_app.config.get('GRAFANA_TAGS_AS_ATTRIBUTES', True)
+    grafana_tags_as_tags = current_app.config.get('GRAFANA_TAGS_AS_TAGS', False)
+
     # get values from request params
     environment = args.get('environment', current_app.config['DEFAULT_ENVIRONMENT'])
     alerting_severity = args.get('severity', 'major')
     service = args.getlist('service') or ['Grafana']
     group = args.get('group', 'Performance')
     customer = args.get('customer', None)
     origin = args.get('origin', 'Grafana')
@@ -32,16 +36,23 @@
     alerting_severity = match_tags.pop('severity', alerting_severity)
     if 'service' in match_tags:
         service.append(match_tags.pop('service'))
     group = match_tags.pop('group', group)
     customer = match_tags.pop('customer', customer)
     origin = match_tags.pop('origin', origin)
 
+    attributes = {}
+    tags = []
+
     # assign leftover match tags as attributes
-    attributes = {k.replace('.', '_'): v for (k, v) in match_tags.items()}
+    if grafana_tags_as_attributes:
+        attributes = {k.replace('.', '_'): v for (k, v) in match_tags.items()}
+    if grafana_tags_as_tags:
+        for (k, v) in match_tags.items():
+            tags.append('{}={}'.format(k, v))
 
     # get alert rule tags
     rules_tags = copy.copy(alert.get('tags') or {})
     environment = rules_tags.pop('environment', environment)
     alerting_severity = rules_tags.pop('severity', alerting_severity)
     if 'service' in rules_tags:
         service.append(rules_tags.pop('service'))
@@ -54,15 +65,19 @@
         severity = alerting_severity
     elif alert['state'] == 'ok':
         severity = alarm_model.DEFAULT_NORMAL_SEVERITY
     else:
         severity = 'indeterminate'
 
     # assign leftover rule tags as attributes
-    attributes.update({k.replace('.', '_'): v for (k, v) in rules_tags.items()})
+    if grafana_tags_as_attributes:
+        attributes.update({k.replace('.', '_'): v for (k, v) in rules_tags.items()})
+    if grafana_tags_as_tags:
+        for (k, v) in rules_tags.items():
+            tags.append('{}={}'.format(k, v))
 
     attributes['ruleId'] = str(alert['ruleId'])
     if 'ruleUrl' in alert:
         attributes['ruleUrl'] = f"<a href=\"{alert['ruleUrl']}\" target=\"_blank\">Rule</a>"
     if 'imageUrl' in alert:
         attributes['imageUrl'] = f"<a href=\"{alert['imageUrl']}\" target=\"_blank\">Image</a>"
 
@@ -71,15 +86,15 @@
         event=alert['ruleName'],
         environment=environment,
         severity=severity,
         service=service,
         group=group,
         value=f"{match['value']}",
         text=alert.get('message', None) or alert.get('title', alert['state']),
-        tags=list(),
+        tags=tags,
         attributes=attributes,
         customer=customer,
         origin=origin,
         event_type='grafanaAlert',
         timeout=timeout,
         raw_data=json.dumps(alert)
     )
```

### Comparing `alerta-server-9.0.1/alerta/webhooks/graylog.py` & `alerta-server-9.0.2/alerta/webhooks/graylog.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/newrelic.py` & `alerta-server-9.0.2/alerta/webhooks/newrelic.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/pagerduty.py` & `alerta-server-9.0.2/alerta/webhooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/pingdom.py` & `alerta-server-9.0.2/alerta/webhooks/pingdom.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/prometheus.py` & `alerta-server-9.0.2/alerta/webhooks/prometheus.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/riemann.py` & `alerta-server-9.0.2/alerta/webhooks/riemann.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/serverdensity.py` & `alerta-server-9.0.2/alerta/webhooks/serverdensity.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/slack.py` & `alerta-server-9.0.2/alerta/webhooks/slack.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/stackdriver.py` & `alerta-server-9.0.2/alerta/webhooks/stackdriver.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta/webhooks/telegram.py` & `alerta-server-9.0.2/alerta/webhooks/telegram.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/alerta_server.egg-info/PKG-INFO` & `alerta-server-9.0.2/alerta_server.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 Metadata-Version: 2.1
 Name: alerta-server
-Version: 9.0.1
+Version: 9.0.2
 Summary: Alerta server WSGI application
 Home-page: https://github.com/guardian/alerta
 Author: Nick Satterly
 Author-email: nfsatterly@gmail.com
 License: Apache License 2.0
 Keywords: alert monitoring system wsgi application api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Plugins
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: mongodb
-Provides-Extra: postgres
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: bcrypt
+Requires-Dist: blinker
+Requires-Dist: cryptography
+Requires-Dist: Flask>=2.0.1
+Requires-Dist: Flask-Compress>=1.4.0
+Requires-Dist: Flask-Cors>=3.0.2
+Requires-Dist: mohawk
+Requires-Dist: PyJWT>=2.0.0
+Requires-Dist: pyparsing
+Requires-Dist: python-dateutil
+Requires-Dist: pytz
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: requests-hawk
+Requires-Dist: sentry-sdk[flask]>=0.10.2
+Provides-Extra: mongodb
+Requires-Dist: pymongo; extra == "mongodb"
+Provides-Extra: postgres
+Requires-Dist: psycopg2; extra == "postgres"
 
-Alerta Release 9.0
+Alerta Release 9.1
 ==================
 
 [![Actions Status](https://github.com/alerta/alerta/workflows/CI%20Tests/badge.svg)](https://github.com/alerta/alerta/actions)
 [![Slack chat](https://img.shields.io/badge/chat-on%20slack-blue?logo=slack)](https://slack.alerta.dev)
 [![Coverage Status](https://coveralls.io/repos/github/alerta/alerta/badge.svg?branch=master)](https://coveralls.io/github/alerta/alerta?branch=master)
 [![Docker Pulls](https://img.shields.io/docker/pulls/alerta/alerta-web.svg)](https://hub.docker.com/r/alerta/alerta-web)
 
@@ -44,20 +61,20 @@
 ![webui](/docs/images/alerta-webui-v7.jpg?raw=true)
 
 ----
 
 Requirements
 ------------
 
-Release 9 only supports Python 3.8 or higher.
+Release 9 only supports Python 3.9 or higher.
 
 The only mandatory dependency is MongoDB or PostgreSQL. Everything else is optional.
 
-- Postgres version 11 or better
-- MongoDB version 4.4 or better
+- Postgres version 13 or better
+- MongoDB version 6.0 or better
 
 Installation
 ------------
 
 To install MongoDB on Debian/Ubuntu run:
 
     $ sudo apt-get install -y mongodb-org
```

### Comparing `alerta-server-9.0.1/alerta_server.egg-info/SOURCES.txt` & `alerta-server-9.0.2/alerta_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 VERSION
 setup.cfg
 setup.py
 wsgi.py
 alerta/__init__.py
 alerta/app.py
 alerta/app.wsgi
-alerta/build.py
 alerta/commands.py
 alerta/dev.py
 alerta/exceptions.py
 alerta/settings.py
 alerta/tasks.py
 alerta/version.py
 alerta/auth/__init__.py
```

### Comparing `alerta-server-9.0.1/alerta_server.egg-info/entry_points.txt` & `alerta-server-9.0.2/alerta_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/setup.py` & `alerta-server-9.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,18 @@
 #!/usr/bin/env python
 
 import os
-import subprocess
-from datetime import datetime
 
 import setuptools
 
 
 def read(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 
-try:
-    with open('alerta/build.py', 'w') as f:
-        build = """
-        BUILD_NUMBER = '{build_number}'
-        BUILD_DATE = '{date}'
-        BUILD_VCS_NUMBER = '{revision}'
-        """.format(
-            build_number=os.environ.get('BUILD_NUMBER', 'PROD'),
-            date=datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ'),
-            revision=subprocess.check_output(['git', 'rev-parse', 'HEAD']).decode('utf-8').strip()
-        ).replace('    ', '')
-        f.write(build)
-except Exception:
-    pass
-
 setuptools.setup(
     name='alerta-server',
     version=read('VERSION'),
     description='Alerta server WSGI application',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url='https://github.com/guardian/alerta',
@@ -51,15 +34,15 @@
         'pytz',
         'PyYAML',
         'requests',
         'requests-hawk',
         'sentry-sdk[flask]>=0.10.2',
     ],
     extras_require={
-        'mongodb': ['pymongo>=3.9.0,<4.0'],
+        'mongodb': ['pymongo'],
         'postgres': ['psycopg2']
     },
     include_package_data=True,
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'alertad = alerta.commands:cli'
@@ -95,15 +78,15 @@
         'Environment :: Web Environment',
         'Environment :: Plugins',
         'Framework :: Flask',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Telecommunications Industry',
         'License :: OSI Approved :: Apache Software License',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.8',
         'Topic :: System :: Monitoring',
     ],
-    python_requires='>=3.8'
+    python_requires='>=3.9'
 )
```

### Comparing `alerta-server-9.0.1/tests/helpers/utils.py` & `alerta-server-9.0.2/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_actions.py` & `alerta-server-9.0.2/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_aggregations.py` & `alerta-server-9.0.2/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_alerts.py` & `alerta-server-9.0.2/tests/test_alerts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_auth.py` & `alerta-server-9.0.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_authproxy.py` & `alerta-server-9.0.2/tests/test_authproxy.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_blackouts.py` & `alerta-server-9.0.2/tests/test_blackouts.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_builtins.py` & `alerta-server-9.0.2/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_commands.py` & `alerta-server-9.0.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_config.py` & `alerta-server-9.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_cors.py` & `alerta-server-9.0.2/tests/test_cors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
 from flask_cors import CORS
-from flask_cors.extension import ACL_ALLOW_HEADERS, ACL_ORIGIN
+from flask_cors.core import ACL_ALLOW_HEADERS, ACL_ORIGIN
 
 from alerta.app import create_app, db, plugins
 
 
 class HTTPCorsTestCase(unittest.TestCase):
 
     def setUp(self):
```

### Comparing `alerta-server-9.0.1/tests/test_customers.py` & `alerta-server-9.0.2/tests/test_customers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_forwarder.py` & `alerta-server-9.0.2/tests/test_forwarder.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_groups.py` & `alerta-server-9.0.2/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_heartbeats.py` & `alerta-server-9.0.2/tests/test_heartbeats.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_hooks.py` & `alerta-server-9.0.2/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_isa_18_2.py` & `alerta-server-9.0.2/tests/test_isa_18_2.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_logging.py` & `alerta-server-9.0.2/tests/test_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
         self.assertEqual(delete_blackout_request['event'], 'blackout-deleted')
         self.assertEqual(delete_blackout_request['category'], 'write')
         self.assertEqual(delete_blackout_request['resource']['type'], 'blackout')
         self.assertEqual(delete_blackout_request['request']['endpoint'], 'api.delete_blackout')
         self.assertEqual(delete_blackout_request['request']['method'], 'DELETE')
         self.assertTrue(delete_blackout_request['request']['url'].startswith('http://localhost/blackout/'))
         self.assertEqual(delete_blackout_request['request']['data'], None)
-        self.assertTrue(delete_blackout_request['request']['userAgent'].startswith('werkzeug/'))
+        self.assertTrue(delete_blackout_request['request']['userAgent'].startswith('Werkzeug/'), delete_blackout_request)
```

### Comparing `alerta-server-9.0.1/tests/test_management.py` & `alerta-server-9.0.2/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_metrics.py` & `alerta-server-9.0.2/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_notes.py` & `alerta-server-9.0.2/tests/test_notes.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_plugins.py` & `alerta-server-9.0.2/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_providers.py` & `alerta-server-9.0.2/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_queryparser.py` & `alerta-server-9.0.2/tests/test_queryparser.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_response.py` & `alerta-server-9.0.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_scopes.py` & `alerta-server-9.0.2/tests/test_scopes.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_search.py` & `alerta-server-9.0.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_severity.py` & `alerta-server-9.0.2/tests/test_severity.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_shelving.py` & `alerta-server-9.0.2/tests/test_shelving.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_tags.py` & `alerta-server-9.0.2/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_users.py` & `alerta-server-9.0.2/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_webhooks.py` & `alerta-server-9.0.2/tests/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `alerta-server-9.0.1/tests/test_zrouting.py` & `alerta-server-9.0.2/tests/test_zrouting.py`

 * *Files identical despite different names*

