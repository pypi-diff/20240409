# Comparing `tmp/vbcore-2.3.1rc0.tar.gz` & `tmp/vbcore-2.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-2.3.1rc0.tar", last modified: Fri Dec 15 01:35:20 2023, max compression
+gzip compressed data, was "vbcore-2.3.1rc1.tar", last modified: Fri Dec 15 17:35:38 2023, max compression
```

## Comparing `vbcore-2.3.1rc0.tar` & `vbcore-2.3.1rc1.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.004547 vbcore-2.3.1rc0/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      402 2023-12-15 01:35:20.004547 vbcore-2.3.1rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.978548 vbcore-2.3.1rc0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     7087 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2005 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     5906 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     2053 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-15 01:35:20.004547 vbcore-2.3.1rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4739 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.982548 vbcore-2.3.1rc0/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/aio.py
--rw-rw-rw-   0 root         (0) root         (0)     3033 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7714 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/batch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.984548 vbcore-2.3.1rc0/vbcore/brokers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3653 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)     1315 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/data.py
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/dummy.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2768 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/nats.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/brokers/publisher.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.985548 vbcore-2.3.1rc0/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1252 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/bcrypt.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/crypto/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     4571 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/csvfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.985548 vbcore-2.3.1rc0/vbcore/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.985548 vbcore-2.3.1rc0/vbcore/data/transformations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.987548 vbcore-2.3.1rc0/vbcore/data/transformations/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     5512 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/dicttoxml.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5834 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/data/transformations/builders/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.988548 vbcore-2.3.1rc0/vbcore/datastruct/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/dictionaries.py
--rw-rw-rw-   0 root         (0) root         (0)     3226 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/lazy.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/datastruct/orderer_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4312 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.990548 vbcore-2.3.1rc0/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4190 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15748 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2389 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6730 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     4439 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.990548 vbcore-2.3.1rc0/vbcore/db/schema_display/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/schema_display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13014 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/schema_display/db_diagram.py
--rw-rw-rw-   0 root         (0) root         (0)     7938 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/schema_display/model_diagram.py
--rw-rw-rw-   0 root         (0) root         (0)     3670 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5322 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/types.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/db/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.991548 vbcore-2.3.1rc0/vbcore/dictutils/
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/dictutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15749 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/dictutils/flatter_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/dictutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.991548 vbcore-2.3.1rc0/vbcore/excel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/excel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/excel/report.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3827 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/files.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/heartbeat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.993548 vbcore-2.3.1rc0/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8046 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/gql.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     6049 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1828 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.993548 vbcore-2.3.1rc0/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.994548 vbcore-2.3.1rc0/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     6964 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2955 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/lambdas.py
--rw-rw-rw-   0 root         (0) root         (0)     6977 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     5687 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.994548 vbcore-2.3.1rc0/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.995548 vbcore-2.3.1rc0/vbcore/net/ftpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/ftpclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2349 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/ftpclient/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     6110 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/ftpclient/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5325 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1552 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/net/socks_smtp.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.995548 vbcore-2.3.1rc0/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3157 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.996548 vbcore-2.3.1rc0/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     8203 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/standalone/wsgi_gunicorn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.996548 vbcore-2.3.1rc0/vbcore/stringutils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/stringutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/stringutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     2158 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/stringutils/notations.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.997547 vbcore-2.3.1rc0/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15948 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/asserter.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7333 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.998547 vbcore-2.3.1rc0/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.999548 vbcore-2.3.1rc0/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/broker.py
--rw-rw-rw-   0 root         (0) root         (0)     6114 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1114 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/entrypoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/ftpclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.999548 vbcore-2.3.1rc0/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.001547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.bumpversion.cfg
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.flake8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.001547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.git-hooks/
--rwxrwxrwx   0 root         (0) root         (0)      179 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
--rw-rw-rw-   0 root         (0) root         (0)     2205 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    16254 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.002547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.002547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/liccheck.ini
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.003547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.003547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/skel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/skel/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:20.003547 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/skel/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/skel/version.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/tools/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/types.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2853 2023-12-15 01:35:07.000000 vbcore-2.3.1rc0/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 01:35:19.983548 vbcore-2.3.1rc0/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      402 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6002 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      642 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-12-15 01:35:19.000000 vbcore-2.3.1rc0/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.987800 vbcore-2.3.1rc1/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      402 2023-12-15 17:35:38.986800 vbcore-2.3.1rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.953801 vbcore-2.3.1rc1/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     7087 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     5906 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     2053 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-15 17:35:38.987800 vbcore-2.3.1rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.958800 vbcore-2.3.1rc1/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3033 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7714 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/batch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.961800 vbcore-2.3.1rc1/vbcore/brokers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/data.py
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3919 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/nats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/brokers/publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.962800 vbcore-2.3.1rc1/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4571 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.963800 vbcore-2.3.1rc1/vbcore/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.963800 vbcore-2.3.1rc1/vbcore/data/transformations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.965800 vbcore-2.3.1rc1/vbcore/data/transformations/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5512 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/dicttoxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5834 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/data/transformations/builders/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.966800 vbcore-2.3.1rc1/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6158 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     3226 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.969800 vbcore-2.3.1rc1/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4190 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15748 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4439 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.969800 vbcore-2.3.1rc1/vbcore/db/schema_display/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/schema_display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13014 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/schema_display/db_diagram.py
+-rw-rw-rw-   0 root         (0) root         (0)     7938 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/schema_display/model_diagram.py
+-rw-rw-rw-   0 root         (0) root         (0)     3670 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5322 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/db/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.970800 vbcore-2.3.1rc1/vbcore/dictutils/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/dictutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15749 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/dictutils/flatter_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/dictutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.970800 vbcore-2.3.1rc1/vbcore/excel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/excel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/excel/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/heartbeat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.972800 vbcore-2.3.1rc1/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8046 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.973800 vbcore-2.3.1rc1/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.973800 vbcore-2.3.1rc1/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6964 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2955 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     7531 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5687 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.974800 vbcore-2.3.1rc1/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.975800 vbcore-2.3.1rc1/vbcore/net/ftpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/ftpclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2349 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/ftpclient/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/ftpclient/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5325 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1552 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/net/socks_smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.975800 vbcore-2.3.1rc1/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3157 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.976800 vbcore-2.3.1rc1/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8203 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/standalone/wsgi_gunicorn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.976800 vbcore-2.3.1rc1/vbcore/stringutils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/stringutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/stringutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/stringutils/notations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.977800 vbcore-2.3.1rc1/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15948 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7333 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.978800 vbcore-2.3.1rc1/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.980800 vbcore-2.3.1rc1/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/broker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6114 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/ftpclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.980800 vbcore-2.3.1rc1/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.983800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.flake8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.983800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.git-hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    16254 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.984800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.985800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/liccheck.ini
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.985800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.986800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/skel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/skel/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.986800 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/skel/entrypoints/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/skel/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/skel/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/tools/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2853 2023-12-15 17:35:26.000000 vbcore-2.3.1rc1/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 17:35:38.960801 vbcore-2.3.1rc1/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      642 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-12-15 17:35:38.000000 vbcore-2.3.1rc1/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-2.3.1rc0/requirements/requirements-all.txt` & `vbcore-2.3.1rc1/requirements/requirements-all.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-build.txt` & `vbcore-2.3.1rc1/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-crypto.txt` & `vbcore-2.3.1rc1/requirements/requirements-crypto.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-db.txt` & `vbcore-2.3.1rc1/requirements/requirements-db.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-dev.txt` & `vbcore-2.3.1rc1/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-extra.txt` & `vbcore-2.3.1rc1/requirements/requirements-extra.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-http.txt` & `vbcore-2.3.1rc1/requirements/requirements-http.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-net.txt` & `vbcore-2.3.1rc1/requirements/requirements-net.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements-test.txt` & `vbcore-2.3.1rc1/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/requirements/requirements.txt` & `vbcore-2.3.1rc1/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/setup.py` & `vbcore-2.3.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/aio.py` & `vbcore-2.3.1rc1/vbcore/aio.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/base.py` & `vbcore-2.3.1rc1/vbcore/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/batch.py` & `vbcore-2.3.1rc1/vbcore/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/brokers/base.py` & `vbcore-2.3.1rc1/vbcore/brokers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,17 @@
         self.log.info("successfully subscribed: topic=%s callback=%s", topic, callback)
 
     def wrap_message(self, callback: Callback) -> Callback:
         @functools.wraps(callback)
         async def decorator(data: Any) -> None:
             self.log.debug("received event: %s", data)
             message = self._wrap_message(data)
-            self.context.set(**message.headers.to_dict())
+            if message.headers:
+                self.context.set(**message.headers.to_dict())
+
             await self.pre_callback_hook()
             await callback(message)
             await self.post_callback_hook()
 
         return decorator
 
     def acknowledge(self, callback: Callback) -> Callback:
```

### Comparing `vbcore-2.3.1rc0/vbcore/brokers/consumer.py` & `vbcore-2.3.1rc1/vbcore/brokers/consumer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/brokers/data.py` & `vbcore-2.3.1rc1/vbcore/brokers/data.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/brokers/dummy.py` & `vbcore-2.3.1rc1/vbcore/brokers/dummy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/brokers/factory.py` & `vbcore-2.3.1rc1/vbcore/brokers/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/brokers/nats.py` & `vbcore-2.3.1rc1/vbcore/brokers/publisher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,66 @@
-from collections.abc import AsyncIterator
-from contextlib import asynccontextmanager
-from dataclasses import dataclass
-from typing import Any, Awaitable, Callable, cast, Optional
-
-from nats import NATS
-from nats.aio.msg import Msg
-from nats.errors import (
-    ConnectionClosedError,
-    NoServersError,
-    TimeoutError as NatsTimeoutError,
-)
-from nats.js import JetStreamContext
-from typing_extensions import Self
-
-from vbcore.types import OptStr
-
-from .base import BrokerClient, Callback
-from .data import BrokerOptions, Header, Message
-
-
-@dataclass(frozen=True, kw_only=True)
-class NatsOptions(BrokerOptions):
-    consumer_group: OptStr = None
-    nack_delay: int = 30
-
-
-class NatsBrokerAdapter(BrokerClient[NATS, NatsOptions]):
-    retryable_errors = (
-        ConnectionClosedError,
-        NatsTimeoutError,
-        NoServersError,
-    )
-
-    def instance(self) -> NATS:
-        return NATS()
-
-    @property
-    def stream(self) -> JetStreamContext:
-        return self.client.jetstream()
-
-    @asynccontextmanager
-    async def connect(self) -> AsyncIterator[Self]:
-        # force to list because nats-py raise error
-        servers = list(self.options.servers)
-        await self.client.connect(servers, connect_timeout=int(self.options.timeout))
-        try:
-            yield self
-        finally:
-            await self.client.close()
-
-    def _wrap_message(self, message: Msg) -> Message:
-        return Message(
-            topic=message.subject,
-            data=message.data,
-            reply=message.reply,
-            headers=Header.from_dict(**message.headers) if message.headers else None,
-        )
+from abc import ABC
+from typing import Callable, ClassVar, List, Optional, Type, Union
 
-    async def _publish(
-        self, topic: str, message: Any, headers: Optional[Header] = None, **kwargs
-    ) -> None:
-        await self.stream.publish(
-            subject=topic,
-            payload=message,
-            timeout=self.options.timeout,
-            headers=headers.to_dict() if headers else None,  # type: ignore
-            **kwargs,
-        )
+import backoff
+from pydantic import BaseModel
+
+from vbcore import json
+from vbcore.loggers import VBLoggerMixin
 
-    async def _subscribe(self, topic: str, callback: Callback, **kwargs) -> None:
-        queue = None
-        if self.options.consumer_group:
-            queue = f"{self.options.consumer_group}_{topic.replace('.', '-')}"
-
-        _callback = cast(Optional[Callable[[Msg], Awaitable[None]]], callback)
-        await self.stream.subscribe(subject=topic, queue=queue, cb=_callback, **kwargs)
-
-    async def _nak_on_failure(self, message: Msg) -> None:
-        await message.nak(self.options.nack_delay)
-        self.log.error(
-            "nack sent on reply %s and delayed for %ss", message.reply, self.options.nack_delay
+from .base import BrokerClient
+from .data import Header
+
+
+class EventModel(ABC, BaseModel):
+    TOPIC: ClassVar[str]
+
+
+class Publisher(VBLoggerMixin):
+    def __init__(
+        self,
+        broker: BrokerClient,
+        backoff_enabled: bool = True,
+        retryable_errors: Optional[List[Type[Exception]]] = None,
+        max_tries: int = 3,
+    ):
+        self.broker = broker
+        self.backoff_enabled = backoff_enabled
+        self.retryable_errors = retryable_errors or [Exception]
+        self.max_tries = max_tries
+
+    def backoff_wrapper(self, func: Callable) -> Callable:
+        decorator = backoff.on_exception(
+            backoff.expo,
+            logger=self.log,
+            exception=self.retryable_errors,
+            max_tries=self.max_tries,
         )
+        return decorator(func)
+
+    async def publish(
+        self, message: EventModel, headers: Optional[Header] = None, **kwargs
+    ) -> None:
+        async def _publish() -> None:
+            async with self.broker.connect() as client:
+                data = message.model_dump_json().encode()
+                await client.publish(
+                    topic=message.TOPIC, message=data, headers=headers or Header(), **kwargs
+                )
+
+        wrapper = self.backoff_wrapper(_publish) if self.backoff_enabled else _publish
+        await wrapper()  # type: ignore
+
+    async def raw_publish(
+        self,
+        topic: str,
+        message: Union[bytes, str, dict],
+        headers: Optional[Header] = None,
+        **kwargs,
+    ) -> None:
+        async with self.broker.connect() as client:
+            if isinstance(message, dict):
+                message = json.dumps(message).encode()
+            elif isinstance(message, str):
+                message = message.encode()
 
-    async def _ack_on_success(self, message: Msg) -> None:
-        await message.ack()
-        self.log.debug("ack sent on reply %s", message.reply)
+            await client.publish(topic, message, headers, **kwargs)
```

### Comparing `vbcore-2.3.1rc0/vbcore/configurator.py` & `vbcore-2.3.1rc1/vbcore/configurator.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/context.py` & `vbcore-2.3.1rc1/vbcore/context.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/crypto/argon.py` & `vbcore-2.3.1rc1/vbcore/crypto/argon.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/crypto/base.py` & `vbcore-2.3.1rc1/vbcore/crypto/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/crypto/bcrypt.py` & `vbcore-2.3.1rc1/vbcore/crypto/bcrypt.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/crypto/factory.py` & `vbcore-2.3.1rc1/vbcore/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/crypto/hashes.py` & `vbcore-2.3.1rc1/vbcore/crypto/hashes.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/csvfile.py` & `vbcore-2.3.1rc1/vbcore/csvfile.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/base.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/csv.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/csv.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/dicttoxml.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/dicttoxml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/factory.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/html.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/html.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/json.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/xml.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/xml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/data/transformations/builders/yaml.py` & `vbcore-2.3.1rc1/vbcore/data/transformations/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/datastruct/buffer.py` & `vbcore-2.3.1rc1/vbcore/datastruct/buffer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/datastruct/cache.py` & `vbcore-2.3.1rc1/vbcore/datastruct/cache.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/datastruct/dictionaries.py` & `vbcore-2.3.1rc1/vbcore/datastruct/dictionaries.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/datastruct/lazy.py` & `vbcore-2.3.1rc1/vbcore/datastruct/lazy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/datastruct/orderer_set.py` & `vbcore-2.3.1rc1/vbcore/datastruct/orderer_set.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/date_helper.py` & `vbcore-2.3.1rc1/vbcore/date_helper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/base.py` & `vbcore-2.3.1rc1/vbcore/db/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/events.py` & `vbcore-2.3.1rc1/vbcore/db/events.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/exceptions.py` & `vbcore-2.3.1rc1/vbcore/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/listener.py` & `vbcore-2.3.1rc1/vbcore/db/listener.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/mixins.py` & `vbcore-2.3.1rc1/vbcore/db/mixins.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/mysql_dumper.py` & `vbcore-2.3.1rc1/vbcore/db/mysql_dumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/repo.py` & `vbcore-2.3.1rc1/vbcore/db/repo.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/schema.py` & `vbcore-2.3.1rc1/vbcore/db/schema.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/schema_display/db_diagram.py` & `vbcore-2.3.1rc1/vbcore/db/schema_display/db_diagram.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/schema_display/model_diagram.py` & `vbcore-2.3.1rc1/vbcore/db/schema_display/model_diagram.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/sqla.py` & `vbcore-2.3.1rc1/vbcore/db/sqla.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/support.py` & `vbcore-2.3.1rc1/vbcore/db/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/types.py` & `vbcore-2.3.1rc1/vbcore/db/types.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/db/views.py` & `vbcore-2.3.1rc1/vbcore/db/views.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/dictutils/flatter_dict.py` & `vbcore-2.3.1rc1/vbcore/dictutils/flatter_dict.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/dispatcher.py` & `vbcore-2.3.1rc1/vbcore/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/enums.py` & `vbcore-2.3.1rc1/vbcore/enums.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/excel/report.py` & `vbcore-2.3.1rc1/vbcore/excel/report.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/exceptions.py` & `vbcore-2.3.1rc1/vbcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/factory.py` & `vbcore-2.3.1rc1/vbcore/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/files.py` & `vbcore-2.3.1rc1/vbcore/files.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/heartbeat.py` & `vbcore-2.3.1rc1/vbcore/heartbeat.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/batch.py` & `vbcore-2.3.1rc1/vbcore/http/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/client.py` & `vbcore-2.3.1rc1/vbcore/http/client.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/gql.py` & `vbcore-2.3.1rc1/vbcore/http/gql.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/headers.py` & `vbcore-2.3.1rc1/vbcore/http/headers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/httpcode.py` & `vbcore-2.3.1rc1/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/httpdumper.py` & `vbcore-2.3.1rc1/vbcore/http/httpdumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/proxy.py` & `vbcore-2.3.1rc1/vbcore/http/proxy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/rpc.py` & `vbcore-2.3.1rc1/vbcore/http/rpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/http/useragent.py` & `vbcore-2.3.1rc1/vbcore/http/useragent.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/importer.py` & `vbcore-2.3.1rc1/vbcore/importer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/json.py` & `vbcore-2.3.1rc1/vbcore/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.3.1rc1/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/jsonschema/support.py` & `vbcore-2.3.1rc1/vbcore/jsonschema/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/lambdas.py` & `vbcore-2.3.1rc1/vbcore/lambdas.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/loggers.py` & `vbcore-2.3.1rc1/vbcore/loggers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging.config
 import os
 import socket
 import struct
 import typing as t
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
 from functools import cached_property
 
 from vbcore import json
 from vbcore.base import Decorator, Static
 from vbcore.context import ContextCorrelationId, ContextMetadata
 from vbcore.datastruct.lazy import ClassDumper
@@ -54,22 +54,25 @@
     logging.root = root_logger
 
     logging.captureWarnings(os.environ.get("LOG_CAPTURE_WARNING", True))
 
 
 @dataclass(frozen=True, kw_only=True)
 class LoggingSettings:
-    level: str = "INFO"
-    force: bool = True
-    config_file: OptStr = None
-    listen_for_reload: bool = False
-    listener_daemon: bool = True
-    listener_port: int = DEFAULT_LISTENER_PORT
-    default_date_format = "%Y-%m-%d %H:%M:%S"
-    default_format: str = "%(asctime)s.%(msecs)03d | %(levelname)-8s | %(name)s | %(message)s"
+    level: str = field(default="INFO")
+    force: bool = field(default=True)
+    config_file: OptStr = field(default=None)
+    listen_for_reload: bool = field(default=False)
+    listener_daemon: bool = field(default=True)
+    listener_port: int = field(default=DEFAULT_LISTENER_PORT)
+    default_date_format: str = field(default="%Y-%m-%d %H:%M:%S")
+    default_format: str = field(
+        default="%(asctime)s.%(msecs)03d | %(levelname)-8s | %(name)s | %(message)s"
+    )
+    logger_levels: t.Dict[str, str] = field(default_factory=dict)
 
 
 class LogContextFilter(logging.Filter):
     _metadata: t.Type[ContextMetadata] = ContextCorrelationId
 
     def __init__(
         self,
@@ -83,53 +86,62 @@
 
     def filter(self, record: logging.LogRecord) -> bool:
         try:
             metadata: t.Any = self._metadata.get()
         except LookupError:
             metadata = object()
 
-        for field in self.fields:
-            value = getattr(metadata, field, None)
-            setattr(record, field, value or self.default)
+        for _field in self.fields:
+            value = getattr(metadata, _field, None)
+            setattr(record, _field, value or self.default)
 
         return True
 
 
 class SetupLoggers:
     def __init__(
         self,
         config: t.Optional[LoggingSettings] = None,
         config_file: OptStr = None,
         context_filter: t.Optional[LogContextFilter] = None,
         **kwargs,
     ):
         self.config = config or LoggingSettings()
-        self.context_filter = context_filter
         self.config_file = config_file or self.config.config_file
+        self.context_filter = context_filter
 
         if not self.prepare_file_config():
             self.prepare_basic_config(**kwargs)
 
         if self.config.listen_for_reload:
             self.prepare_listener()
 
+    @classmethod
+    def set_logger_levels(cls, logger_levels: t.Dict[str, str]) -> None:
+        """
+        It is a class method because we want the possibilities
+        to call this method anyway at anypoint
+        """
+        for name, level in logger_levels.items():
+            logging.getLogger(name).setLevel(level)
+
     def prepare_basic_config(self, **kwargs):
         kwargs.setdefault("force", self.config.force)
         kwargs.setdefault("level", self.config.level)
         kwargs.setdefault("format", self.config.default_format)
         kwargs.setdefault("datefmt", self.config.default_date_format)
         kwargs["level"] = os.environ.get("LOG_LEVEL") or self.config.level
 
         if self.context_filter:
             handler = logging.StreamHandler()
             handler.addFilter(self.context_filter)
-            handlers = kwargs.get("handlers") or []
-            handlers.append(handler)
+            kwargs["handlers"] = [handler]
 
         logging.basicConfig(**kwargs)
+        self.set_logger_levels(self.config.logger_levels)
 
     def prepare_file_config(self) -> bool:
         config_file = os.environ.get("LOG_FILE_CONFIG") or self.config_file
         if not config_file:
             return False
 
         with FileHandler(config_file).open() as file:
```

### Comparing `vbcore-2.3.1rc0/vbcore/misc.py` & `vbcore-2.3.1rc1/vbcore/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/net/ftpclient/legacy.py` & `vbcore-2.3.1rc1/vbcore/net/ftpclient/legacy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/net/ftpclient/sftp.py` & `vbcore-2.3.1rc1/vbcore/net/ftpclient/sftp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/net/helpers.py` & `vbcore-2.3.1rc1/vbcore/net/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/net/sendmail.py` & `vbcore-2.3.1rc1/vbcore/net/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/net/socks_smtp.py` & `vbcore-2.3.1rc1/vbcore/net/socks_smtp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/rule_engine/base.py` & `vbcore-2.3.1rc1/vbcore/rule_engine/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/rule_engine/engine.py` & `vbcore-2.3.1rc1/vbcore/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/standalone/scheduler.py` & `vbcore-2.3.1rc1/vbcore/standalone/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.3.1rc1/vbcore/standalone/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/stringutils/misc.py` & `vbcore-2.3.1rc1/vbcore/stringutils/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/stringutils/notations.py` & `vbcore-2.3.1rc1/vbcore/stringutils/notations.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/system.py` & `vbcore-2.3.1rc1/vbcore/system.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tester/asserter.py` & `vbcore-2.3.1rc1/vbcore/tester/asserter.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tester/fetchmail.py` & `vbcore-2.3.1rc1/vbcore/tester/fetchmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tester/helpers.py` & `vbcore-2.3.1rc1/vbcore/tester/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tester/http.py` & `vbcore-2.3.1rc1/vbcore/tester/http.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/broker.py` & `vbcore-2.3.1rc1/vbcore/tools/broker.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/cli.py` & `vbcore-2.3.1rc1/vbcore/tools/cli.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/crypto.py` & `vbcore-2.3.1rc1/vbcore/tools/crypto.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/database.py` & `vbcore-2.3.1rc1/vbcore/tools/database.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/entrypoint.py` & `vbcore-2.3.1rc1/vbcore/tools/entrypoint.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/ftpclient.py` & `vbcore-2.3.1rc1/vbcore/tools/ftpclient.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/init.py` & `vbcore-2.3.1rc1/vbcore/tools/initializer/init.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.gitignore` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.gitignore`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/.pylintrc` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/.pylintrc`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/Makefile` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/README.md` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/README.md`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/liccheck.ini` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/liccheck.ini`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/initializer/skeleton/setup.py` & `vbcore-2.3.1rc1/vbcore/tools/initializer/skeleton/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/scheduler.py` & `vbcore-2.3.1rc1/vbcore/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/sendmail.py` & `vbcore-2.3.1rc1/vbcore/tools/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/tools/wsgi_gunicorn.py` & `vbcore-2.3.1rc1/vbcore/tools/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/types.py` & `vbcore-2.3.1rc1/vbcore/types.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore/yaml.py` & `vbcore-2.3.1rc1/vbcore/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore.egg-info/SOURCES.txt` & `vbcore-2.3.1rc1/vbcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.3.1rc0/vbcore.egg-info/requires.txt` & `vbcore-2.3.1rc1/vbcore.egg-info/requires.txt`

 * *Files identical despite different names*

