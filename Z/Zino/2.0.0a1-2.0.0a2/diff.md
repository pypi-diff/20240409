# Comparing `tmp/Zino-2.0.0a1.tar.gz` & `tmp/Zino-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Zino-2.0.0a1.tar", last modified: Fri Jan 26 09:35:24 2024, max compression
+gzip compressed data, was "Zino-2.0.0a2.tar", last modified: Tue Apr  9 10:39:52 2024, max compression
```

## Comparing `Zino-2.0.0a1.tar` & `Zino-2.0.0a2.tar`

### file list

```diff
@@ -1,150 +1,155 @@
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.706282 Zino-2.0.0a1/
--rw-r--r--   0 mvold     (1346) users      (100)       92 2023-06-15 13:00:29.000000 Zino-2.0.0a1/.codecov.yml
--rw-r--r--   0 mvold     (1346) users      (100)      416 2023-02-23 15:30:20.000000 Zino-2.0.0a1/.editorconfig
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.693282 Zino-2.0.0a1/.github/
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.695282 Zino-2.0.0a1/.github/workflows/
--rw-r--r--   0 mvold     (1346) users      (100)     2056 2023-08-09 09:50:27.000000 Zino-2.0.0a1/.github/workflows/linter.yml
--rw-r--r--   0 mvold     (1346) users      (100)     1054 2023-05-11 13:12:56.000000 Zino-2.0.0a1/.github/workflows/publish-test-results.yml
--rw-r--r--   0 mvold     (1346) users      (100)     1678 2023-11-28 10:39:04.000000 Zino-2.0.0a1/.github/workflows/tests.yml
--rw-r--r--   0 mvold     (1346) users      (100)      267 2023-08-17 12:44:13.000000 Zino-2.0.0a1/.gitignore
--rw-r--r--   0 mvold     (1346) users      (100)      539 2023-08-09 09:50:27.000000 Zino-2.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 mvold     (1346) users      (100)      356 2023-11-28 10:39:04.000000 Zino-2.0.0a1/.sonarcloud.properties
--rw-r--r--   0 mvold     (1346) users      (100)      506 2024-01-26 09:26:00.000000 Zino-2.0.0a1/AUTHORS.md
--rw-r--r--   0 mvold     (1346) users      (100)      452 2024-01-26 09:19:03.000000 Zino-2.0.0a1/CHANGELOG.md
--rw-r--r--   0 mvold     (1346) users      (100)    11358 2023-03-29 12:53:35.000000 Zino-2.0.0a1/LICENSE
--rw-r--r--   0 mvold     (1346) users      (100)      170 2024-01-26 09:19:03.000000 Zino-2.0.0a1/NOTICE
--rw-r--r--   0 mvold     (1346) users      (100)    23198 2024-01-26 09:35:24.706282 Zino-2.0.0a1/PKG-INFO
--rw-r--r--   0 mvold     (1346) users      (100)     8584 2024-01-26 09:26:00.000000 Zino-2.0.0a1/README.md
--rw-r--r--   0 mvold     (1346) users      (100)     1274 2024-01-25 10:26:46.000000 Zino-2.0.0a1/polldevs.cf.example
--rw-r--r--   0 mvold     (1346) users      (100)     2381 2024-01-26 09:31:36.000000 Zino-2.0.0a1/pyproject.toml
--rw-r--r--   0 mvold     (1346) users      (100)       38 2024-01-26 09:35:24.707282 Zino-2.0.0a1/setup.cfg
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.693282 Zino-2.0.0a1/src/
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.705282 Zino-2.0.0a1/src/Zino.egg-info/
--rw-r--r--   0 mvold     (1346) users      (100)    23198 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/Zino.egg-info/PKG-INFO
--rw-r--r--   0 mvold     (1346) users      (100)     4040 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/Zino.egg-info/SOURCES.txt
--rw-r--r--   0 mvold     (1346) users      (100)        1 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/Zino.egg-info/dependency_links.txt
--rw-r--r--   0 mvold     (1346) users      (100)       40 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/Zino.egg-info/entry_points.txt
--rw-r--r--   0 mvold     (1346) users      (100)        1 2024-01-18 09:45:52.000000 Zino-2.0.0a1/src/Zino.egg-info/not-zip-safe
--rw-r--r--   0 mvold     (1346) users      (100)      197 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/Zino.egg-info/requires.txt
--rw-r--r--   0 mvold     (1346) users      (100)        5 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/Zino.egg-info/top_level.txt
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.696282 Zino-2.0.0a1/src/zino/
--rw-r--r--   0 mvold     (1346) users      (100)       13 2023-02-23 15:30:20.000000 Zino-2.0.0a1/src/zino/__init__.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.697282 Zino-2.0.0a1/src/zino/api/
--rw-r--r--   0 mvold     (1346) users      (100)        0 2023-10-20 10:30:51.000000 Zino-2.0.0a1/src/zino/api/__init__.py
--rw-r--r--   0 mvold     (1346) users      (100)     2232 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/api/auth.py
--rw-r--r--   0 mvold     (1346) users      (100)    15222 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/api/legacy.py
--rw-r--r--   0 mvold     (1346) users      (100)     4830 2024-01-25 08:44:34.000000 Zino-2.0.0a1/src/zino/api/notify.py
--rw-r--r--   0 mvold     (1346) users      (100)     2015 2024-01-25 08:44:34.000000 Zino-2.0.0a1/src/zino/api/server.py
--rw-r--r--   0 mvold     (1346) users      (100)      459 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/compat.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.697282 Zino-2.0.0a1/src/zino/config/
--rw-r--r--   0 mvold     (1346) users      (100)        0 2023-02-23 15:30:20.000000 Zino-2.0.0a1/src/zino/config/__init__.py
--rw-r--r--   0 mvold     (1346) users      (100)      838 2023-10-11 11:18:48.000000 Zino-2.0.0a1/src/zino/config/models.py
--rw-r--r--   0 mvold     (1346) users      (100)     1776 2023-10-11 11:12:54.000000 Zino-2.0.0a1/src/zino/config/polldevs.py
--rw-r--r--   0 mvold     (1346) users      (100)     5928 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/events.py
--rw-r--r--   0 mvold     (1346) users      (100)     1107 2023-11-03 08:36:03.000000 Zino-2.0.0a1/src/zino/getuptime.py
--rw-r--r--   0 mvold     (1346) users      (100)     1179 2023-11-03 08:35:54.000000 Zino-2.0.0a1/src/zino/getyellowalarms.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.699282 Zino-2.0.0a1/src/zino/mibdumps/
--rw-r--r--   0 mvold     (1346) users      (100)    31051 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/BFD-STD-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)     5601 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/BFD-TC-STD-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)    43401 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/mibdumps/BGP4-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)   152115 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/mibdumps/BGP4-V2-MIB-JUNIPER.py
--rw-r--r--   0 mvold     (1346) users      (100)    84335 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/mibdumps/CISCO-BGP4-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)    42882 2024-01-17 12:52:21.000000 Zino-2.0.0a1/src/zino/mibdumps/CISCO-IETF-BFD-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)    21764 2024-01-17 12:52:21.000000 Zino-2.0.0a1/src/zino/mibdumps/CISCO-SMI.py
--rw-r--r--   0 mvold     (1346) users      (100)     3486 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/DIFFSERV-DSCP-TC.py
--rw-r--r--   0 mvold     (1346) users      (100)   113815 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/DIFFSERV-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)     8117 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/IANA-BFD-TC-STD-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)     9735 2023-10-03 09:59:34.000000 Zino-2.0.0a1/src/zino/mibdumps/IANAifType-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)    25451 2023-10-03 11:23:11.000000 Zino-2.0.0a1/src/zino/mibdumps/IF-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)    25613 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/INTEGRATED-SERVICES-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)   184120 2024-01-23 13:56:40.000000 Zino-2.0.0a1/src/zino/mibdumps/IP-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)     4117 2023-08-18 09:06:29.000000 Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-ALARM-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)     8047 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-BFD-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)     5301 2023-11-28 10:39:04.000000 Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-EXPERIMENT-MIB.py
--rw-r--r--   0 mvold     (1346) users      (100)    11653 2023-08-09 09:50:27.000000 Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-SMI.py
--rw-r--r--   0 mvold     (1346) users      (100)     1671 2023-10-03 12:46:19.000000 Zino-2.0.0a1/src/zino/oid.py
--rw-r--r--   0 mvold     (1346) users      (100)     2465 2023-10-11 10:42:06.000000 Zino-2.0.0a1/src/zino/polltest.py
--rw-r--r--   0 mvold     (1346) users      (100)     3144 2023-10-11 10:39:54.000000 Zino-2.0.0a1/src/zino/scheduler.py
--rw-r--r--   0 mvold     (1346) users      (100)    19200 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/snmp.py
--rw-r--r--   0 mvold     (1346) users      (100)     1938 2024-01-23 13:56:40.000000 Zino-2.0.0a1/src/zino/state.py
--rw-r--r--   0 mvold     (1346) users      (100)    10429 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/statemodels.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.700282 Zino-2.0.0a1/src/zino/tasks/
--rw-r--r--   0 mvold     (1346) users      (100)     1032 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/tasks/__init__.py
--rw-r--r--   0 mvold     (1346) users      (100)     3289 2024-01-23 13:56:40.000000 Zino-2.0.0a1/src/zino/tasks/addrs.py
--rw-r--r--   0 mvold     (1346) users      (100)     6278 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/bfdtask.py
--rw-r--r--   0 mvold     (1346) users      (100)    15183 2024-01-26 09:26:00.000000 Zino-2.0.0a1/src/zino/tasks/bgpstatemonitortask.py
--rw-r--r--   0 mvold     (1346) users      (100)       50 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/errors.py
--rw-r--r--   0 mvold     (1346) users      (100)     2741 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/juniperalarmtask.py
--rw-r--r--   0 mvold     (1346) users      (100)     7352 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/linkstatetask.py
--rw-r--r--   0 mvold     (1346) users      (100)     2827 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/reachabletask.py
--rw-r--r--   0 mvold     (1346) users      (100)      778 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/task.py
--rw-r--r--   0 mvold     (1346) users      (100)     1150 2024-01-25 07:41:54.000000 Zino-2.0.0a1/src/zino/tasks/vendor.py
--rw-r--r--   0 mvold     (1346) users      (100)      206 2023-05-11 13:12:56.000000 Zino-2.0.0a1/src/zino/time.py
--rw-r--r--   0 mvold     (1346) users      (100)      413 2024-01-26 09:35:24.000000 Zino-2.0.0a1/src/zino/version.py
--rw-r--r--   0 mvold     (1346) users      (100)     3301 2024-01-25 08:44:34.000000 Zino-2.0.0a1/src/zino/zino.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.701282 Zino-2.0.0a1/tests/
--rw-r--r--   0 mvold     (1346) users      (100)        0 2023-02-23 15:30:20.000000 Zino-2.0.0a1/tests/__init__.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.701282 Zino-2.0.0a1/tests/api/
--rw-r--r--   0 mvold     (1346) users      (100)        0 2023-10-20 10:30:51.000000 Zino-2.0.0a1/tests/api/__init__.py
--rw-r--r--   0 mvold     (1346) users      (100)     2764 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/api/auth_test.py
--rw-r--r--   0 mvold     (1346) users      (100)      764 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/api/conftest.py
--rw-r--r--   0 mvold     (1346) users      (100)    27319 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/api/legacy_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     5641 2024-01-25 08:44:34.000000 Zino-2.0.0a1/tests/api/notify_test.py
--rw-r--r--   0 mvold     (1346) users      (100)      265 2024-01-25 08:44:34.000000 Zino-2.0.0a1/tests/api/server_test.py
--rw-r--r--   0 mvold     (1346) users      (100)      638 2023-06-15 13:00:29.000000 Zino-2.0.0a1/tests/bin_test.py
--rw-r--r--   0 mvold     (1346) users      (100)      581 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/compat_test.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.701282 Zino-2.0.0a1/tests/config/
--rw-r--r--   0 mvold     (1346) users      (100)        0 2023-02-23 15:31:31.000000 Zino-2.0.0a1/tests/config/__init__.py
--rw-r--r--   0 mvold     (1346) users      (100)      369 2023-02-23 15:31:31.000000 Zino-2.0.0a1/tests/config/models_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     2745 2023-10-11 11:53:13.000000 Zino-2.0.0a1/tests/config/polldevs_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     3856 2024-01-23 13:56:40.000000 Zino-2.0.0a1/tests/conftest.py
--rw-r--r--   0 mvold     (1346) users      (100)     4543 2024-01-23 13:56:40.000000 Zino-2.0.0a1/tests/events_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     1136 2023-08-09 09:50:27.000000 Zino-2.0.0a1/tests/oid_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     2590 2023-06-21 10:34:41.000000 Zino-2.0.0a1/tests/scheduler_test.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.704282 Zino-2.0.0a1/tests/snmp_fixtures/
--rw-r--r--   0 mvold     (1346) users      (100)      285 2024-01-17 12:52:21.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bfd-up.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      375 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bgp-admin-down.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      375 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bgp-admin-up.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      371 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bgp-external-reset.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      371 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bgp-oper-down-short.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      375 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bgp-oper-down.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      343 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/cisco-bgp.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/general-bgp-admin-down.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/general-bgp-admin-up.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      373 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/general-bgp-external-reset.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      373 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/general-bgp-oper-down-short.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/general-bgp-oper-down.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/general-bgp.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      287 2024-01-23 13:56:40.000000 Zino-2.0.0a1/tests/snmp_fixtures/ip-ad-ent-addr.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)       71 2023-08-09 09:50:27.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-alarm-wrong.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)       68 2023-09-11 13:32:27.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-alarm-zero.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)       68 2023-09-11 13:32:27.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-alarm.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      867 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bfd-up.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      551 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-admin-down.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      550 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-admin-up.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      547 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-external-reset.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      547 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-oper-down-short.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      551 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-oper-down.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      551 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)     2948 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/snmp_fixtures/linksdown.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)     2948 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/snmp_fixtures/linksup.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)      180 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/missing-info-bgp.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)    42180 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_fixtures/public.snmprec
--rw-r--r--   0 mvold     (1346) users      (100)     9697 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/snmp_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     2404 2024-01-17 11:17:17.000000 Zino-2.0.0a1/tests/state_test.py
--rw-r--r--   0 mvold     (1346) users      (100)     5334 2024-01-25 08:44:34.000000 Zino-2.0.0a1/tests/statemodels_test.py
-drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-01-26 09:35:24.705282 Zino-2.0.0a1/tests/tasks/
--rw-r--r--   0 mvold     (1346) users      (100)        0 2023-06-15 13:00:29.000000 Zino-2.0.0a1/tests/tasks/__init__.py
--rw-r--r--   0 mvold     (1346) users      (100)      800 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/conftest.py
--rw-r--r--   0 mvold     (1346) users      (100)     3014 2024-01-23 13:56:40.000000 Zino-2.0.0a1/tests/tasks/test_addrs.py
--rw-r--r--   0 mvold     (1346) users      (100)     5027 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/test_bfdtask.py
--rw-r--r--   0 mvold     (1346) users      (100)    14218 2024-01-26 09:26:00.000000 Zino-2.0.0a1/tests/tasks/test_bgpstatemonitortask.py
--rw-r--r--   0 mvold     (1346) users      (100)      164 2023-11-28 10:39:04.000000 Zino-2.0.0a1/tests/tasks/test_init.py
--rw-r--r--   0 mvold     (1346) users      (100)     6425 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/test_juniperalarmtask.py
--rw-r--r--   0 mvold     (1346) users      (100)     5481 2024-01-17 11:26:31.000000 Zino-2.0.0a1/tests/tasks/test_linkstatetask.py
--rw-r--r--   0 mvold     (1346) users      (100)     3353 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/test_reachabletask.py
--rw-r--r--   0 mvold     (1346) users      (100)     1819 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/test_run_all_tasks.py
--rw-r--r--   0 mvold     (1346) users      (100)     1063 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/test_task.py
--rw-r--r--   0 mvold     (1346) users      (100)     1173 2024-01-25 07:41:54.000000 Zino-2.0.0a1/tests/tasks/test_vendor.py
--rw-r--r--   0 mvold     (1346) users      (100)     1857 2024-01-23 13:56:40.000000 Zino-2.0.0a1/tests/zino_test.py
--rw-r--r--   0 mvold     (1346) users      (100)      646 2024-01-25 08:44:34.000000 Zino-2.0.0a1/tox.ini
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.853507 Zino-2.0.0a2/
+-rw-r--r--   0 mvold     (1346) users      (100)       92 2023-06-15 13:00:29.000000 Zino-2.0.0a2/.codecov.yml
+-rw-r--r--   0 mvold     (1346) users      (100)      416 2023-02-23 15:30:20.000000 Zino-2.0.0a2/.editorconfig
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.823505 Zino-2.0.0a2/.github/
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.825505 Zino-2.0.0a2/.github/workflows/
+-rw-r--r--   0 mvold     (1346) users      (100)     2284 2024-04-09 10:37:24.000000 Zino-2.0.0a2/.github/workflows/linter.yml
+-rw-r--r--   0 mvold     (1346) users      (100)     1096 2024-04-09 10:37:24.000000 Zino-2.0.0a2/.github/workflows/publish-test-results.yml
+-rw-r--r--   0 mvold     (1346) users      (100)     1739 2024-04-09 10:37:24.000000 Zino-2.0.0a2/.github/workflows/tests.yml
+-rw-r--r--   0 mvold     (1346) users      (100)      279 2024-04-09 10:37:24.000000 Zino-2.0.0a2/.gitignore
+-rw-r--r--   0 mvold     (1346) users      (100)      538 2024-04-09 10:37:24.000000 Zino-2.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 mvold     (1346) users      (100)      356 2023-11-28 10:39:04.000000 Zino-2.0.0a2/.sonarcloud.properties
+-rw-r--r--   0 mvold     (1346) users      (100)      506 2024-01-26 09:26:00.000000 Zino-2.0.0a2/AUTHORS.md
+-rw-r--r--   0 mvold     (1346) users      (100)     2117 2024-04-09 10:37:49.000000 Zino-2.0.0a2/CHANGELOG.md
+-rw-r--r--   0 mvold     (1346) users      (100)    11358 2023-03-29 12:53:35.000000 Zino-2.0.0a2/LICENSE
+-rw-r--r--   0 mvold     (1346) users      (100)      170 2024-01-26 09:19:03.000000 Zino-2.0.0a2/NOTICE
+-rw-r--r--   0 mvold     (1346) users      (100)    25009 2024-04-09 10:39:52.853507 Zino-2.0.0a2/PKG-INFO
+-rw-r--r--   0 mvold     (1346) users      (100)    10395 2024-04-09 10:37:24.000000 Zino-2.0.0a2/README.md
+-rw-r--r--   0 mvold     (1346) users      (100)     1185 2024-04-09 10:37:24.000000 Zino-2.0.0a2/polldevs.cf.example
+-rw-r--r--   0 mvold     (1346) users      (100)     2387 2024-04-09 10:37:24.000000 Zino-2.0.0a2/pyproject.toml
+-rw-r--r--   0 mvold     (1346) users      (100)       38 2024-04-09 10:39:52.854507 Zino-2.0.0a2/setup.cfg
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.823505 Zino-2.0.0a2/src/
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.851507 Zino-2.0.0a2/src/Zino.egg-info/
+-rw-r--r--   0 mvold     (1346) users      (100)    25009 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/Zino.egg-info/PKG-INFO
+-rw-r--r--   0 mvold     (1346) users      (100)     4137 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/Zino.egg-info/SOURCES.txt
+-rw-r--r--   0 mvold     (1346) users      (100)        1 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/Zino.egg-info/dependency_links.txt
+-rw-r--r--   0 mvold     (1346) users      (100)       40 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/Zino.egg-info/entry_points.txt
+-rw-r--r--   0 mvold     (1346) users      (100)        1 2024-01-18 09:45:52.000000 Zino-2.0.0a2/src/Zino.egg-info/not-zip-safe
+-rw-r--r--   0 mvold     (1346) users      (100)      197 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/Zino.egg-info/requires.txt
+-rw-r--r--   0 mvold     (1346) users      (100)        5 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/Zino.egg-info/top_level.txt
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.828505 Zino-2.0.0a2/src/zino/
+-rw-r--r--   0 mvold     (1346) users      (100)       13 2023-02-23 15:30:20.000000 Zino-2.0.0a2/src/zino/__init__.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.828505 Zino-2.0.0a2/src/zino/api/
+-rw-r--r--   0 mvold     (1346) users      (100)        0 2023-10-20 10:30:51.000000 Zino-2.0.0a2/src/zino/api/__init__.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2315 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/api/auth.py
+-rw-r--r--   0 mvold     (1346) users      (100)    15464 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/api/legacy.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5075 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/api/notify.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2015 2024-01-25 08:44:34.000000 Zino-2.0.0a2/src/zino/api/server.py
+-rw-r--r--   0 mvold     (1346) users      (100)      459 2023-11-28 10:39:04.000000 Zino-2.0.0a2/src/zino/compat.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.829505 Zino-2.0.0a2/src/zino/config/
+-rw-r--r--   0 mvold     (1346) users      (100)        0 2023-02-23 15:30:20.000000 Zino-2.0.0a2/src/zino/config/__init__.py
+-rw-r--r--   0 mvold     (1346) users      (100)      838 2024-03-22 14:42:42.000000 Zino-2.0.0a2/src/zino/config/models.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1776 2023-10-11 11:12:54.000000 Zino-2.0.0a2/src/zino/config/polldevs.py
+-rw-r--r--   0 mvold     (1346) users      (100)     7480 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/events.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1107 2023-11-03 08:36:03.000000 Zino-2.0.0a2/src/zino/getuptime.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1179 2023-11-03 08:35:54.000000 Zino-2.0.0a2/src/zino/getyellowalarms.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.832505 Zino-2.0.0a2/src/zino/mibdumps/
+-rw-r--r--   0 mvold     (1346) users      (100)    31051 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/BFD-STD-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5601 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/BFD-TC-STD-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)    43401 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/BGP4-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)   152115 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/BGP4-V2-MIB-JUNIPER.py
+-rw-r--r--   0 mvold     (1346) users      (100)    84335 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/CISCO-BGP4-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)    42882 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/CISCO-IETF-BFD-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)    21764 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/CISCO-SMI.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3486 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/DIFFSERV-DSCP-TC.py
+-rw-r--r--   0 mvold     (1346) users      (100)   113815 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/DIFFSERV-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)     8117 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/IANA-BFD-TC-STD-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)     9735 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/IANAifType-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)    25451 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/IF-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)    25613 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/INTEGRATED-SERVICES-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)   184120 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/IP-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)     4117 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-ALARM-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)     8047 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-BFD-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5301 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-EXPERIMENT-MIB.py
+-rw-r--r--   0 mvold     (1346) users      (100)    11653 2024-04-03 12:11:11.000000 Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-SMI.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1671 2023-10-03 12:46:19.000000 Zino-2.0.0a2/src/zino/oid.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2465 2023-10-11 10:42:06.000000 Zino-2.0.0a2/src/zino/polltest.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3499 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/scheduler.py
+-rw-r--r--   0 mvold     (1346) users      (100)    19432 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/snmp.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1938 2024-01-23 13:56:40.000000 Zino-2.0.0a2/src/zino/state.py
+-rw-r--r--   0 mvold     (1346) users      (100)    10997 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/statemodels.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.835506 Zino-2.0.0a2/src/zino/tasks/
+-rw-r--r--   0 mvold     (1346) users      (100)     1032 2024-01-26 09:26:00.000000 Zino-2.0.0a2/src/zino/tasks/__init__.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3289 2024-03-22 14:42:29.000000 Zino-2.0.0a2/src/zino/tasks/addrs.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5523 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/tasks/bfdtask.py
+-rw-r--r--   0 mvold     (1346) users      (100)    14150 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/tasks/bgpstatemonitortask.py
+-rw-r--r--   0 mvold     (1346) users      (100)       50 2024-01-25 07:41:54.000000 Zino-2.0.0a2/src/zino/tasks/errors.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2800 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/tasks/juniperalarmtask.py
+-rw-r--r--   0 mvold     (1346) users      (100)     7352 2024-01-25 07:41:54.000000 Zino-2.0.0a2/src/zino/tasks/linkstatetask.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2827 2024-01-25 07:41:54.000000 Zino-2.0.0a2/src/zino/tasks/reachabletask.py
+-rw-r--r--   0 mvold     (1346) users      (100)      778 2024-03-22 13:59:50.000000 Zino-2.0.0a2/src/zino/tasks/task.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1150 2024-01-25 07:41:54.000000 Zino-2.0.0a2/src/zino/tasks/vendor.py
+-rw-r--r--   0 mvold     (1346) users      (100)      206 2023-05-11 13:12:56.000000 Zino-2.0.0a2/src/zino/time.py
+-rw-r--r--   0 mvold     (1346) users      (100)     9373 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/trapd.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2373 2024-04-03 12:09:00.000000 Zino-2.0.0a2/src/zino/traptest.py
+-rw-r--r--   0 mvold     (1346) users      (100)      913 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/utils.py
+-rw-r--r--   0 mvold     (1346) users      (100)      413 2024-04-09 10:39:52.000000 Zino-2.0.0a2/src/zino/version.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5984 2024-04-09 10:37:24.000000 Zino-2.0.0a2/src/zino/zino.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.838506 Zino-2.0.0a2/tests/
+-rw-r--r--   0 mvold     (1346) users      (100)        0 2023-02-23 15:30:20.000000 Zino-2.0.0a2/tests/__init__.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.839506 Zino-2.0.0a2/tests/api/
+-rw-r--r--   0 mvold     (1346) users      (100)        0 2023-10-20 10:30:51.000000 Zino-2.0.0a2/tests/api/__init__.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2764 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/api/auth_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)      764 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/api/conftest.py
+-rw-r--r--   0 mvold     (1346) users      (100)    28633 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/api/legacy_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     6085 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/api/notify_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)      265 2024-01-25 08:44:34.000000 Zino-2.0.0a2/tests/api/server_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)      638 2023-06-15 13:00:29.000000 Zino-2.0.0a2/tests/bin_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)      581 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/compat_test.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.839506 Zino-2.0.0a2/tests/config/
+-rw-r--r--   0 mvold     (1346) users      (100)        0 2023-02-23 15:31:31.000000 Zino-2.0.0a2/tests/config/__init__.py
+-rw-r--r--   0 mvold     (1346) users      (100)      369 2023-02-23 15:31:31.000000 Zino-2.0.0a2/tests/config/models_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2745 2023-10-11 11:53:13.000000 Zino-2.0.0a2/tests/config/polldevs_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3856 2024-03-19 14:40:23.000000 Zino-2.0.0a2/tests/conftest.py
+-rw-r--r--   0 mvold     (1346) users      (100)     7233 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/events_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1136 2023-08-09 09:50:27.000000 Zino-2.0.0a2/tests/oid_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2755 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/scheduler_test.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.847506 Zino-2.0.0a2/tests/snmp_fixtures/
+-rw-r--r--   0 mvold     (1346) users      (100)      285 2024-01-17 12:52:21.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bfd-up.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      375 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bgp-admin-down.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      375 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bgp-admin-up.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      371 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bgp-external-reset.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      371 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bgp-oper-down-short.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      375 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bgp-oper-down.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      343 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/cisco-bgp.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/general-bgp-admin-down.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/general-bgp-admin-up.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      373 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/general-bgp-external-reset.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      373 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/general-bgp-oper-down-short.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/general-bgp-oper-down.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      377 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/general-bgp.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      287 2024-01-23 13:56:40.000000 Zino-2.0.0a2/tests/snmp_fixtures/ip-ad-ent-addr.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)       71 2023-08-09 09:50:27.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-alarm-wrong.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)       68 2023-09-11 13:32:27.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-alarm-zero.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)       68 2023-09-11 13:32:27.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-alarm.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      867 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bfd-up.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      551 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-admin-down.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      550 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-admin-up.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      547 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-external-reset.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      547 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-oper-down-short.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      551 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-oper-down.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      551 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)     2948 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/snmp_fixtures/linksdown.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)     2948 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/snmp_fixtures/linksup.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)      180 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/missing-info-bgp.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)    42180 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_fixtures/public.snmprec
+-rw-r--r--   0 mvold     (1346) users      (100)     9697 2024-01-26 09:26:00.000000 Zino-2.0.0a2/tests/snmp_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     2404 2024-01-17 11:17:17.000000 Zino-2.0.0a2/tests/state_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5717 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/statemodels_test.py
+drwxr-xr-x   0 mvold     (1346) users      (100)        0 2024-04-09 10:39:52.851507 Zino-2.0.0a2/tests/tasks/
+-rw-r--r--   0 mvold     (1346) users      (100)        0 2023-06-15 13:00:29.000000 Zino-2.0.0a2/tests/tasks/__init__.py
+-rw-r--r--   0 mvold     (1346) users      (100)      800 2024-01-25 07:41:54.000000 Zino-2.0.0a2/tests/tasks/conftest.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3014 2024-01-23 13:56:40.000000 Zino-2.0.0a2/tests/tasks/test_addrs.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3869 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/tasks/test_bfdtask.py
+-rw-r--r--   0 mvold     (1346) users      (100)    12965 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/tasks/test_bgpstatemonitortask.py
+-rw-r--r--   0 mvold     (1346) users      (100)      164 2023-11-28 10:39:04.000000 Zino-2.0.0a2/tests/tasks/test_init.py
+-rw-r--r--   0 mvold     (1346) users      (100)     6425 2024-01-25 07:41:54.000000 Zino-2.0.0a2/tests/tasks/test_juniperalarmtask.py
+-rw-r--r--   0 mvold     (1346) users      (100)     5481 2024-01-17 11:26:31.000000 Zino-2.0.0a2/tests/tasks/test_linkstatetask.py
+-rw-r--r--   0 mvold     (1346) users      (100)     3353 2024-01-25 07:41:54.000000 Zino-2.0.0a2/tests/tasks/test_reachabletask.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1819 2024-01-25 07:41:54.000000 Zino-2.0.0a2/tests/tasks/test_run_all_tasks.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1063 2024-01-25 07:41:54.000000 Zino-2.0.0a2/tests/tasks/test_task.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1173 2024-01-25 07:41:54.000000 Zino-2.0.0a2/tests/tasks/test_vendor.py
+-rw-r--r--   0 mvold     (1346) users      (100)     6399 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/trapd_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     1652 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/utils_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)     4989 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tests/zino_test.py
+-rw-r--r--   0 mvold     (1346) users      (100)      665 2024-04-09 10:37:24.000000 Zino-2.0.0a2/tox.ini
```

### Comparing `Zino-2.0.0a1/.github/workflows/linter.yml` & `Zino-2.0.0a2/.github/workflows/linter.yml`

 * *Files 13% similar despite different names*

```diff
@@ -45,23 +45,30 @@
           # Full git history is needed to get a proper
           # list of changed files within `super-linter`
           fetch-depth: 0
 
       ################################
       # Run Linter against code base #
       ################################
-      - name: Lint Code Base
+      - name: Lint Code Base with black and isort
         uses: github/super-linter/slim@v5
         env:
           VALIDATE_ALL_CODEBASE: false
           DEFAULT_BRANCH: master
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           # Add validation for other languages here or comment out all to validate all languages
           VALIDATE_PYTHON_BLACK: true
-          VALIDATE_PYTHON_FLAKE8: true
           VALIDATE_PYTHON_ISORT: true
           # Tell the linter the location of the configuration file (pyproject.toml)
           LINTER_RULES_PATH: .
           PYTHON_BLACK_CONFIG_FILE: pyproject.toml
           PYTHON_ISORT_CONFIG_FILE: pyproject.toml
           # Exclude mibdumps files
           FILTER_REGEX_EXCLUDE: .*src/zino/mibdumps/.*
+
+      ################################
+      # Run ruff against code base #
+      ################################
+      - name: Lint Code Base with ruff
+        uses: chartboost/ruff-action@v1
+        with:
+          args: --exclude "mibdumps"
```

### Comparing `Zino-2.0.0a1/.github/workflows/publish-test-results.yml` & `Zino-2.0.0a2/.github/workflows/publish-test-results.yml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     types:
       - completed
 
 jobs:
   publish-test-results:
     name: "Publish test results"
     runs-on: ubuntu-latest
-    if: github.event.workflow_run.conclusion != 'skipped'
+    if: github.event.workflow_run.conclusion != 'skipped' && github.repository_owner == 'Uninett'
+
 
     steps:
       - name: Download and Extract Artifacts
         env:
           GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
         run: |
            mkdir -p artifacts && cd artifacts
@@ -29,8 +30,8 @@
            done
 
       - name: "Publish test results"
         uses: EnricoMi/publish-unit-test-result-action/composite@v1
         with:
           commit: ${{ github.event.workflow_run.head_sha }}
           check_name: "Test results"
-          files: artifacts/**/*-results.xml
+          files: artifacts/**/*-results.xml
```

### Comparing `Zino-2.0.0a1/.github/workflows/tests.yml` & `Zino-2.0.0a2/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -42,21 +42,22 @@
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install "tox<4" tox-gh-actions coverage
+          sudo apt-get install -y --no-install-recommends snmp
 
       - name: Test with tox
         run: tox
 
       - name: "Upload coverage to Codecov"
-        if: "github.repository_owner == 'Uninett'"
-        uses: codecov/codecov-action@v3
+        if: github.repository_owner == 'Uninett'
+        uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
           token: ${{ secrets.CODECOV_TOKEN }}
 
       - name: Upload test reports (${{ matrix.python-version }})
         if: always()
         uses: actions/upload-artifact@v3
```

### Comparing `Zino-2.0.0a1/.pre-commit-config.yaml` & `Zino-2.0.0a2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
       - id: isort
         name: isort (python)
   - repo: https://github.com/psf/black
     rev: 23.1.0
     hooks:
       - id: black
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.245
+    rev: v0.1.13
     hooks:
       - id: ruff
```

### Comparing `Zino-2.0.0a1/LICENSE` & `Zino-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/PKG-INFO` & `Zino-2.0.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zino
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Robust network management system for large backbone networks
 Author-email: Sikt - Kunnskapssektorens Tjenesteleverandør <kontakt@sikt.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -252,16 +252,20 @@
 This is the modern Python re-implementation of the battle-proven Zino network
 state monitor, first implemented in Tcl/Scotty at Uninett in the 1990s.
 
 This is still a work in progress, and is not yet a fully functional replacement
 for the original Tcl-based Zino.  An incomplete list of features that have yet
 to be ported:
 
-- SNMP trap reception
-  - Hence, no port flapping status
+- SNMP trap handling
+  - Incoming traps are only logged (except for a selected set of spammy traps
+    that are ignored)
+  - Since link traps aren't handled yet, there's no port flapping status
+  - No support for reading trap messages from a trap multiplexer like
+    `straps`/`nmtrapd`.
 - Planned maintenance (the `PM` family of API commands)
 - Router and single-port poll triggering from the API (the `POLLRTR` and
   `POLLINTF` API commands)
 
 Development of Zino 2.0 is fully sponsored by [NORDUnet](https://nordu.net/),
 on behalf of the nordic NRENs.
 
@@ -283,21 +287,23 @@
 research institutions of Norway.  Uninett was also part of NORDUnet, the
 collaboration that interconnects the NRENs of the Nordic countries, and Zino
 is also utilized to monitor the NORDUnet backbone.
 
 Here's a quote about its features from the `README` file of the original Tcl
 codebase:
 
-> o Trap-driven polling; receives and interprets traps.
-> o Periodic status polling (by default low frequency).
-> o A simplistic event handling system.
-> o A simple SMTP-like client/server protocol.
-> o A TK-based user interface.
+```
+ o Trap-driven polling; receives and interprets traps.
+ o Periodic status polling (by default low frequency).
+ o A simplistic event handling system.
+ o A simple SMTP-like client/server protocol.
+ o A TK-based user interface.
 
-> all in a little under 5000 lines of Tcl.
+all in a little under 5000 lines of Tcl.
+```
 
 This project aims to port all this to Python, except for the TK-based user
 interface.  The Python implementation keeps backwards compatibility with the
 "simple SMTP-like client/server protocol", so that the existing user interface
 clients can be re-used (such as *Ritz* and *cuRitz*).  Additionally, a new web
 user interface client is being developed at https://github.com/uninett/howitz .
 
@@ -376,32 +382,48 @@
 
 In order for Zino to function properly, you first need to make a minimal
 `polldevs.cf` configuration file, as described in the next section.  However,
 at this point you can test that the `zino` command is available to run:
 
 ```console
 $ zino --help
-usage: zino [-h] [--polldevs PATH] [--debug] [--stop-in N]
+usage: zino [-h] [--polldevs PATH] [--debug] [--stop-in N] [--trap-port PORT] [--user USER]
 
 Zino is not OpenView
 
 options:
-  -h, --help       show this help message and exit
-  --polldevs PATH  Path to polldevs.cf
-  --debug          Set global log level to DEBUG. Very chatty!
-  --stop-in N      Stop zino after N seconds.
+  -h, --help        show this help message and exit
+  --polldevs PATH   Path to polldevs.cf
+  --debug           Set global log level to DEBUG. Very chatty!
+  --stop-in N       Stop zino after N seconds.
+  --trap-port PORT  Which UDP port to listen for traps on. Default value is 162. Any value below 1024 requires root privileges. Setting to 0
+                    disables SNMP trap monitoring.
+  --user USER       Switch to this user immediately after binding to privileged ports
 ```
 
 Even if the Python virtual environment hasn't been activated in your shell, you
 can still run Zino directly from inside this environment, like so:
 
 ```shell
 ./zino-env/bin/zino --help
 ```
 
+By default, Zino will listen for incoming SNMP traps on UDP port `162`.  This
+port is privileged (less than 1024), however, which means that Zino *needs to
+be started as `root`* if you want to receive traps.  In order to avoid running
+continuously with `root` privileges, the `--user` option can be used to tell
+Zino to switch to running as a less privileged user as soon as port `162` has
+been acquired.
+
+Alternately, you can tell Zino to listen for traps on a non-privileged port,
+e.g. by adding `--trap-port 1162` to the command line arguments, but this only
+works if you can configure your SNMP agents to send traps to this non-standard
+port.  In any case, you can also tell Zino to skip listening for traps by
+specifying `--trap-port 0`.
+
 ### Configuring Zino
 
 ### Minimal configuration
 
 At minimum, Zino must be configured with a list of SNMP-enabled routers to
 monitor.  By default, it looks for `polldevs.cf` in the current working
 directory, but a different configuration file can be specified using the
@@ -485,7 +507,30 @@
 
 Before you start hacking, enable pre-commit hooks in your cloned repository,
 like so:
 
 ```shell
 pre-commit install
 ```
+
+
+### Test trap examples
+
+Running Zino during development might look like this (listening for traps on
+the non-privileged port 1162):
+
+```shell
+zino --trap-port 1162
+```
+
+To send an example trap (`BGP4-MIB::bgpBackwardTransition`, which Zino ignores
+by default), you can use a command like:
+
+```shell
+snmptrap -v2c -c public \
+    127.0.0.1:1162 \
+    '' \
+    BGP4-MIB::bgpBackwardTransition \
+    BGP4-MIB::bgpPeerRemoteAddr a 192.168.42.42 \
+    BGP4-MIB::bgpPeerLastError x 4242 \
+    BGP4-MIB::bgpPeerState i 2
+```
```

### Comparing `Zino-2.0.0a1/README.md` & `Zino-2.0.0a2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 This is the modern Python re-implementation of the battle-proven Zino network
 state monitor, first implemented in Tcl/Scotty at Uninett in the 1990s.
 
 This is still a work in progress, and is not yet a fully functional replacement
 for the original Tcl-based Zino.  An incomplete list of features that have yet
 to be ported:
 
-- SNMP trap reception
-  - Hence, no port flapping status
+- SNMP trap handling
+  - Incoming traps are only logged (except for a selected set of spammy traps
+    that are ignored)
+  - Since link traps aren't handled yet, there's no port flapping status
+  - No support for reading trap messages from a trap multiplexer like
+    `straps`/`nmtrapd`.
 - Planned maintenance (the `PM` family of API commands)
 - Router and single-port poll triggering from the API (the `POLLRTR` and
   `POLLINTF` API commands)
 
 Development of Zino 2.0 is fully sponsored by [NORDUnet](https://nordu.net/),
 on behalf of the nordic NRENs.
 
@@ -37,21 +41,23 @@
 research institutions of Norway.  Uninett was also part of NORDUnet, the
 collaboration that interconnects the NRENs of the Nordic countries, and Zino
 is also utilized to monitor the NORDUnet backbone.
 
 Here's a quote about its features from the `README` file of the original Tcl
 codebase:
 
-> o Trap-driven polling; receives and interprets traps.
-> o Periodic status polling (by default low frequency).
-> o A simplistic event handling system.
-> o A simple SMTP-like client/server protocol.
-> o A TK-based user interface.
+```
+ o Trap-driven polling; receives and interprets traps.
+ o Periodic status polling (by default low frequency).
+ o A simplistic event handling system.
+ o A simple SMTP-like client/server protocol.
+ o A TK-based user interface.
 
-> all in a little under 5000 lines of Tcl.
+all in a little under 5000 lines of Tcl.
+```
 
 This project aims to port all this to Python, except for the TK-based user
 interface.  The Python implementation keeps backwards compatibility with the
 "simple SMTP-like client/server protocol", so that the existing user interface
 clients can be re-used (such as *Ritz* and *cuRitz*).  Additionally, a new web
 user interface client is being developed at https://github.com/uninett/howitz .
 
@@ -130,32 +136,48 @@
 
 In order for Zino to function properly, you first need to make a minimal
 `polldevs.cf` configuration file, as described in the next section.  However,
 at this point you can test that the `zino` command is available to run:
 
 ```console
 $ zino --help
-usage: zino [-h] [--polldevs PATH] [--debug] [--stop-in N]
+usage: zino [-h] [--polldevs PATH] [--debug] [--stop-in N] [--trap-port PORT] [--user USER]
 
 Zino is not OpenView
 
 options:
-  -h, --help       show this help message and exit
-  --polldevs PATH  Path to polldevs.cf
-  --debug          Set global log level to DEBUG. Very chatty!
-  --stop-in N      Stop zino after N seconds.
+  -h, --help        show this help message and exit
+  --polldevs PATH   Path to polldevs.cf
+  --debug           Set global log level to DEBUG. Very chatty!
+  --stop-in N       Stop zino after N seconds.
+  --trap-port PORT  Which UDP port to listen for traps on. Default value is 162. Any value below 1024 requires root privileges. Setting to 0
+                    disables SNMP trap monitoring.
+  --user USER       Switch to this user immediately after binding to privileged ports
 ```
 
 Even if the Python virtual environment hasn't been activated in your shell, you
 can still run Zino directly from inside this environment, like so:
 
 ```shell
 ./zino-env/bin/zino --help
 ```
 
+By default, Zino will listen for incoming SNMP traps on UDP port `162`.  This
+port is privileged (less than 1024), however, which means that Zino *needs to
+be started as `root`* if you want to receive traps.  In order to avoid running
+continuously with `root` privileges, the `--user` option can be used to tell
+Zino to switch to running as a less privileged user as soon as port `162` has
+been acquired.
+
+Alternately, you can tell Zino to listen for traps on a non-privileged port,
+e.g. by adding `--trap-port 1162` to the command line arguments, but this only
+works if you can configure your SNMP agents to send traps to this non-standard
+port.  In any case, you can also tell Zino to skip listening for traps by
+specifying `--trap-port 0`.
+
 ### Configuring Zino
 
 ### Minimal configuration
 
 At minimum, Zino must be configured with a list of SNMP-enabled routers to
 monitor.  By default, it looks for `polldevs.cf` in the current working
 directory, but a different configuration file can be specified using the
@@ -239,7 +261,30 @@
 
 Before you start hacking, enable pre-commit hooks in your cloned repository,
 like so:
 
 ```shell
 pre-commit install
 ```
+
+
+### Test trap examples
+
+Running Zino during development might look like this (listening for traps on
+the non-privileged port 1162):
+
+```shell
+zino --trap-port 1162
+```
+
+To send an example trap (`BGP4-MIB::bgpBackwardTransition`, which Zino ignores
+by default), you can use a command like:
+
+```shell
+snmptrap -v2c -c public \
+    127.0.0.1:1162 \
+    '' \
+    BGP4-MIB::bgpBackwardTransition \
+    BGP4-MIB::bgpPeerRemoteAddr a 192.168.42.42 \
+    BGP4-MIB::bgpPeerLastError x 4242 \
+    BGP4-MIB::bgpPeerState i 2
+```
```

### Comparing `Zino-2.0.0a1/pyproject.toml` & `Zino-2.0.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -105,11 +105,11 @@
 profile = "black"
 src_paths = ["src", "tests"]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
     # Don't need coverage for ellipsis used for type annotations
-    "...",
+    "\\.\\.\\.",
     # Don't complain about lines excluded unless type checking
     "if TYPE_CHECKING:",
 ]
```

### Comparing `Zino-2.0.0a1/src/Zino.egg-info/PKG-INFO` & `Zino-2.0.0a2/src/Zino.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Zino
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Robust network management system for large backbone networks
 Author-email: Sikt - Kunnskapssektorens Tjenesteleverandør <kontakt@sikt.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -252,16 +252,20 @@
 This is the modern Python re-implementation of the battle-proven Zino network
 state monitor, first implemented in Tcl/Scotty at Uninett in the 1990s.
 
 This is still a work in progress, and is not yet a fully functional replacement
 for the original Tcl-based Zino.  An incomplete list of features that have yet
 to be ported:
 
-- SNMP trap reception
-  - Hence, no port flapping status
+- SNMP trap handling
+  - Incoming traps are only logged (except for a selected set of spammy traps
+    that are ignored)
+  - Since link traps aren't handled yet, there's no port flapping status
+  - No support for reading trap messages from a trap multiplexer like
+    `straps`/`nmtrapd`.
 - Planned maintenance (the `PM` family of API commands)
 - Router and single-port poll triggering from the API (the `POLLRTR` and
   `POLLINTF` API commands)
 
 Development of Zino 2.0 is fully sponsored by [NORDUnet](https://nordu.net/),
 on behalf of the nordic NRENs.
 
@@ -283,21 +287,23 @@
 research institutions of Norway.  Uninett was also part of NORDUnet, the
 collaboration that interconnects the NRENs of the Nordic countries, and Zino
 is also utilized to monitor the NORDUnet backbone.
 
 Here's a quote about its features from the `README` file of the original Tcl
 codebase:
 
-> o Trap-driven polling; receives and interprets traps.
-> o Periodic status polling (by default low frequency).
-> o A simplistic event handling system.
-> o A simple SMTP-like client/server protocol.
-> o A TK-based user interface.
+```
+ o Trap-driven polling; receives and interprets traps.
+ o Periodic status polling (by default low frequency).
+ o A simplistic event handling system.
+ o A simple SMTP-like client/server protocol.
+ o A TK-based user interface.
 
-> all in a little under 5000 lines of Tcl.
+all in a little under 5000 lines of Tcl.
+```
 
 This project aims to port all this to Python, except for the TK-based user
 interface.  The Python implementation keeps backwards compatibility with the
 "simple SMTP-like client/server protocol", so that the existing user interface
 clients can be re-used (such as *Ritz* and *cuRitz*).  Additionally, a new web
 user interface client is being developed at https://github.com/uninett/howitz .
 
@@ -376,32 +382,48 @@
 
 In order for Zino to function properly, you first need to make a minimal
 `polldevs.cf` configuration file, as described in the next section.  However,
 at this point you can test that the `zino` command is available to run:
 
 ```console
 $ zino --help
-usage: zino [-h] [--polldevs PATH] [--debug] [--stop-in N]
+usage: zino [-h] [--polldevs PATH] [--debug] [--stop-in N] [--trap-port PORT] [--user USER]
 
 Zino is not OpenView
 
 options:
-  -h, --help       show this help message and exit
-  --polldevs PATH  Path to polldevs.cf
-  --debug          Set global log level to DEBUG. Very chatty!
-  --stop-in N      Stop zino after N seconds.
+  -h, --help        show this help message and exit
+  --polldevs PATH   Path to polldevs.cf
+  --debug           Set global log level to DEBUG. Very chatty!
+  --stop-in N       Stop zino after N seconds.
+  --trap-port PORT  Which UDP port to listen for traps on. Default value is 162. Any value below 1024 requires root privileges. Setting to 0
+                    disables SNMP trap monitoring.
+  --user USER       Switch to this user immediately after binding to privileged ports
 ```
 
 Even if the Python virtual environment hasn't been activated in your shell, you
 can still run Zino directly from inside this environment, like so:
 
 ```shell
 ./zino-env/bin/zino --help
 ```
 
+By default, Zino will listen for incoming SNMP traps on UDP port `162`.  This
+port is privileged (less than 1024), however, which means that Zino *needs to
+be started as `root`* if you want to receive traps.  In order to avoid running
+continuously with `root` privileges, the `--user` option can be used to tell
+Zino to switch to running as a less privileged user as soon as port `162` has
+been acquired.
+
+Alternately, you can tell Zino to listen for traps on a non-privileged port,
+e.g. by adding `--trap-port 1162` to the command line arguments, but this only
+works if you can configure your SNMP agents to send traps to this non-standard
+port.  In any case, you can also tell Zino to skip listening for traps by
+specifying `--trap-port 0`.
+
 ### Configuring Zino
 
 ### Minimal configuration
 
 At minimum, Zino must be configured with a list of SNMP-enabled routers to
 monitor.  By default, it looks for `polldevs.cf` in the current working
 directory, but a different configuration file can be specified using the
@@ -485,7 +507,30 @@
 
 Before you start hacking, enable pre-commit hooks in your cloned repository,
 like so:
 
 ```shell
 pre-commit install
 ```
+
+
+### Test trap examples
+
+Running Zino during development might look like this (listening for traps on
+the non-privileged port 1162):
+
+```shell
+zino --trap-port 1162
+```
+
+To send an example trap (`BGP4-MIB::bgpBackwardTransition`, which Zino ignores
+by default), you can use a command like:
+
+```shell
+snmptrap -v2c -c public \
+    127.0.0.1:1162 \
+    '' \
+    BGP4-MIB::bgpBackwardTransition \
+    BGP4-MIB::bgpPeerRemoteAddr a 192.168.42.42 \
+    BGP4-MIB::bgpPeerLastError x 4242 \
+    BGP4-MIB::bgpPeerState i 2
+```
```

### Comparing `Zino-2.0.0a1/src/Zino.egg-info/SOURCES.txt` & `Zino-2.0.0a2/src/Zino.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 src/zino/oid.py
 src/zino/polltest.py
 src/zino/scheduler.py
 src/zino/snmp.py
 src/zino/state.py
 src/zino/statemodels.py
 src/zino/time.py
+src/zino/trapd.py
+src/zino/traptest.py
+src/zino/utils.py
 src/zino/version.py
 src/zino/zino.py
 src/zino/api/__init__.py
 src/zino/api/auth.py
 src/zino/api/legacy.py
 src/zino/api/notify.py
 src/zino/api/server.py
@@ -78,14 +81,16 @@
 tests/conftest.py
 tests/events_test.py
 tests/oid_test.py
 tests/scheduler_test.py
 tests/snmp_test.py
 tests/state_test.py
 tests/statemodels_test.py
+tests/trapd_test.py
+tests/utils_test.py
 tests/zino_test.py
 tests/api/__init__.py
 tests/api/auth_test.py
 tests/api/conftest.py
 tests/api/legacy_test.py
 tests/api/notify_test.py
 tests/api/server_test.py
```

### Comparing `Zino-2.0.0a1/src/zino/api/auth.py` & `Zino-2.0.0a2/src/zino/api/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,8 +54,9 @@
             user, secret = line.split(" ", maxsplit=1)
             secrets[user] = secret
 
     return secrets
 
 
 class AuthenticationFailure(Exception):
-    pass
+    def __init__(self, message="Authentication failure"):
+        super().__init__(message)
```

### Comparing `Zino-2.0.0a1/src/zino/api/legacy.py` & `Zino-2.0.0a2/src/zino/api/legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Legacy API implementation for Zino 2.0.
 
 The Legacy API from the Tcl-based Zino 1.0 is a 'vaguely SMTP-esque line-based text protocol'.  This module
 implements this protocol using asyncio semantics.
 """
+
 import asyncio
 import inspect
 import logging
 import re
 import textwrap
 from functools import wraps
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable, List, Optional, Union
 
 from zino import version
 from zino.api import auth
 from zino.api.notify import Zino1NotificationProtocol
 from zino.state import ZinoState
-from zino.statemodels import Event, EventState
+from zino.statemodels import ClosedEventError, Event, EventState
 
 if TYPE_CHECKING:
     from zino.api.server import ZinoServer
 
 _logger = logging.getLogger(__name__)
 
 
@@ -229,16 +230,18 @@
 
     async def do_version(self):
         self._respond(200, f"zino version is {version.__version__}")
 
     @requires_authentication
     async def do_caseids(self):
         self._respond(304, "list of active cases follows, terminated with '.'")
-        for event_id in sorted(self._state.events.events):
-            self._respond_raw(str(event_id))
+        events = self._state.events.events
+        for event_id, event in sorted(events.items()):
+            if event.state != EventState.CLOSED:
+                self._respond_raw(str(event_id))
         self._respond_raw(".")
 
     def _translate_case_id_to_event(responder: callable):  # noqa
         """Decorates any command that works with events/cases, adding verification of the incoming case_id argument
         and translation to an actual Event object.
         """
 
@@ -328,15 +331,18 @@
         try:
             event_state = EventState(state)
         except ValueError:
             allowable_states = ", ".join(s.value for s in EventState)
             return self._respond_error(f"state must be one of {allowable_states}")
 
         out_event = self._state.events.checkout(event.id)
-        out_event.set_state(event_state, user=self.user)
+        try:
+            out_event.set_state(event_state, user=self.user)
+        except ClosedEventError:
+            return self._respond_error(f"Cannot reopen closed event {event.id}")
         self._state.events.commit(out_event)
 
         return self._respond_ok()
 
     @requires_authentication
     async def do_community(self, router_name: str):
         from zino.state import polldevs
```

### Comparing `Zino-2.0.0a1/src/zino/api/notify.py` & `Zino-2.0.0a2/src/zino/api/notify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Notification channel implementation for Zino 2.0.
 
 Notification channels are currently part of the legacy API from the Tcl-based Zino 1.0.  They are a simple text-based,
 line-oriented protocol.  Clients are not expected to send any data to a notification channel, only receive data from
 the server.
 """
+
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Any, Iterator, NamedTuple, Optional
 
 from zino.api import auth
 from zino.state import ZinoState
 from zino.statemodels import Event, EventState
@@ -72,42 +73,48 @@
 
     @tied_to.setter
     def tied_to(self, client: "Zino1ServerProtocol") -> None:
         self._tied_to = client
 
     def notify(self, notification: Notification):
         """Sends a notification to the connected client"""
-        self._respond_raw(f"{notification.event_id} {notification.change_type} {notification.value}")
+        self._respond_raw(f"{notification.event_id} {notification.change_type} {notification.value or ''}")
 
     def _respond_raw(self, message: str):
         """Encodes and sends a response line to the connected client"""
         self.transport.write(f"{message}\r\n".encode("utf-8"))
 
     @classmethod
     def build_and_send_notifications(
         cls, server: "ZinoServer", new_event: Event, old_event: Optional[Event] = None
     ) -> None:
         """Prepares and sends notifications for all changes between old_event and new_event to all connected and tied
         notification channels.
         """
-        notifications = list(cls.build_notifications(new_event, old_event))
+        notifications = list(cls.build_notifications(server.state, new_event, old_event))
         tied_channels = [channel for channel in server.notification_channels.values() if channel.tied_to]
         _logger.debug("Sending %s notifications to %s tied channels", len(notifications), len(tied_channels))
 
         for notification in notifications:
             for channel in tied_channels:
                 channel.notify(notification)
 
     @classmethod
-    def build_notifications(cls, new_event: Event, old_event: Optional[Event] = None) -> Iterator[Notification]:
+    def build_notifications(
+        cls, state: ZinoState, new_event: Event, old_event: Optional[Event] = None
+    ) -> Iterator[Notification]:
         """Generates a sequence of Notification objects from the changes detected between old_event and new_event.
 
         If `old_event` is `None`, it is assumed the event is brand new, and only the state change from EMBRYONIC
         matters.
         """
+        if new_event.id not in state.events.events:
+            # Event has just been scavenged after being closed for a while
+            yield Notification(new_event.id, "scavenged", None)
+
         changed = new_event.get_changed_fields(old_event) if old_event else ["state"]
 
         for attr in changed:
             if attr == "state":
                 old_state = EventState.EMBRYONIC if not old_event else old_event.state
                 yield Notification(new_event.id, attr, f"{old_state.value} {new_event.state.value}")
```

### Comparing `Zino-2.0.0a1/src/zino/api/server.py` & `Zino-2.0.0a2/src/zino/api/server.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/config/models.py` & `Zino-2.0.0a2/src/zino/config/models.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/config/polldevs.py` & `Zino-2.0.0a2/src/zino/config/polldevs.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/events.py` & `Zino-2.0.0a2/src/zino/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import logging
+from datetime import timedelta
 from typing import Dict, NamedTuple, Optional, Protocol, Type, Union
 
 from pydantic.main import BaseModel
 
 from zino.statemodels import (
     AlarmEvent,
     BFDEvent,
     BGPEvent,
     Event,
     EventState,
     PortStateEvent,
     ReachabilityEvent,
     SubIndex,
 )
+from zino.time import now
 
 _log = logging.getLogger(__name__)
 
+EVENT_EXPIRY = timedelta(hours=8)
+EVENT_DUMP_DIR = "old-events"
+
 
 class EventIndex(NamedTuple):
     router: str
     subindex: SubIndex
     type: Type
 
 
@@ -49,16 +54,17 @@
     def _rebuild_indexes(self):
         """Rebuilds the event index from the current dict of events.
 
         Mostly useful when this object was constructed from dumped data, of which the index isn't a part.
         """
         new_index: Dict[EventIndex, Event] = {}
         for event in self.events.values():
-            key = EventIndex(event.router, event.subindex, type(event))
-            new_index[key] = event
+            if event.state != EventState.CLOSED:
+                key = EventIndex(event.router, event.subindex, type(event))
+                new_index[key] = event
         self._events_by_index = new_index
 
     def get_or_create_event(
         self,
         device_name: str,
         subindex: SubIndex,
         event_class: Type[Event],
@@ -127,19 +133,49 @@
         is_new = not event.id
         if is_new:
             old_event = None
             event.id = self.get_next_available_event_id()
         else:
             old_event = self.events[event.id]
         index = EventIndex(event.router, event.subindex, type(event))
-        self._events_by_index[index] = event
         self.events[event.id] = event
 
+        # If event is set to closed, remove it from index and set updated
+        if event.state == EventState.CLOSED:
+            if self._events_by_index.get(index) and event.id == self._events_by_index[index].id:
+                del self._events_by_index[index]
+            event.updated = now()
+        else:
+            self._events_by_index[index] = event
+
         self._call_observers_for(new_event=event, old_event=old_event)
 
+    def _delete(self, event: Event):
+        """Removes a closed event from the events dict and notifies all observers"""
+        if event.state != EventState.CLOSED:
+            return
+
+        event.dump_event_to_file(dir_name=f"{EVENT_DUMP_DIR}/{now().year}-{now().month}/{now().day}")
+        index = EventIndex(event.router, event.subindex, type(event))
+        if self._events_by_index.get(index) and event.id == self._events_by_index[index].id:
+            _log.info("Closed event %s was still in event index, removing it now", event.id)
+            del self._events_by_index[index]
+        try:
+            del self.events[event.id]
+        except KeyError:
+            pass
+        self._call_observers_for(new_event=event)
+
+    def delete_expired_events(self):
+        """Deletes all events that have been closed for a certain time"""
+        event_list = list(self.events.values())
+        for event in event_list:
+            if event.state == EventState.CLOSED and now() > (event.updated + EVENT_EXPIRY):
+                self._delete(event)
+
     def add_event_observer(self, observer: EventObserver):
         """Adds an observer function that will be called any time an event is committed"""
         self._observers.append(observer)
 
     def get_next_available_event_id(self):
         """Returns the next available event id"""
         self.last_event_id += 1
```

### Comparing `Zino-2.0.0a1/src/zino/getuptime.py` & `Zino-2.0.0a2/src/zino/getuptime.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/getyellowalarms.py` & `Zino-2.0.0a2/src/zino/getyellowalarms.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/BFD-STD-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/BFD-STD-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/BFD-TC-STD-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/BFD-TC-STD-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/BGP4-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/BGP4-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/BGP4-V2-MIB-JUNIPER.py` & `Zino-2.0.0a2/src/zino/mibdumps/BGP4-V2-MIB-JUNIPER.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/CISCO-BGP4-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/CISCO-BGP4-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/CISCO-IETF-BFD-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/CISCO-IETF-BFD-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/CISCO-SMI.py` & `Zino-2.0.0a2/src/zino/mibdumps/CISCO-SMI.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/DIFFSERV-DSCP-TC.py` & `Zino-2.0.0a2/src/zino/mibdumps/DIFFSERV-DSCP-TC.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/DIFFSERV-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/DIFFSERV-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/IANA-BFD-TC-STD-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/IANA-BFD-TC-STD-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/IANAifType-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/IANAifType-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/IF-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/IF-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/INTEGRATED-SERVICES-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/INTEGRATED-SERVICES-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/IP-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/IP-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-ALARM-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-ALARM-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-BFD-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-BFD-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-EXPERIMENT-MIB.py` & `Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-EXPERIMENT-MIB.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/mibdumps/JUNIPER-SMI.py` & `Zino-2.0.0a2/src/zino/mibdumps/JUNIPER-SMI.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/oid.py` & `Zino-2.0.0a2/src/zino/oid.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/polltest.py` & `Zino-2.0.0a2/src/zino/polltest.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/scheduler.py` & `Zino-2.0.0a2/src/zino/scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Sequence, Set, Tuple
 
 from apscheduler.executors.asyncio import AsyncIOExecutor
 from apscheduler.jobstores.base import JobLookupError
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from zino import state
-from zino.config.models import DEFAULT_INTERVAL_MINUTES
+from zino.config.models import DEFAULT_INTERVAL_MINUTES, PollDevice
 from zino.config.polldevs import read_polldevs
 from zino.tasks import run_all_tasks
 
 _log = logging.getLogger(__name__)
 _scheduler = None
 
 
@@ -44,24 +44,32 @@
     :returns: A tuple of (new_devices, deleted_devices)
     """
     devices = {d.name: d for d in read_polldevs(polldevs_conf)}
     new_devices = set(devices) - set(state.polldevs)
     deleted_devices = set(state.polldevs) - set(devices)
     if new_devices:
         _log.info("loaded new devices: %r", new_devices)
+        init_state_for_devices((devices[d] for d in new_devices))
     if deleted_devices:
         _log.info("deleted devices: %r", deleted_devices)
 
     state.polldevs.update(devices)
     for device in deleted_devices:
         del state.polldevs[device]
 
     return new_devices, deleted_devices
 
 
+def init_state_for_devices(devices: Sequence[PollDevice]):
+    """Initializes empty state structures for new devices, if none already exist"""
+    for device in devices:
+        state.state.addresses[device.address] = device.name
+        state.state.devices.get(device.name)
+
+
 async def load_and_schedule_polldevs(polldevs_conf: str):
     new_devices, deleted_devices = load_polldevs(polldevs_conf)
     schedule_new_devices(new_devices)
     deschedule_deleted_devices(deleted_devices)
 
 
 def schedule_new_devices(new_devices: Sequence[str]):
```

### Comparing `Zino-2.0.0a1/src/zino/snmp.py` & `Zino-2.0.0a2/src/zino/snmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,20 +33,27 @@
 _local = threading.local()
 
 MIB_SOURCE_DIR = os.path.join(os.path.dirname(__file__), "mibdumps")
 
 
 def _get_engine():
     if not getattr(_local, "snmp_engine", None):
-        _local.snmp_engine = SnmpEngine()
-        mib_builder = _local.snmp_engine.getMibBuilder()
-        mib_builder.addMibSources(builder.DirMibSource(MIB_SOURCE_DIR))
+        _local.snmp_engine = get_new_snmp_engine()
     return _local.snmp_engine
 
 
+def get_new_snmp_engine() -> SnmpEngine:
+    """Returns a new SnmpEngine object with Zino's directory of MIB modules loaded"""
+    snmp_engine = SnmpEngine()
+    mib_builder = snmp_engine.getMibBuilder()
+    mib_builder.addMibSources(builder.DirMibSource(MIB_SOURCE_DIR))
+    mib_builder.loadModules()
+    return snmp_engine
+
+
 @dataclass
 class MibObject:
     oid: OID
     value: Union[str, int, OID]
 
 
 class Identifier(NamedTuple):
@@ -454,12 +461,12 @@
     if isinstance(value, univ.Integer):
         value = int(value) if not value.namedValues else value.prettyPrint()
     elif isinstance(value, univ.OctetString):
         if type(value).__name__ in ("InetAddress", "IpAddress"):
             value = value.prettyPrint()
         else:
             value = str(value)
-    elif isinstance(value, ObjectIdentity):
+    elif isinstance(value, (ObjectIdentity, univ.ObjectIdentifier)):
         value = OID(str(value))
     else:
         raise ValueError(f"Could not convert unknown type {type(value)}")
     return value
```

### Comparing `Zino-2.0.0a1/src/zino/state.py` & `Zino-2.0.0a2/src/zino/state.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/statemodels.py` & `Zino-2.0.0a2/src/zino/statemodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Basic data models for keeping/serializing/deserializing Zino state"""
+
 import datetime
 import logging
+import pathlib
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from pydantic import BaseModel, Field
 
 from zino.compat import StrEnum
@@ -13,14 +15,20 @@
 IPAddress = Union[IPv4Address, IPv6Address]
 AlarmType = Literal["yellow", "red"]
 SubIndex = Union[None, int, IPAddress, AlarmType]
 
 _logger = logging.getLogger(__name__)
 
 
+class ClosedEventError(Exception):
+    """Closed events cannot be reopened"""
+
+    pass
+
+
 class BGPStyle(StrEnum):
     """The set of allowable BGP styles"""
 
     JUNIPER = "juniper"
     CISCO = "cisco"
     GENERAL = "general"
 
@@ -101,15 +109,14 @@
 
 class DeviceState(BaseModel):
     """Keep device state"""
 
     name: str
     addresses: set[IPAddress] = set()
     enterprise_id: Optional[int] = None
-    boot_time: Optional[int] = None
     ports: Dict[int, Port] = {}
     alarms: Optional[Dict[AlarmType, int]] = None
     boot_time: Optional[datetime.datetime] = None
     bgp_style: Optional[BGPStyle] = None
     bgp_peers: dict[IPAddress, BGPPeerSession] = dict()
 
     # This is the remaining set of potential device attributes stored in device state by the original Zino code:
@@ -222,14 +229,15 @@
 
     router: str
     type: Literal["Event"] = "Event"
     state: EventState = EventState.EMBRYONIC
     opened: datetime.datetime = Field(default_factory=now)
     updated: Optional[datetime.datetime] = None
     priority: int = 100
+    lastevent: Optional[str] = None
 
     log: List[LogEntry] = []
     history: List[LogEntry] = []
 
     # More-or-less optional event attrs (as guesstimated from the original Zino code)
     lasttrans: Optional[datetime.datetime] = None
     flaps: Optional[int] = None
@@ -247,14 +255,16 @@
         """
         return None
 
     def set_state(self, new_state: EventState, user: str = "monitor"):
         """Sets a new event state value, logging the change to the event history with a username"""
         if new_state == self.state:
             return
+        if self.state == EventState.CLOSED:
+            raise ClosedEventError
 
         old_state, self.state = self.state, new_state
         if (old_state, new_state) == (EventState.EMBRYONIC, EventState.OPEN):
             self.opened = now()
         self.add_history(f"state change {old_state.value} -> {new_state.value} ({user})")
         _logger.debug("id %s state %s -> %s by %s", self.id, old_state.value, new_state.value, user)
 
@@ -290,38 +300,46 @@
             return str(int(value.timestamp()))
         return str(value)
 
     def get_changed_fields(self, other: "Event") -> List[str]:
         """Compares this Event to another Event and returns a list of names of attributes that are different"""
         return [field for field in self.model_fields if getattr(other, field) != getattr(self, field)]
 
+    def dump_event_to_file(self, dir_name: str):
+        """Dumps the full event to a file in JSON format"""
+        pathlib.Path(dir_name).mkdir(parents=True, exist_ok=True)
+        filename = f"{dir_name}/{self.id}.json"
+        _logger.debug("dumping state to %s", filename)
+        with open(filename, "w") as statefile:
+            statefile.write(self.model_dump_json(exclude_none=True, indent=2))
+
 
 class PortStateEvent(Event):
     type: Literal["portstate"] = "portstate"
     port: Optional[str] = ""
     ifindex: Optional[int] = None
     portstate: Optional[InterfaceState] = None
     descr: Optional[str] = None
 
     @property
     def subindex(self) -> SubIndex:
-        return self.port
+        return self.ifindex
 
 
 class BGPEvent(Event):
     type: Literal["bgp"] = "bgp"
-    remote_address: Optional[IPAddress] = None
+    remote_addr: Optional[IPAddress] = None
     remote_as: Optional[int] = None
     peer_uptime: Optional[int] = None
-    operational_state: Optional[BGPOperState] = None
-    admin_status: Optional[BGPAdminStatus] = None
+    bgpos: Optional[BGPOperState] = None
+    bgpas: Optional[BGPAdminStatus] = None
 
     @property
     def subindex(self) -> SubIndex:
-        return self.remote_address
+        return self.remote_addr
 
 
 class BFDEvent(Event):
     type: Literal["bfd"] = "bfd"
     ifindex: Optional[int] = None
     bfdstate: Optional[BFDSessState] = None
     bfdix: Optional[int] = None
```

### Comparing `Zino-2.0.0a1/src/zino/tasks/__init__.py` & `Zino-2.0.0a2/src/zino/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/tasks/addrs.py` & `Zino-2.0.0a2/src/zino/tasks/addrs.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/tasks/bfdtask.py` & `Zino-2.0.0a2/src/zino/tasks/bfdtask.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import ipaddress
 import logging
-from typing import Dict, Literal
+from typing import Dict
 
 from zino.oid import OID
 from zino.scheduler import get_scheduler
 from zino.snmp import SparseWalkResponse
-from zino.statemodels import BFDEvent, BFDSessState, BFDState, IPAddress, Port
+from zino.statemodels import BFDEvent, BFDSessState, BFDState, Port
 from zino.tasks.task import Task
+from zino.utils import parse_ip
 
 _log = logging.getLogger(__name__)
 
 # IfDescr as key
 DescrBFDStates = Dict[str, BFDState]
 # IfIndex as key
 IndexBFDStates = Dict[int, BFDState]
@@ -18,23 +18,21 @@
 
 class BFDTask(Task):
     JUNIPER_BFD_COLUMNS = [
         ("BFD-STD-MIB", "bfdSessState"),
         ("JUNIPER-BFD-MIB", "jnxBfdSessIntfName"),  # This should match IfDescr from the IF-MIB
         ("BFD-STD-MIB", "bfdSessDiscriminator"),
         ("BFD-STD-MIB", "bfdSessAddr"),
-        ("BFD-STD-MIB", "bfdSessAddrType"),
     ]
 
     CISCO_BFD_COLUMNS = [
         ("CISCO-IETF-BFD-MIB", "ciscoBfdSessState"),
         ("CISCO-IETF-BFD-MIB", "ciscoBfdSessInterface"),  # This should match IfIndex from the IF-MIB
         ("CISCO-IETF-BFD-MIB", "ciscoBfdSessDiscriminator"),
         ("CISCO-IETF-BFD-MIB", "ciscoBfdSessAddr"),
-        ("CISCO-IETF-BFD-MIB", "ciscoBfdSessAddrType"),
     ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._scheduler = get_scheduler()
 
     async def run(self):
@@ -70,16 +68,17 @@
         event.polladdr = self.device.address
         event.priority = self.device.priority
         event.bfdstate = new_state.session_state
         event.bfdix = new_state.session_index
         event.bfddiscr = new_state.session_discr
         event.bfdaddr = new_state.session_addr
 
-        log = f"Port {port.ifdescr} changed BFD state from {port.bfd_state.session_state} to {new_state.session_state}"
-        event.add_log(log)
+        log = f"changed BFD state from {port.bfd_state.session_state} to {new_state.session_state}"
+        event.lastevent = log
+        event.add_log(f"Port {port.ifdescr}" + log)
         self.state.events.commit(event)
 
     async def _poll_juniper(self) -> DescrBFDStates:
         bfd_rows = await self.snmp.sparsewalk(*self.JUNIPER_BFD_COLUMNS)
         bfd_states = self._parse_juniper_rows(bfd_rows)
         return bfd_states
 
@@ -89,15 +88,14 @@
         for index, row in bfd_rows.items():
             interface_name = row["jnxBfdSessIntfName"]
             bfd_state = self._parse_row(
                 index,
                 row["bfdSessState"],
                 row["bfdSessDiscriminator"],
                 row["bfdSessAddr"],  # This is a string representing hexadecimals (ex "0x7f000001")
-                row["bfdSessAddrType"],
             )
             bfd_states[interface_name] = bfd_state
         return bfd_states
 
     async def _poll_cisco(self) -> IndexBFDStates:
         bfd_rows = await self.snmp.sparsewalk(*self.CISCO_BFD_COLUMNS)
         bfd_states = self._parse_cisco_rows(bfd_rows)
@@ -109,40 +107,27 @@
         for index, row in bfd_rows.items():
             ifindex = row["ciscoBfdSessInterface"]
             bfd_state = self._parse_row(
                 index,
                 row["ciscoBfdSessState"],
                 row["ciscoBfdSessDiscriminator"],
                 row["ciscoBfdSessAddr"],  # This is a string representing hexadecimals (ex "0x7f000001")
-                row["ciscoBfdSessAddrType"],
             )
             bfd_states[ifindex] = bfd_state
         return bfd_states
 
-    def _parse_row(self, index: OID, state: str, discr: int, addr: str, addr_type: str) -> BFDState:
+    def _parse_row(self, index: OID, state: str, discr: int, addr: str) -> BFDState:
         try:
-            stripped_hexstring = addr.replace("0x", "")
-            addr_bytes = bytes.fromhex(stripped_hexstring)
-            ipaddr = self._convert_address(addr_bytes, addr_type)
+            ipaddr = parse_ip(addr)
         except ValueError as e:
             _log.error(f"Error converting addr {addr} to an IP address on device {self.device.name}: {e}")
             ipaddr = None
 
         # convert from OID object to int
         session_index = int(index[0])
         bfd_state = BFDState(
             session_state=BFDSessState(state),
             session_index=session_index,
             session_discr=discr,
             session_addr=ipaddr,
         )
         return bfd_state
-
-    @classmethod
-    def _convert_address(cls, address: bytes, address_type: Literal["ipv4", "ipv6"]) -> IPAddress:
-        """Converts bytes to either an ipv4 or ipv6 address"""
-        if address_type == "ipv4":
-            return ipaddress.IPv4Address(address)
-        elif address_type == "ipv6":
-            return ipaddress.IPv6Address(address)
-        else:
-            raise ValueError("address_type must be either ipv4 or ipv6")
```

### Comparing `Zino-2.0.0a1/src/zino/tasks/bgpstatemonitortask.py` & `Zino-2.0.0a2/src/zino/tasks/bgpstatemonitortask.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import logging
-from dataclasses import dataclass
-from ipaddress import ip_address
-from typing import Any, Iterable, Optional
-
-from pyasn1.type.univ import OctetString
+from dataclasses import dataclass, replace
+from typing import Iterable, Optional
 
 from zino.snmp import SparseWalkResponse
 from zino.statemodels import (
     BGPAdminStatus,
     BGPEvent,
     BGPOperState,
     BGPPeerSession,
     BGPStyle,
     IPAddress,
 )
 from zino.tasks.task import Task
+from zino.utils import parse_ip
 
 _logger = logging.getLogger(__name__)
 
 TIME_BEFORE_OPER_DOWN_ALERT = 600
 
 JUNIPER_TRANSLATION_MAP = [
     ("peer_state", "jnxBgpM2PeerState"),
@@ -88,18 +86,16 @@
             bgp_info = await self._get_cisco_bgp_info()
         elif bgp_style == BGPStyle.GENERAL:
             bgp_info = await self._get_general_bgp_info()
 
         if not bgp_info:
             return
 
-        bgp_info = self._fixup_ip_addresses(bgp_info=bgp_info)
-
-        for result in bgp_info.values():
-            self._update_single_bgp_entry(row=result, local_as=local_as, uptime=uptime)
+        for result in bgp_info:
+            self._update_single_bgp_entry(data=result, local_as=local_as, uptime=uptime)
 
     async def _get_bgp_style(self) -> Optional[BGPStyle]:
         if await self.snmp.subtree_is_supported("BGP4-V2-MIB-JUNIPER", "jnxBgpM2"):
             return BGPStyle.JUNIPER
 
         if await self.snmp.subtree_is_supported("CISCO-BGP4-MIB", "cbgpPeer2Table"):
             return BGPStyle.CISCO
@@ -116,15 +112,15 @@
             return
         response = await self.snmp.getnext(mib, object_name)
         if self.snmp.is_in_scope(response, (mib, object_name)):
             return response.value
         else:
             _logger.info(f"router {self.device.name} misses {object_name}")
 
-    async def _get_juniper_bgp_info(self) -> Optional[SparseWalkResponse]:
+    async def _get_juniper_bgp_info(self) -> Optional[list[BaseBGPRow]]:
         variables = (
             "jnxBgpM2PeerState",
             "jnxBgpM2PeerStatus",
             "jnxBgpM2PeerRemoteAddr",
             "jnxBgpM2PeerRemoteAs",
             "jnxBgpM2PeerFsmEstablishedTime",
         )
@@ -136,15 +132,15 @@
 
         juniper_bgp_info = self._transform_variables_from_specific_to_general(
             bgp_info=juniper_bgp_info, bgp_style=BGPStyle.JUNIPER
         )
 
         return juniper_bgp_info
 
-    async def _get_cisco_bgp_info(self) -> Optional[SparseWalkResponse]:
+    async def _get_cisco_bgp_info(self) -> Optional[list[BaseBGPRow]]:
         variables = (
             "cbgpPeer2State",
             "cbgpPeer2AdminStatus",
             "cbgpPeer2RemoteAs",
             "cbgpPeer2FsmEstablishedTime",
         )
 
@@ -158,15 +154,15 @@
 
         cisco_bgp_info = self._transform_variables_from_specific_to_general(
             bgp_info=cisco_bgp_info, bgp_style=BGPStyle.CISCO
         )
 
         return cisco_bgp_info
 
-    async def _get_general_bgp_info(self) -> Optional[SparseWalkResponse]:
+    async def _get_general_bgp_info(self) -> Optional[list[BaseBGPRow]]:
         variables = (
             "bgpPeerState",
             "bgpPeerAdminStatus",
             "bgpPeerRemoteAddr",
             "bgpPeerRemoteAs",
             "bgpPeerFsmEstablishedTime",
         )
@@ -196,15 +192,15 @@
             else:
                 cleaned_bgp_info[oid[1].prettyPrint()] = entry
 
         return cleaned_bgp_info
 
     def _transform_variables_from_specific_to_general(
         self, bgp_info: SparseWalkResponse, bgp_style: BGPStyle
-    ) -> SparseWalkResponse:
+    ) -> Optional[list[BaseBGPRow]]:
         if bgp_style == BGPStyle.JUNIPER:
             translation = JUNIPER_TRANSLATION_MAP
         elif bgp_style == BGPStyle.CISCO:
             translation = CISCO_TRANSLATION_MAP
         elif bgp_style == BGPStyle.GENERAL:
             translation = GENERAL_TRANSLATION_MAP
 
@@ -218,47 +214,28 @@
                 except KeyError:
                     missing_variables.append(specific_name)
 
         if missing_variables:
             _logger.info(f"router {self.device.name} misses BGP variables ({missing_variables})")
             return None
 
-        return generalized_bgp_info
+        results = list()
 
-    def _fixup_ip_addresses(self, bgp_info: SparseWalkResponse) -> SparseWalkResponse:
-        fixed_bgp_info = dict()
-        for oid, result in bgp_info.items():
+        # Fix up peer remote address and transform to BaseBGPRow
+        for result in generalized_bgp_info.values():
             try:
-                fixed_remote_address = self._fixup_ip_address(address=result["peer_remote_address"])
+                result["peer_remote_address"] = parse_ip(result["peer_remote_address"])
             except ValueError:
                 _logger.debug(f"{self.device_state.name}: Invalid peer_remote_address {result['peer_remote_address']}")
-                continue
-
-            fixed_bgp_info[oid] = result
-            fixed_bgp_info[oid]["peer_remote_address"] = fixed_remote_address
-
-        return fixed_bgp_info
-
-    def _fixup_ip_address(self, address: str) -> IPAddress:
-        if address.startswith("0x"):
-            if len(address) == 10:
-                # IPv4 address
-                address_str = ".".join((map(str, OctetString(hexValue=address[2:]).asNumbers())))
-            elif len(address) == 34:
-                # IPv6 address
-                address_str = ":".join(["".join(item) for item in zip(*[iter(address[2:])] * 4)])
             else:
-                raise ValueError(f"Input {address} could not be converted to IP address.")
-        else:
-            address_str = address
+                results.append(BaseBGPRow(**result))
 
-        return ip_address(address=address_str)
+        return results
 
-    def _update_single_bgp_entry(self, row: dict[str, Any], local_as: int, uptime: int):
-        data = BaseBGPRow(**row)
+    def _update_single_bgp_entry(self, data: BaseBGPRow, local_as: int, uptime: int):
         if data.peer_remote_address in BUGGY_REMOTE_ADDRESSES:
             return
 
         # Internal bgp sessions are not observed
         if local_as == data.peer_remote_as:
             return
 
@@ -275,15 +252,15 @@
     def _update_established_peer(self, data: BaseBGPRow, uptime: int):
         saved_bgp_peer_session = self.device_state.bgp_peers.get(data.peer_remote_address)
         if saved_bgp_peer_session and uptime >= saved_bgp_peer_session.uptime > data.peer_fsm_established_time:
             self._bgp_external_reset(data)
             _logger.debug(f"Noted external reset for {self.device_state.name}: {data.peer_remote_address}")
         else:
             event = self.state.events.get(self.device.name, data.peer_remote_address, BGPEvent)
-            if event and event.operational_state != "established":
+            if event and event.bgpos != "established":
                 self._bgp_external_reset(data)
                 _logger.debug(f"BGP session up for {self.device_state.name}: {data.peer_remote_address}")
 
     def _update_nonestablished_peer(self, data: BaseBGPRow, uptime: int):
         saved_bgp_peer_session = self.device_state.bgp_peers.get(data.peer_remote_address)
         if data.peer_admin_status in ["stop", "halted"]:
             if not saved_bgp_peer_session or saved_bgp_peer_session.admin_status != data.peer_admin_status:
@@ -312,90 +289,83 @@
                 _logger.debug(
                     f"Router {self.device_state.name} peer {data.peer_remote_address} AS {data.peer_remote_as} "
                     f"is {data.peer_state} (down), but uptime = {uptime}",
                 )
 
     def _bgp_external_reset(self, data: BaseBGPRow):
         event = self.state.events.get_or_create_event(self.device.name, data.peer_remote_address, BGPEvent)
-
-        event.operational_state = data.peer_state
-        event.admin_status = data.peer_admin_status
-        event.remote_address = data.peer_remote_address
-        event.remote_as = data.peer_remote_as
-        event.peer_uptime = data.peer_fsm_established_time
-        event.polladdr = self.device.address
-        event.priority = self.device.priority
+        event = self._update_bgp_event(event=event, data=data, last_event="peer was reset (now up)")
 
         log = f"{event.router} peer {data.peer_remote_address} AS {data.peer_remote_as} was reset (now up)"
         _logger.info(log)
         event.add_log(log)
 
         self.state.events.commit(event=event)
 
     def _bgp_admin_down(self, data: BaseBGPRow):
         event = self.state.events.get_or_create_event(self.device.name, data.peer_remote_address, BGPEvent)
 
-        if event.admin_status == data.peer_admin_status:
+        if event.bgpas == data.peer_admin_status:
             return
 
-        event.operational_state = "down"
-        event.admin_status = data.peer_admin_status
-        event.remote_address = data.peer_remote_address
-        event.remote_as = data.peer_remote_as
-        event.peer_uptime = 0
-        event.polladdr = self.device.address
-        event.priority = self.device.priority
+        copied_data = replace(data, peer_state="down", peer_fsm_established_time=0)
+        event = self._update_bgp_event(event=event, data=copied_data, last_event="peer is admin turned off")
 
         log = (
             f"{event.router} peer {data.peer_remote_address} AS {data.peer_remote_as} is admin turned off "
             f"({data.peer_admin_status})"
         )
         _logger.info(log)
         event.add_log(log)
 
         self.state.events.commit(event=event)
 
     def _bgp_admin_up(self, data: BaseBGPRow):
         event = self.state.events.get_or_create_event(self.device.name, data.peer_remote_address, BGPEvent)
 
-        if event.admin_status == data.peer_admin_status:
+        # No previous event, so no need to notify or event already up to date
+        if event.id is None or event.bgpas == data.peer_admin_status:
             return
 
-        event.operational_state = data.peer_state
-        event.admin_status = data.peer_admin_status
-        event.remote_address = data.peer_remote_address
-        event.remote_as = data.peer_remote_as
-        event.peer_uptime = 0
-        event.polladdr = self.device.address
-        event.priority = self.device.priority
+        copied_data = replace(data, peer_fsm_established_time=0)
+        event = self._update_bgp_event(event=event, data=copied_data, last_event="peer is now admin turned on")
 
         log = (
             f"{event.router} peer {data.peer_remote_address} AS {data.peer_remote_as} is now admin turned on "
             f"({data.peer_admin_status})"
         )
         _logger.info(log)
         event.add_log(log)
 
         self.state.events.commit(event=event)
 
     def _bgp_oper_down(self, data: BaseBGPRow):
         event = self.state.events.get_or_create_event(self.device.name, data.peer_remote_address, BGPEvent)
 
-        if event.operational_state == "down":
+        if event.bgpos == "down":
             return
 
-        event.operational_state = "down"
-        event.admin_status = data.peer_admin_status
-        event.remote_address = data.peer_remote_address
-        event.remote_as = data.peer_remote_as
-        event.peer_uptime = data.peer_fsm_established_time
-        event.polladdr = self.device.address
-        event.priority = self.device.priority
+        copied_data = replace(data, peer_state="down")
+        event = self._update_bgp_event(event=event, data=copied_data, last_event="peer is down")
 
         log = (
             f"{event.router} peer {data.peer_remote_address} AS {data.peer_remote_as} is down "
             f"({data.peer_admin_status})"
         )
         _logger.info(log)
         event.add_log(log)
 
         self.state.events.commit(event=event)
+
+    def _update_bgp_event(self, event: BGPEvent, data: BaseBGPRow, last_event: str) -> BGPEvent:
+        """Updates a given BGP event with the given BGP data"""
+
+        event.bgpos = data.peer_state
+        event.bgpas = data.peer_admin_status
+        event.remote_addr = data.peer_remote_address
+        event.remote_as = data.peer_remote_as
+        event.peer_uptime = data.peer_fsm_established_time
+        event.polladdr = self.device.address
+        event.priority = self.device.priority
+        event.lastevent = last_event
+
+        return event
```

### Comparing `Zino-2.0.0a1/src/zino/tasks/juniperalarmtask.py` & `Zino-2.0.0a2/src/zino/tasks/juniperalarmtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,13 +61,15 @@
         alarm_event = self.state.events.get_or_create_event(
             device_name=self.device.name,
             subindex=color,
             event_class=AlarmEvent,
         )
 
         old_alarm_count = alarm_event.alarm_count
+        log = f"alarms went from {old_alarm_count} to {alarm_count}"
         alarm_event.alarm_type = color
         alarm_event.alarm_count = alarm_count
-        alarm_event.add_log(f"{self.device.name} {color} alarms went from {old_alarm_count} to {alarm_count}")
+        alarm_event.add_log(f"{self.device.name} {color} {log}")
         alarm_event.polladdr = self.device.address
         alarm_event.priority = self.device.priority
+        alarm_event.lastevent = log
         self.state.events.commit(alarm_event)
```

### Comparing `Zino-2.0.0a1/src/zino/tasks/linkstatetask.py` & `Zino-2.0.0a2/src/zino/tasks/linkstatetask.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/tasks/reachabletask.py` & `Zino-2.0.0a2/src/zino/tasks/reachabletask.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/tasks/task.py` & `Zino-2.0.0a2/src/zino/tasks/task.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/src/zino/tasks/vendor.py` & `Zino-2.0.0a2/src/zino/tasks/vendor.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/api/auth_test.py` & `Zino-2.0.0a2/tests/api/auth_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/api/conftest.py` & `Zino-2.0.0a2/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/api/legacy_test.py` & `Zino-2.0.0a2/tests/api/legacy_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -368,14 +368,29 @@
 
         await authenticated_protocol.message_received("CASEIDS")
 
         output = authenticated_protocol.transport.data_buffer.getvalue()
         assert f"{event1.id}\r\n".encode() in output
         assert f"{event2.id}\r\n".encode() in output
 
+    @pytest.mark.asyncio
+    async def test_should_output_a_list_of_only_ids_of_non_closed_events(self, authenticated_protocol):
+        state = authenticated_protocol._state
+        event1 = state.events.create_event("foo", None, ReachabilityEvent)
+        state.events.commit(event1)
+        event2 = state.events.create_event("bar", None, ReachabilityEvent)
+        event2.state = EventState.CLOSED
+        state.events.commit(event2)
+
+        await authenticated_protocol.message_received("CASEIDS")
+
+        output = authenticated_protocol.transport.data_buffer.getvalue()
+        assert f"{event1.id}\r\n".encode() in output
+        assert f"{event2.id}\r\n".encode() not in output
+
 
 class TestZino1ServerProtocolVersionCommand:
     @pytest.mark.asyncio
     async def test_should_output_current_version(self, buffered_fake_transport):
         protocol = Zino1ServerProtocol()
         protocol.connection_made(buffered_fake_transport)
         protocol._authenticated = True  # fake authentication
@@ -521,14 +536,29 @@
 
         await authenticated_protocol.message_received(f"SETSTATE {event.id} invalidgabbagabba")
 
         output = authenticated_protocol.transport.data_buffer.getvalue().decode()
         assert "\r\n500 " in output
 
     @pytest.mark.asyncio
+    async def test_when_event_is_closed_it_should_output_error_and_stay_closed(self, authenticated_protocol):
+        state = authenticated_protocol._state
+        event = state.events.create_event("foo", None, ReachabilityEvent)
+        event.state = EventState.CLOSED
+        state.events.commit(event)
+
+        await authenticated_protocol.message_received(f"SETSTATE {event.id} ignored")
+
+        output = authenticated_protocol.transport.data_buffer.getvalue().decode()
+        assert "\r\n500 " in output
+
+        event = state.events[event.id]
+        assert event.state == EventState.CLOSED
+
+    @pytest.mark.asyncio
     async def test_when_caseid_and_state_is_valid_event_state_should_be_changed(self, authenticated_protocol):
         state = authenticated_protocol._state
         event = state.events.create_event("foo", None, ReachabilityEvent)
         state.events.commit(event)
 
         await authenticated_protocol.message_received(f"SETSTATE {event.id} ignored")
```

### Comparing `Zino-2.0.0a1/tests/api/notify_test.py` & `Zino-2.0.0a2/tests/api/notify_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,45 +69,57 @@
         protocol.goodbye()
         assert fake_transport.close.called
 
 
 class TestZino1NotificationProtocolBuildNotifications:
     def test_should_make_notifications_for_regular_changed_attrs(self, fake_event):
         protocol = Zino1NotificationProtocol()
+        protocol._state.events.events[fake_event.id] = fake_event
         event_copy = fake_event.model_copy(deep=True)
         event_copy.updated = now() + timedelta(seconds=5)
 
-        notifications = list(protocol.build_notifications(new_event=event_copy, old_event=fake_event))
+        notifications = list(
+            protocol.build_notifications(state=protocol._state, new_event=event_copy, old_event=fake_event)
+        )
         assert notifications == [Notification(event_id=42, change_type="attr", value="updated")]
 
     def test_should_make_notifications_for_log_changes(self, fake_event):
         protocol = Zino1NotificationProtocol()
+        protocol._state.events.events[fake_event.id] = fake_event
         event_copy = fake_event.model_copy(deep=True)
         event_copy.add_log("foo")
 
-        notifications = list(protocol.build_notifications(new_event=event_copy, old_event=fake_event))
+        notifications = list(
+            protocol.build_notifications(state=protocol._state, new_event=event_copy, old_event=fake_event)
+        )
         assert Notification(event_id=42, change_type="log", value=1) in notifications
 
     def test_should_make_notifications_for_history_changes(self, fake_event):
         protocol = Zino1NotificationProtocol()
+        protocol._state.events.events[fake_event.id] = fake_event
         event_copy = fake_event.model_copy(deep=True)
         event_copy.add_history("foo")
 
-        notifications = list(protocol.build_notifications(new_event=event_copy, old_event=fake_event))
+        notifications = list(
+            protocol.build_notifications(state=protocol._state, new_event=event_copy, old_event=fake_event)
+        )
         assert Notification(event_id=42, change_type="history", value=1) in notifications
 
     def test_should_make_notifications_for_state_changes(self, fake_event):
         protocol = Zino1NotificationProtocol()
+        protocol._state.events.events[fake_event.id] = fake_event
         event_copy = fake_event.model_copy(deep=True)
         event_copy.state = EventState.IGNORED
 
         old, new = fake_event.state.value, event_copy.state.value
         expected = f"{old} {new}"
 
-        notifications = list(protocol.build_notifications(new_event=event_copy, old_event=fake_event))
+        notifications = list(
+            protocol.build_notifications(state=protocol._state, new_event=event_copy, old_event=fake_event)
+        )
         assert Notification(event_id=42, change_type="state", value=expected) in notifications
 
 
 class TestZino1NotificationProtocolBuildAndSendNotifications:
     def test_should_send_notifications_only_to_tied_channels(self, event_loop, fake_event, changed_fake_event):
         server = ZinoServer(loop=event_loop, state=ZinoState())
         channel1 = Mock()
```

### Comparing `Zino-2.0.0a1/tests/bin_test.py` & `Zino-2.0.0a2/tests/bin_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/compat_test.py` & `Zino-2.0.0a2/tests/compat_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/config/polldevs_test.py` & `Zino-2.0.0a2/tests/config/polldevs_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/conftest.py` & `Zino-2.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/oid_test.py` & `Zino-2.0.0a2/tests/oid_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/scheduler_test.py` & `Zino-2.0.0a2/tests/scheduler_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import logging
 from unittest.mock import Mock, patch
 
 import pytest
 from apscheduler.jobstores.base import JobLookupError
 
 from zino import scheduler
+from zino.state import ZinoState
 
 
 class TestLoadPolldevs:
     @patch("zino.state.polldevs", dict())
+    @patch("zino.state.state", ZinoState())
     def test_should_return_all_new_devices_on_first_run(self, polldevs_conf):
         new_devices, deleted_devices = scheduler.load_polldevs(polldevs_conf)
         assert len(new_devices) > 0
         assert not deleted_devices
 
     @patch("zino.state.polldevs", dict())
+    @patch("zino.state.state", ZinoState())
     def test_should_return_deleted_devices_on_second_run(self, polldevs_conf, polldevs_conf_with_single_router):
         scheduler.load_polldevs(polldevs_conf)
         new_devices, deleted_devices = scheduler.load_polldevs(polldevs_conf_with_single_router)
         assert not new_devices
         assert len(deleted_devices) > 0
 
 
 class TestScheduleNewDevices:
     @patch("zino.state.polldevs", dict())
+    @patch("zino.state.state", ZinoState())
     def test_should_schedule_jobs_for_new_devices(self, polldevs_conf, mocked_scheduler):
         new_devices, _ = scheduler.load_polldevs(polldevs_conf)
         assert len(new_devices) > 0
 
         scheduler.schedule_new_devices(new_devices)
         assert mocked_scheduler.add_job.called
```

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bfd-up.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bfd-up.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-admin-down.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-admin-down.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-admin-up.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-admin-up.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-external-reset.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-external-reset.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-oper-down-short.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-oper-down-short.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp-oper-down.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp-oper-down.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/juniper-bgp.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/juniper-bgp.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/linksdown.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/linksdown.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/linksup.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/linksup.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_fixtures/public.snmprec` & `Zino-2.0.0a2/tests/snmp_fixtures/public.snmprec`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/snmp_test.py` & `Zino-2.0.0a2/tests/snmp_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/state_test.py` & `Zino-2.0.0a2/tests/state_test.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/statemodels_test.py` & `Zino-2.0.0a2/tests/statemodels_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import datetime
+import json
+import os
 
 import pytest
 
 from zino.statemodels import (
     DeviceState,
     DeviceStates,
     Event,
@@ -78,14 +80,23 @@
         copy = fake_event.model_copy(deep=True)
         copy.add_log("test")
         copy.updated = now() + datetime.timedelta(seconds=3)
 
         changed = fake_event.get_changed_fields(copy)
         assert set(changed) == {"log", "updated"}
 
+    def test_dump_event_to_file_should_dump_valid_json_to_file(self, tmp_path, fake_event):
+        fake_event.set_state(EventState.CLOSED)
+        fake_event.dump_event_to_file(tmp_path)
+
+        dumpfile = f"{tmp_path}/{fake_event.id}.json"
+        assert os.path.exists(dumpfile)
+        with open(dumpfile, "r") as data:
+            assert json.load(data)
+
 
 class TestLogEntryModelDumpLegacy:
     def test_should_be_prefixed_by_timestamp(self):
         entry = LogEntry(message="foobar")
         lines = entry.model_dump_legacy()
         timestamp, message = lines[0].split(" ")
```

### Comparing `Zino-2.0.0a1/tests/tasks/conftest.py` & `Zino-2.0.0a2/tests/tasks/conftest.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_addrs.py` & `Zino-2.0.0a2/tests/tasks/test_addrs.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_bfdtask.py` & `Zino-2.0.0a2/tests/tasks/test_bfdtask.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,26 @@
-import ipaddress
 from ipaddress import IPv4Address
 
 import pytest
 
 from zino.config.models import PollDevice
 from zino.oid import OID
 from zino.state import ZinoState
 from zino.statemodels import BFDEvent, BFDSessState, BFDState, Port
 from zino.tasks.bfdtask import BFDTask
 
 
-class TestConvertAddress:
-    def test_converts_bytes_to_correct_ipv6_address(self):
-        parsed_address = BFDTask._convert_address(
-            b"\x00\x00\x00\x00\x00\x00\x00\x00\00\x00\x00\x00\x00\x00\x00\x01",
-            "ipv6",
-        )
-        assert parsed_address == ipaddress.IPv6Address("::1")
-
-    def test_converts_bytes_to_correct_ipv4_address(self):
-        parsed_address = BFDTask._convert_address(b"\x7f\x00\x00\x01", "ipv4")
-        assert parsed_address == ipaddress.IPv4Address("127.0.0.1")
-
-    def test_fails_if_parsing_ipv4_as_ipv6(self):
-        with pytest.raises(ipaddress.AddressValueError):
-            BFDTask._convert_address(b"\x7f\x00\x00\x01", "ipv6")
-
-    def test_fails_if_parsing_ipv6_as_ipv4(self):
-        with pytest.raises(ipaddress.AddressValueError):
-            BFDTask._convert_address(
-                b"\x00\x00\x00\x00\x00\x00\x00\x00\00\x00\x00\x00\x00\x00\x00\x01",
-                "ipv4",
-            )
-
-    def test_fails_if_address_type_is_invalid(self):
-        with pytest.raises(ValueError):
-            BFDTask._convert_address("\x7f\x00\x00\x01", "invalid")
-
-
 class TestJuniper:
     @pytest.mark.parametrize("task", ["juniper-bfd-up"], indirect=True)
     def test_parse_row_creates_correct_bfd_state(self, task, bfd_state):
         state = task._parse_row(
             OID(f".{bfd_state.session_index}"),
             "up",
             bfd_state.session_discr,
             "0x7f000001",
-            "ipv4",
         )
         assert state == bfd_state
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize("task", ["juniper-bfd-up"], indirect=True)
     async def test_poll_juniper_returns_correct_ifdescr_to_state_mapping(self, task, bfd_state, device_port):
         result = await task._poll_juniper()
```

### Comparing `Zino-2.0.0a1/tests/tasks/test_bgpstatemonitortask.py` & `Zino-2.0.0a2/tests/tasks/test_bgpstatemonitortask.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from ipaddress import IPv4Address, IPv6Address
+from ipaddress import IPv4Address
 
 import pytest
 
 from zino.config.models import PollDevice
 from zino.state import ZinoState
 from zino.statemodels import (
     BGPAdminStatus,
@@ -47,17 +47,17 @@
         await task.run()
         # check if state has been updated to reflect state defined in .snmprec
         assert task.device_state.bgp_peers[PEER_ADDRESS].admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
         assert task.device_state.bgp_peers[PEER_ADDRESS].oper_state == BGPOperState.ESTABLISHED
         # check that the correct event has been created
         event = task.state.events.get(device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent)
         assert event
-        assert event.admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
-        assert event.operational_state == BGPOperState.ESTABLISHED
-        assert event.remote_address == PEER_ADDRESS
+        assert event.bgpas in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
+        assert event.bgpos == BGPOperState.ESTABLISHED
+        assert event.remote_addr == PEER_ADDRESS
         assert event.remote_as == DEFAULT_REMOTE_AS
         assert event.peer_uptime == DEFAULT_UPTIME
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize(
         "task", ["general-bgp-external-reset", "cisco-bgp-external-reset", "juniper-bgp-external-reset"], indirect=True
     )
@@ -65,32 +65,32 @@
         """Tests that the oper down event should be updated if a BGP connection to a device reports that their
         oper_state has changed back to established
         """
         # create admin down event
         event = task.state.events.get_or_create_event(
             device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent
         )
-        event.operational_state = BGPOperState.DOWN
-        event.admin_status = BGPAdminStatus.STOP
-        event.remote_address = PEER_ADDRESS
+        event.bgpos = BGPOperState.DOWN
+        event.bgpas = BGPAdminStatus.STOP
+        event.remote_addr = PEER_ADDRESS
         event.remote_as = DEFAULT_REMOTE_AS
         event.peer_uptime = 0
         task.state.events.commit(event=event)
 
         await task.run()
 
         # check if state has been updated to reflect state defined in .snmprec
         assert task.device_state.bgp_peers[PEER_ADDRESS].admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
         assert task.device_state.bgp_peers[PEER_ADDRESS].oper_state == BGPOperState.ESTABLISHED
         # check that the correct event has been created
         event = task.state.events.get(device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent)
         assert event
-        assert event.admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
-        assert event.operational_state == BGPOperState.ESTABLISHED
-        assert event.remote_address == PEER_ADDRESS
+        assert event.bgpas in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
+        assert event.bgpos == BGPOperState.ESTABLISHED
+        assert event.remote_addr == PEER_ADDRESS
         assert event.remote_as == DEFAULT_REMOTE_AS
         assert event.peer_uptime == DEFAULT_UPTIME
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize(
         "task", ["general-bgp-admin-down", "cisco-bgp-admin-down", "juniper-bgp-admin-down"], indirect=True
     )
@@ -107,17 +107,17 @@
         await task.run()
         # check if state has been updated to reflect state defined in .snmprec
         assert task.device_state.bgp_peers[PEER_ADDRESS].admin_status in [BGPAdminStatus.HALTED, BGPAdminStatus.STOP]
         assert task.device_state.bgp_peers[PEER_ADDRESS].oper_state != BGPOperState.ESTABLISHED
         # check that the correct event has been created
         event = task.state.events.get(device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent)
         assert event
-        assert event.admin_status in [BGPAdminStatus.HALTED, BGPAdminStatus.STOP]
-        assert event.operational_state == BGPOperState.DOWN
-        assert event.remote_address == PEER_ADDRESS
+        assert event.bgpas in [BGPAdminStatus.HALTED, BGPAdminStatus.STOP]
+        assert event.bgpos == BGPOperState.DOWN
+        assert event.remote_addr == PEER_ADDRESS
         assert event.remote_as == DEFAULT_REMOTE_AS
         assert event.peer_uptime == 0
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize(
         "task", ["general-bgp-admin-up", "cisco-bgp-admin-up", "juniper-bgp-admin-up"], indirect=True
     )
@@ -129,24 +129,35 @@
         task.device_state.bgp_peers = {
             PEER_ADDRESS: BGPPeerSession(
                 uptime=DEFAULT_UPTIME,
                 admin_status=BGPAdminStatus.STOP,
                 oper_state=BGPOperState.IDLE,
             )
         }
+        # create admin down event
+        event = task.state.events.get_or_create_event(
+            device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent
+        )
+        event.bgpos = BGPOperState.DOWN
+        event.bgpas = BGPAdminStatus.STOP
+        event.remote_addr = PEER_ADDRESS
+        event.remote_as = DEFAULT_REMOTE_AS
+        event.peer_uptime = 0
+        task.state.events.commit(event=event)
+
         await task.run()
         # check if state has been updated to reflect state defined in .snmprec
         assert task.device_state.bgp_peers[PEER_ADDRESS].admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
         assert task.device_state.bgp_peers[PEER_ADDRESS].oper_state != BGPOperState.ESTABLISHED
         # check that the correct event has been created
         event = task.state.events.get(device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent)
         assert event
-        assert event.admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
-        assert event.operational_state == BGPOperState.IDLE
-        assert event.remote_address == PEER_ADDRESS
+        assert event.bgpas in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
+        assert event.bgpos == BGPOperState.IDLE
+        assert event.remote_addr == PEER_ADDRESS
         assert event.remote_as == DEFAULT_REMOTE_AS
         assert event.peer_uptime == 0
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize(
         "task", ["general-bgp-oper-down", "cisco-bgp-oper-down", "juniper-bgp-oper-down"], indirect=True
     )
@@ -162,17 +173,17 @@
         }
         await task.run()
         # check if state has been updated to reflect state defined in .snmprec
         assert task.device_state.bgp_peers[PEER_ADDRESS].oper_state != BGPOperState.ESTABLISHED
         # check that the correct event has been created
         event = task.state.events.get(device_name=task.device.name, subindex=PEER_ADDRESS, event_class=BGPEvent)
         assert event
-        assert event.admin_status in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
-        assert event.operational_state == BGPOperState.DOWN
-        assert event.remote_address == PEER_ADDRESS
+        assert event.bgpas in [BGPAdminStatus.RUNNING, BGPAdminStatus.START]
+        assert event.bgpos == BGPOperState.DOWN
+        assert event.remote_addr == PEER_ADDRESS
         assert event.remote_as == DEFAULT_REMOTE_AS
         assert event.peer_uptime == 1000000
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize(
         "task",
         ["general-bgp-oper-down-short", "cisco-bgp-oper-down-short", "juniper-bgp-oper-down-short"],
@@ -248,46 +259,14 @@
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize("task", ["public"], indirect=True)
     async def test_get_local_as_returns_none_for_non_existent_local_as_with_juniper_bgp_style(self, task):
         assert (await task._get_local_as(bgp_style=BGPStyle.JUNIPER)) is None
 
 
-class TestFixupIPAddress:
-    @pytest.mark.parametrize("task", ["general-bgp"], indirect=True)
-    def test_can_parse_ipv4_starting_with_0x(self, task):
-        encoded_address = "0x7f000001"
-        decoded_address = task._fixup_ip_address(encoded_address)
-        assert decoded_address == IPv4Address("127.0.0.1")
-
-    @pytest.mark.parametrize("task", ["general-bgp"], indirect=True)
-    def test_can_parse_ipv6_starting_with_0x(self, task):
-        encoded_address = "0x13c7db1c4430c8266333aed0e6053a3b"
-        decoded_address = task._fixup_ip_address(encoded_address)
-        assert decoded_address == IPv6Address("13c7:db1c:4430:c826:6333:aed0:e605:3a3b")
-
-    @pytest.mark.parametrize("task", ["general-bgp"], indirect=True)
-    def test_can_parse_ipv4_in_string_format(self, task):
-        string_address = "127.0.0.1"
-        decoded_address = task._fixup_ip_address(string_address)
-        assert decoded_address == IPv4Address(string_address)
-
-    @pytest.mark.parametrize("task", ["general-bgp"], indirect=True)
-    def test_can_parse_ipv6_in_string_format(self, task):
-        string_address = "13c7:db1c:4430:c826:6333:aed0:e605:3a3b"
-        decoded_address = task._fixup_ip_address(string_address)
-        assert decoded_address == IPv6Address(string_address)
-
-    @pytest.mark.parametrize("task", ["general-bgp"], indirect=True)
-    def test_parsing_invalid_ip_address_raises_error(self, task):
-        string_address = "abc"
-        with pytest.raises(ValueError):
-            task._fixup_ip_address(string_address)
-
-
 @pytest.fixture
 def task(request, snmpsim, snmp_test_port):
     device = PollDevice(
         name="buick.lab.example.org",
         address="127.0.0.1",
         community=request.param,
         port=snmp_test_port,
```

### Comparing `Zino-2.0.0a1/tests/tasks/test_juniperalarmtask.py` & `Zino-2.0.0a2/tests/tasks/test_juniperalarmtask.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_linkstatetask.py` & `Zino-2.0.0a2/tests/tasks/test_linkstatetask.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_reachabletask.py` & `Zino-2.0.0a2/tests/tasks/test_reachabletask.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_run_all_tasks.py` & `Zino-2.0.0a2/tests/tasks/test_run_all_tasks.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_task.py` & `Zino-2.0.0a2/tests/tasks/test_task.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tests/tasks/test_vendor.py` & `Zino-2.0.0a2/tests/tasks/test_vendor.py`

 * *Files identical despite different names*

### Comparing `Zino-2.0.0a1/tox.ini` & `Zino-2.0.0a2/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     3.11: py311
 
 [testenv]
 deps =
     pytest
     pytest-asyncio<0.22.0
     pytest-cov
+    pytest-timeout
     snmpsim
     pyasn1<0.5.0
     retry
 
 setenv =
     LC_ALL=C.UTF-8
     LANG=C.UTF-8
```

