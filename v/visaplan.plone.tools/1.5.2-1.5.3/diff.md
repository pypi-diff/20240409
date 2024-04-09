# Comparing `tmp/visaplan.plone.tools-1.5.2.tar.gz` & `tmp/visaplan.plone.tools-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.plone.tools-1.5.2.tar", last modified: Thu Mar 21 11:25:53 2024, max compression
+gzip compressed data, was "dist/visaplan.plone.tools-1.5.3.tar", last modified: Tue Apr  9 16:29:58 2024, max compression
```

## Comparing `visaplan.plone.tools-1.5.2.tar` & `visaplan.plone.tools-1.5.3.tar`

### file list

```diff
@@ -1,115 +1,109 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2019-11-06 14:05:55.000000 visaplan.plone.tools-1.5.2/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      615 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/Makefile
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5494 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/conf.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      103 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/conf.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      501 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/index.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      822 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/make.bat
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      102 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/modules.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      106 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/setup.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.plone.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      181 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.plone.tools.functions.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      258 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.plone.tools.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      209 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      759 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      839 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_data.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8596 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_group.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3413 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_group_pio.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8675 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_helpers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      687 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_imports.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8339 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_membership.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5968 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_user.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3418 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_user_pio.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5483 2022-01-20 18:17:48.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_group.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3215 2022-01-20 14:33:44.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_membership.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3431 2022-01-20 14:32:17.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_user.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3114 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    19711 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_args.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2416 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_attr.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12467 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_decorator.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1668 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_exc.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12815 2024-02-09 10:40:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_get_object.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4632 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_gs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7747 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_make_folder.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1224 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_misc.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    22871 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_o_tools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4622 2023-11-29 09:56:09.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_query.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13552 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_reindex.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8117 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_rename.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5543 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_roles.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1563 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_switch.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    32598 2024-02-09 10:40:18.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_tree.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1651 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_types.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10604 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_uid.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3153 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_watch.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24264 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_workflow.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       45 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1137 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2143 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/check-blobs.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      884 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13282 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/fixblobs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1557 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at0.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      921 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at1.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13055 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at2.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      916 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at3.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3023 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at4.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3909 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at5.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      539 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at6.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3108 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx4.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3601 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx5.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1275 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_have.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      760 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_idxnames.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1317 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/attools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8290 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/brains.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    15313 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/cfg.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      202 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18151 2024-03-21 11:22:18.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18047 2024-01-22 12:38:47.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py.orig
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1859 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/decorators.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      346 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/dxtools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5190 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/env.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    30839 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/forms.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5041 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/functions.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1692 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/indexes.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10338 2024-02-09 10:40:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/lock.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7325 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/log.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3539 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1799 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock_cfg.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/profiles.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    11691 2024-02-09 10:35:17.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/search.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4919 2023-11-29 09:56:09.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/seo.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1452 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setuphandlers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      291 2022-12-06 12:33:06.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/strings.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12714 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/zcmlgen.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.5.2/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    28324 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3607 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-03-25 17:32:23.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      116 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    15722 2024-03-21 11:24:19.000000 visaplan.plone.tools-1.5.2/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-14 11:15:58.000000 visaplan.plone.tools-1.5.2/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3933 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      218 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/TODO.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9342 2020-09-04 22:52:51.000000 visaplan.plone.tools-1.5.2/long-description.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1597 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7604 2024-03-21 11:20:35.000000 visaplan.plone.tools-1.5.2/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    28324 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2019-11-06 14:05:55.000000 visaplan.plone.tools-1.5.3/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      615 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/Makefile
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5494 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/conf.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      103 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/conf.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      501 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/index.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      822 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/make.bat
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      102 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/modules.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      106 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/setup.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/visaplan.plone.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      181 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/visaplan.plone.tools.functions.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      258 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/visaplan.plone.tools.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      209 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/docs/visaplan.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      759 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      839 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_data.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8596 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_group.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3413 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_group_pio.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8675 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_helpers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      687 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_imports.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8339 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_membership.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5968 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_user.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3418 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_user_pio.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5483 2022-01-20 18:17:48.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/_group.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3215 2022-01-20 14:33:44.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/_membership.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3431 2022-01-20 14:32:17.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/_user.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3360 2024-04-09 15:54:33.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    19711 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_args.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2416 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_attr.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12822 2024-04-09 16:01:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_decorator.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1668 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_exc.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12815 2024-02-09 10:40:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_get_object.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4632 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_gs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7747 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_make_folder.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1224 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_misc.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    22871 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_o_tools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4622 2023-11-29 09:56:09.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_query.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13552 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_reindex.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8117 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_rename.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5543 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_roles.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1563 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_switch.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    32598 2024-02-09 10:40:18.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_tree.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1651 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_types.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10604 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_uid.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3153 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_watch.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    24264 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_workflow.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1557 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at0.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      921 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at1.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13055 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at2.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      916 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at3.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3023 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at4.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3909 2024-03-21 11:26:40.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at5.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      539 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at6.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3108 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_dx4.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3601 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_dx5.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1275 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_have.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      760 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_idxnames.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1317 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/attools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8290 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/brains.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    15313 2024-04-09 14:50:42.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/cfg.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      116 2024-04-09 14:49:43.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18151 2024-03-21 11:26:40.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/context.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18047 2024-01-22 12:38:47.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/context.py.orig
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1859 2024-03-21 11:26:40.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/decorators.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      346 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/dxtools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5190 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/env.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    30839 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/forms.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5041 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/functions.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1692 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/indexes.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10338 2024-02-09 10:40:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/lock.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7325 2024-04-09 14:50:42.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/log.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3539 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/mock.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1799 2024-04-09 14:50:42.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/mock_cfg.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      910 2024-04-09 14:49:43.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/profiles.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11691 2024-02-09 10:35:17.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/search.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4919 2023-11-29 09:56:09.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/seo.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1440 2024-04-09 14:49:43.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setuphandlers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      291 2022-12-06 12:33:06.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/strings.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12714 2024-04-09 14:50:42.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/zcmlgen.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.5.3/src/visaplan/plone/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.5.3/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    29283 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3367 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-03-25 17:32:23.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      116 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    16401 2024-04-09 16:24:03.000000 visaplan.plone.tools-1.5.3/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.3/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-14 11:15:58.000000 visaplan.plone.tools-1.5.3/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3933 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      218 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.3/TODO.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2024-04-09 14:49:43.000000 visaplan.plone.tools-1.5.3/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     9342 2020-09-04 22:52:51.000000 visaplan.plone.tools-1.5.3/long-description.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1597 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7604 2024-04-03 13:37:29.000000 visaplan.plone.tools-1.5.3/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    29283 2024-04-09 16:29:58.000000 visaplan.plone.tools-1.5.3/PKG-INFO
```

### Comparing `visaplan.plone.tools-1.5.2/docs/LICENSE.GPL` & `visaplan.plone.tools-1.5.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/docs/LICENSE.rst` & `visaplan.plone.tools-1.5.3/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/docs/Makefile` & `visaplan.plone.tools-1.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/docs/conf.py` & `visaplan.plone.tools-1.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/docs/make.bat` & `visaplan.plone.tools-1.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/__init__.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_data.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_data.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_group.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_group.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_group_pio.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_group_pio.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_helpers.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_helpers.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_imports.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_imports.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_membership.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_membership.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_user.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_user.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_user_pio.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/groups/_user_pio.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_group.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/_group.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_membership.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/_membership.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_user.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/infofact/_user.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/__init__.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,19 @@
         ## _args (Helferlein für **kwargs):
         'extract_object_and_brain', # --> (o, brain)
         'extract_object_or_brain',  # --> (o, brain=None)
         'extract_brain_or_object',  # --> (brain, o=None)
         ## _attr:
         'make_attribute_setter',
         ## _decorator.py:
-        'step',
-        'importStep',
+        'upgradeStep',
+        'installStep',
         'StepAborted',
+        ## ... deprecated names:
+        'step', 'importStep',
         ## _get_object:
         'make_object_getter',
         ## _make_folder:
         'make_subfolder_creator',
         ## _query:
         'make_query_extractor',
         'iterate_query',
@@ -58,15 +60,19 @@
 # Local imports:
 from visaplan.plone.tools.setup._args import (
     extract_brain_or_object,
     extract_object_and_brain,
     extract_object_or_brain,
     )
 from visaplan.plone.tools.setup._attr import make_attribute_setter
-from visaplan.plone.tools.setup._decorator import StepAborted, importStep, step
+from visaplan.plone.tools.setup._decorator import StepAborted, installStep, upgradeStep
+# deprecated names:
+from visaplan.plone.tools.setup._decorator import installStep as importStep
+from visaplan.plone.tools.setup._decorator import upgradeStep as step
+
 from visaplan.plone.tools.setup._get_object import make_object_getter
 from visaplan.plone.tools.setup._gs import load_and_cook, safe_context_id
 from visaplan.plone.tools.setup._make_folder import make_subfolder_creator
 from visaplan.plone.tools.setup._query import (
     getAllLanguages,
     iterate_query,
     make_query_extractor,
```

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_args.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_args.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_attr.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_attr.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_decorator.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- äöü vim: sw=4 sts=4 et tw=79
 """
-Decorators for upgrade steps
+Decorators for GenericSetup upgrade steps and handler functions
 
 Common functionality of the decorators provided by this module:
 
 - They expect the decorated function to accept a context and a logger argument.
   The logger argument might be omitted depending on the usage, so it is
   complemented by the decorator for this cases;
   thus, the decorated function doesn't need any code to handle a missing logger option.
@@ -29,35 +29,37 @@
 from visaplan.plone.tools.env import worker_name
 
 # Logging / Debugging:
 import logging
 
 __all__ = [
         # decorators:
-        'step',
-        'importStep',
+        'upgradeStep',  # inject a default logger (deprecated name: 'step')
+        'installStep',  # check for a marker file (deprecated name: 'importStep')
         # noch unfertig:
-        # 'upgrade_step',
+        # 'upgradeTo',
         'make_step_decorator',
         # exceptions:
         'StepAborted',
         ]
 
 
 class StepAborted(Exception):
     """
-    Vom Dekorator @step geworfen, wenn in einem Migrationsschritt eine
+    Vom Dekorator @upgradeStep geworfen, wenn in einem Migrationsschritt eine
     KeyBoard-Exception ausgelöst wurde
     """
 
 
-def step(func):
+def upgradeStep(func):
     """
     Dekorator für Migrationsschritte:
-    - ergänzt ggf. fehlendes logger-Argument
+    - ergänzt ein ggf. fehlendes logger-Argument
+      und
+    - verwendet dabei den Namen des Workers
     - stoppt die Zeit
     - (experimentell:)
       erlaubt das Weiterlaufen der Zope-Instanz auch nach manuellem Abbruch
       des Migrationsschritts
     """
     # da die def-Anweisung hier nicht ausgeführt wird, ist eine implizite
     # "Impfung" der verpackten Funktion mit zusätzlichen Variablen (wie z.B.
@@ -93,70 +95,71 @@
             delta = time() - _started
             logger.info('%(res)r <-- %(funcname)s (%(delta)5.2f seconds)', locals())
         return res
 
     return wrapper
 
 
-def importStep(marker_file, verbose=False):
+def installStep(marker_file, verbose=False):
     """
-    Return a decorator for importStep functions.
+    Return a decorator for functions which are constrained by a marker file:
+    the decorated function will be executed *only* if the given file is found.
 
     Options:
 
       marker_file -- relative path to a marker file (required)
 
              Note: This path is not (yet?) checked for existence,
                    but this might change in a future release!
 
       verbose -- enables some informational output (default: False)
 
-    Import steps are usually excecuted in the context of their own package only
-    and thus usually start with something like::
+    Some .setuphandlers functions are commonly executed in the context of their
+    own package only and thus usually start with something like::
 
       >>> if context.readDataFile('my.astonishing.addon-marker.txt') is None:
       ...    return                   # doctest: +SKIP
 
     The file in question is commonly located in some local directory
     in the package sources ('profiles/default/') relative to the module.
 
     For convenience, we provide a decorator which allows you to write things
     like::
 
-      >>> @importStep('profiles/default/my.astonishing.addon-marker.txt')
+      >>> @installStep('profiles/default/my.astonishing.addon-marker.txt')
       ... def setup_various(context):
       ...     portal = context.getSite()
       ...     do_fancy_things(portal)  # doctest: +SKIP
 
     That way you see the path to that file; but as the readDataFile method
     expects the filename only, it is shortened.
 
-    To prevent errors, the importStep won't accept anything callable by itself:
+    To prevent errors, the installStep won't accept anything callable by itself:
 
     >>> def some_function(context): pass
-    >>> importStep(some_function)   # doctest: +NORMALIZE_WHITESPACE
+    >>> installStep(some_function)   # doctest: +NORMALIZE_WHITESPACE
     Traceback (most recent call last):
       ...
     TypeError: This function doesn't decorate any function directly
                but expects the name of a marker file and
                *returns* the decorator!
 
-    We *always* want our importSteps to check a marker file, right?!
+    We *always* want our installSteps to check a marker file, right?!
     (If not, you wouldn't use our decorator -- if any at all!)
-    >>> importStep()   # doctest: +NORMALIZE_WHITESPACE
+    >>> installStep()   # doctest: +NORMALIZE_WHITESPACE
     Traceback (most recent call last):
       ...
-    TypeError: importStep() takes at least 1 argument (0 given)
+    TypeError: installStep() takes at least 1 argument (0 given)
 
     Other wrong usage should be prevented as well:
-    >>> importStep(None)   # doctest: +NORMALIZE_WHITESPACE
+    >>> installStep(None)   # doctest: +NORMALIZE_WHITESPACE
     Traceback (most recent call last):
       ...
     ValueError: Please specify the name of a marker file!
-    >>> importStep(0)   # doctest: +NORMALIZE_WHITESPACE
+    >>> installStep(0)   # doctest: +NORMALIZE_WHITESPACE
     Traceback (most recent call last):
       ...
     AttributeError: 'int' object has no attribute 'split'
 
     """
     if marker_file is None:
         raise ValueError('Please specify the name of a marker file!')
@@ -184,36 +187,36 @@
                 raise StepAborted
 
         return wrapper
 
     return my_decorator
 
 
-def upgrade_step(destination, **kwargs):
+def upgradeTo(destination, **kwargs):
     """
     Gib einen Dekorator zur einmaligen Verwendung zurück.
     Es wird als erstes Argument die Zielversion (destination)
     angegeben; weitere werden üblicherweise in einem Dict gesammelt:
 
     >>> deco_kwargs = {'package': __package__, 'module': __name__}
-    >>> @upgrade_step(1001, **deco_kwargs)  # doctest: +SKIP
+    >>> @upgradeTo(1001, **deco_kwargs)  # doctest: +SKIP
     ... def create_interesting_folder(context, logger):
     ...     pass
 
     Der Dekorator sorgt für das (je nach Aufruf fehlende) logger-Argument;
     protokolliert wird:
     - die Zielversion (destination)
     - der Name der Funktion
     - jeweils wenn übergeben:
       - der Name des Python-Packages (package)
       - der Name des Moduls (module)
       - die Revisionsnummer (rev), normalerweise als String
 
     Die Logik ist wie folgt:
-    - upgrade_step wird aufgerufen und verarbeitet die übergebenen Argumente,
+    - upgradeTo wird aufgerufen und verarbeitet die übergebenen Argumente,
       um eine Funktion mit einem Argument <func> zu erzeugen,
       die die übergebene Funktion dekoriert
     - die so generierte Funktion bekommt die letztlich zu dekorierende Funktion
       übergeben und gibt eine Wrapper-Funktion zurück, die folgendes tut:
       - sie erzeugt einen Logger, falls nicht übergeben,
         und ergänzt so das an die dekorierte Funktion übergebene logger-Argument;
       - sie protokolliert das Paket (sofern package übergeben; dringend
@@ -288,15 +291,15 @@
 
         return wrapper
     return make_wrapper()
 
 
 def make_step_decorator(**kwargs):
     """
-    Erzeuge einen Dekorator wie vorstehende Funktion --> step,
+    Erzeuge einen Dekorator wie vorstehende Funktion --> upgradeStep,
     aber ergänze bei der Protokollierung des Aufrufs, gemäß benannten
     Argumenten:
     - rev --> die svn-Revision des aufrufenden Moduls;
       z. B., wenn das svn:keyword "Revision" aktiv ist:
       >>> MODULE_REVISION = '$Revision: 31126 $'[8+3:-2]
     """
     rev = kwargs.pop('rev', 0)
```

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_exc.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_exc.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_get_object.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_get_object.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_gs.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_gs.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_make_folder.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_make_folder.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_misc.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_misc.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_o_tools.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_o_tools.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_query.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_query.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_reindex.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_reindex.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_rename.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_rename.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_roles.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_roles.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_switch.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_switch.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_tree.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_tree.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_types.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_types.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_uid.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_uid.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_watch.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_watch.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_workflow.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setup/_workflow.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at0.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at0.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at1.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at1.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at2.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at2.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at3.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at3.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at4.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at4.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at5.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at5.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at6.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_at6.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx4.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_dx4.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx5.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_dx5.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_have.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_have.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_idxnames.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/_idxnames.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/attools.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/attools.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/brains.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/brains.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/cfg.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/cfg.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/context.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py.orig` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/context.py.orig`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/decorators.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/env.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/env.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/forms.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/forms.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/functions.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/functions.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/indexes.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/indexes.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/lock.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/lock.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/log.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/log.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/mock.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock_cfg.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/mock_cfg.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/profiles.zcml` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/profiles.zcml`

 * *Files 17% similar despite different names*

```diff
@@ -14,8 +14,13 @@
                    (e.g. collective.metadataversion),
                    we don't delete our catalog metadata column 'metadata_version';
                    you can do so easily yourself.
                    "
       provides="Products.GenericSetup.interfaces.EXTENSION"
       />
 
+  <utility
+      factory=".setuphandlers.Hidden"
+      name="visaplan.plone.tools"
+      />
+
 </configure>
```

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/search.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/search.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/seo.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/seo.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setuphandlers.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/setuphandlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,39 +14,34 @@
 
 # Zope:
 from zope.interface import implementer
 
 # Plone:
 from Products.CMFPlone.interfaces import INonInstallable
 
-__all__ = [
-    'HiddenProfiles',
-    ]
-
 # ------------------------------------------------------ [ Daten ... [
-PROJECTNAME = 'visaplan.plone.tools'
-PROFILE_ID = PROJECTNAME + ':default'
-LOGGER_LABEL = PROJECTNAME + ': setuphandlers'
+PROJECTNAME = u'visaplan.plone.tools'
+PROFILE_ID = PROJECTNAME + u':default'
+LOGGER_LABEL = PROJECTNAME + u': setuphandlers'
 # ------------------------------------------------------ ] ... Daten ]
 
 
 @implementer(INonInstallable)
-class HiddenProfiles(object):
+class Hidden(object):
 
     def getNonInstallableProfiles(self):
         """Hide uninstall profile from site-creation and quickinstaller."""
         return [
-            PROJECTNAME + ':uninstall',
+            PROJECTNAME + u':uninstall',
         ]
 
-
-@implementer(INonInstallable)
-class HiddenProducts(object):
-
     def getNonInstallableProducts(self):
+        """
+        There is *nothing* in this package which could be "installed"!
+        """
         return [PROJECTNAME]
 
 
 def post_install(context):
     """Post install script"""
     # Do something at the end of the installation of this package.
```

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/zcmlgen.py` & `visaplan.plone.tools-1.5.3/src/visaplan/plone/tools/zcmlgen.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/PKG-INFO` & `visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.plone.tools
-Version: 1.5.2
+Version: 1.5.3
 Summary: General tools for Plone sites
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/plone.tools
 Project-URL: Documentation, https://pypi.org/project/visaplan.plone.tools
@@ -207,26 +207,59 @@
         
         1.6.0 (estimated)
         -----------------
         
         - Removal of all profile and zcml code
         
         
+        1.5.3 (2024-04-09)
+        ------------------
+        
+        New Features:
+        
+        - .setup:
+        
+          - new decorator ``upgradeStep()``; usage:
+        
+            .. code-block:: python
+        
+              @ungradeStep
+              def setup_various(context, logger):
+                  # just use the logger
+        
+            (the old name ``step`` is deprecated)
+        
+          - new decorator ``installStep()``; usage:
+        
+            .. code-block:: python
+        
+              @installStep('profiles/default/my.checked-marker.txt')
+              def setup_various(context):
+                  # jump right in!
+        
+            (the old name ``importStep`` is deprecated)
+        
+        Miscellaneous:
+        
+        - Registered a `Hidden` utility
+          to hide both the ``:uninstall`` profile and the entire package altogether
+          from Add-On installation forms.
+        
+        [tobiasherp]
+        
+        
         1.5.2 (2024-03-21)
         ------------------
         
         New Features:
         
         - .decorators: new decorator ``headless_json``
         
-        - .setup: new decorator ``importStep()``; usage::
-          
-            @importStep('profiles/default/my.checked-marker.txt')
-            def setup_various(context):
-                # jump right in!
+        - .setup: new decorator ``importStep()``
+          (please use the new name introduced in v1.5.3, if possible)
         
         Profile changes:
         
         - We try pretty hard to prevent people from activating this package!
           *NOTE:* Removal of any profile and ZCML code is scheduled for release 1.6.
         
         [tobiasherp]
@@ -321,25 +354,25 @@
         
         [tobiasherp]
         
         
         1.4.17 (2023-04-05)
         -------------------
         
-        New features: 
+        New features:
         
         - function .attools.can_be_html(field)
         
         [tobiasherp]
         
         
         1.4.16 (2023-03-24)
         -------------------
         
-        New features: 
+        New features:
         
         - New function `short_hostname` in .functions
         
         [tobiasherp]
         
         
         1.4.15 (2023-03-08)
@@ -348,15 +381,15 @@
         Bugfixes:
         
         - Py3K support fixes for
         
           - .functions.is_uid_shaped
           - .log.getLogSupport
         
-        New features: 
+        New features:
         
         - New (still tiny) module .seo for SEO support;
           for now, focused on structured data.
           Functions:
         
           - `parse_title`, returning a dict
         
@@ -383,17 +416,19 @@
         
         - Fixed a bug in .groups.groupinfo_factory(pretty);
           for this to work, we need visaplan.plone.groups.
         
         Improvements:
         
         - The label of the default logger of the ``@@step`` decorator
-          now includes the name of the worker, e.g. ``instance`` or ``client``
+          now includes the name of the worker, e.g. ``instance`` or ``client``.
+        
+          (*Note:* this decorator is renamed in release 1.5.3!)
         
-        New features: 
+        New features:
         
         - New `.env` module, providing the `worker_name()`
         
         [tobiasherp]
         
         
         1.4.12 (2022-02-15)
@@ -420,15 +455,15 @@
         1.4.10 (2022-02-03)
         -------------------
         
         Improvements:
         
         - Converted the .groups module in a subpackage
         
-        New features: 
+        New features:
         
         - New option `missing=False` for
         
           - .groups.groupinfo_factory
         
           If `True`, the resulting function creates an `existing` key,
           and for missing groups, the `group_title` is `None`;
@@ -447,15 +482,15 @@
         
         [tobiasherp]
         
         
         1.4.8 (2021-11-29)
         ------------------
         
-        New features: 
+        New features:
         
         - New ``.setup`` function `load_and_cook`, for use in GenericSetup upgrade steps
         
         [tobiasherp]
         
         
         1.4.7 (2021-11-17)
@@ -489,15 +524,15 @@
         
         Breaking changes:
         
         - Removed the .metadata module which had been added in release 1.4.2;
           we have collective.metadataversion_ now to replace it,
           storing the `metadata_version`_ value persistently in the registry.
         
-        New features: 
+        New features:
         
         - New .attools functions:
         
           - `get_first_text_as_html`
           - `get_all_texts`
           - `generate_all_texts`
         
@@ -544,15 +579,15 @@
         
         [tobiasherp]
         
         
         1.4.3 (2021-08-27)
         ------------------
         
-        New features: 
+        New features:
         
         - ``.search`` module:
         
           - New conversion utilities ...
         
             - `make_querystring_mangle`, a factory, to create
             - `mangleQueryString`, using
```

### Comparing `visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/SOURCES.txt` & `visaplan.plone.tools-1.5.3/src/visaplan.plone.tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -91,13 +91,8 @@
 src/visaplan/plone/tools/setup/_rename.py
 src/visaplan/plone/tools/setup/_roles.py
 src/visaplan/plone/tools/setup/_switch.py
 src/visaplan/plone/tools/setup/_tree.py
 src/visaplan/plone/tools/setup/_types.py
 src/visaplan/plone/tools/setup/_uid.py
 src/visaplan/plone/tools/setup/_watch.py
-src/visaplan/plone/tools/setup/_workflow.py
-src/visaplan/plone/tools/views/__init__.py
-src/visaplan/plone/tools/views/check-blobs-delete-selected.pt
-src/visaplan/plone/tools/views/check-blobs.pt
-src/visaplan/plone/tools/views/configure.zcml
-src/visaplan/plone/tools/views/fixblobs.py
+src/visaplan/plone/tools/setup/_workflow.py
```

### Comparing `visaplan.plone.tools-1.5.2/CHANGES.rst` & `visaplan.plone.tools-1.5.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,59 @@
 
 1.6.0 (estimated)
 -----------------
 
 - Removal of all profile and zcml code
 
 
+1.5.3 (2024-04-09)
+------------------
+
+New Features:
+
+- .setup:
+
+  - new decorator ``upgradeStep()``; usage:
+
+    .. code-block:: python
+
+      @ungradeStep
+      def setup_various(context, logger):
+          # just use the logger
+
+    (the old name ``step`` is deprecated)
+
+  - new decorator ``installStep()``; usage:
+
+    .. code-block:: python
+
+      @installStep('profiles/default/my.checked-marker.txt')
+      def setup_various(context):
+          # jump right in!
+
+    (the old name ``importStep`` is deprecated)
+
+Miscellaneous:
+
+- Registered a `Hidden` utility
+  to hide both the ``:uninstall`` profile and the entire package altogether
+  from Add-On installation forms.
+
+[tobiasherp]
+
+
 1.5.2 (2024-03-21)
 ------------------
 
 New Features:
 
 - .decorators: new decorator ``headless_json``
 
-- .setup: new decorator ``importStep()``; usage::
-  
-    @importStep('profiles/default/my.checked-marker.txt')
-    def setup_various(context):
-        # jump right in!
+- .setup: new decorator ``importStep()``
+  (please use the new name introduced in v1.5.3, if possible)
 
 Profile changes:
 
 - We try pretty hard to prevent people from activating this package!
   *NOTE:* Removal of any profile and ZCML code is scheduled for release 1.6.
 
 [tobiasherp]
@@ -119,25 +152,25 @@
 
 [tobiasherp]
 
 
 1.4.17 (2023-04-05)
 -------------------
 
-New features: 
+New features:
 
 - function .attools.can_be_html(field)
 
 [tobiasherp]
 
 
 1.4.16 (2023-03-24)
 -------------------
 
-New features: 
+New features:
 
 - New function `short_hostname` in .functions
 
 [tobiasherp]
 
 
 1.4.15 (2023-03-08)
@@ -146,15 +179,15 @@
 Bugfixes:
 
 - Py3K support fixes for
 
   - .functions.is_uid_shaped
   - .log.getLogSupport
 
-New features: 
+New features:
 
 - New (still tiny) module .seo for SEO support;
   for now, focused on structured data.
   Functions:
 
   - `parse_title`, returning a dict
 
@@ -181,17 +214,19 @@
 
 - Fixed a bug in .groups.groupinfo_factory(pretty);
   for this to work, we need visaplan.plone.groups.
 
 Improvements:
 
 - The label of the default logger of the ``@@step`` decorator
-  now includes the name of the worker, e.g. ``instance`` or ``client``
+  now includes the name of the worker, e.g. ``instance`` or ``client``.
+
+  (*Note:* this decorator is renamed in release 1.5.3!)
 
-New features: 
+New features:
 
 - New `.env` module, providing the `worker_name()`
 
 [tobiasherp]
 
 
 1.4.12 (2022-02-15)
@@ -218,15 +253,15 @@
 1.4.10 (2022-02-03)
 -------------------
 
 Improvements:
 
 - Converted the .groups module in a subpackage
 
-New features: 
+New features:
 
 - New option `missing=False` for
 
   - .groups.groupinfo_factory
 
   If `True`, the resulting function creates an `existing` key,
   and for missing groups, the `group_title` is `None`;
@@ -245,15 +280,15 @@
 
 [tobiasherp]
 
 
 1.4.8 (2021-11-29)
 ------------------
 
-New features: 
+New features:
 
 - New ``.setup`` function `load_and_cook`, for use in GenericSetup upgrade steps
 
 [tobiasherp]
 
 
 1.4.7 (2021-11-17)
@@ -287,15 +322,15 @@
 
 Breaking changes:
 
 - Removed the .metadata module which had been added in release 1.4.2;
   we have collective.metadataversion_ now to replace it,
   storing the `metadata_version`_ value persistently in the registry.
 
-New features: 
+New features:
 
 - New .attools functions:
 
   - `get_first_text_as_html`
   - `get_all_texts`
   - `generate_all_texts`
 
@@ -342,15 +377,15 @@
 
 [tobiasherp]
 
 
 1.4.3 (2021-08-27)
 ------------------
 
-New features: 
+New features:
 
 - ``.search`` module:
 
   - New conversion utilities ...
 
     - `make_querystring_mangle`, a factory, to create
     - `mangleQueryString`, using
```

### Comparing `visaplan.plone.tools-1.5.2/README.rst` & `visaplan.plone.tools-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/long-description.rst` & `visaplan.plone.tools-1.5.3/long-description.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/setup.cfg` & `visaplan.plone.tools-1.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/setup.py` & `visaplan.plone.tools-1.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.5.2/PKG-INFO` & `visaplan.plone.tools-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.plone.tools
-Version: 1.5.2
+Version: 1.5.3
 Summary: General tools for Plone sites
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/plone.tools
 Project-URL: Documentation, https://pypi.org/project/visaplan.plone.tools
@@ -207,26 +207,59 @@
         
         1.6.0 (estimated)
         -----------------
         
         - Removal of all profile and zcml code
         
         
+        1.5.3 (2024-04-09)
+        ------------------
+        
+        New Features:
+        
+        - .setup:
+        
+          - new decorator ``upgradeStep()``; usage:
+        
+            .. code-block:: python
+        
+              @ungradeStep
+              def setup_various(context, logger):
+                  # just use the logger
+        
+            (the old name ``step`` is deprecated)
+        
+          - new decorator ``installStep()``; usage:
+        
+            .. code-block:: python
+        
+              @installStep('profiles/default/my.checked-marker.txt')
+              def setup_various(context):
+                  # jump right in!
+        
+            (the old name ``importStep`` is deprecated)
+        
+        Miscellaneous:
+        
+        - Registered a `Hidden` utility
+          to hide both the ``:uninstall`` profile and the entire package altogether
+          from Add-On installation forms.
+        
+        [tobiasherp]
+        
+        
         1.5.2 (2024-03-21)
         ------------------
         
         New Features:
         
         - .decorators: new decorator ``headless_json``
         
-        - .setup: new decorator ``importStep()``; usage::
-          
-            @importStep('profiles/default/my.checked-marker.txt')
-            def setup_various(context):
-                # jump right in!
+        - .setup: new decorator ``importStep()``
+          (please use the new name introduced in v1.5.3, if possible)
         
         Profile changes:
         
         - We try pretty hard to prevent people from activating this package!
           *NOTE:* Removal of any profile and ZCML code is scheduled for release 1.6.
         
         [tobiasherp]
@@ -321,25 +354,25 @@
         
         [tobiasherp]
         
         
         1.4.17 (2023-04-05)
         -------------------
         
-        New features: 
+        New features:
         
         - function .attools.can_be_html(field)
         
         [tobiasherp]
         
         
         1.4.16 (2023-03-24)
         -------------------
         
-        New features: 
+        New features:
         
         - New function `short_hostname` in .functions
         
         [tobiasherp]
         
         
         1.4.15 (2023-03-08)
@@ -348,15 +381,15 @@
         Bugfixes:
         
         - Py3K support fixes for
         
           - .functions.is_uid_shaped
           - .log.getLogSupport
         
-        New features: 
+        New features:
         
         - New (still tiny) module .seo for SEO support;
           for now, focused on structured data.
           Functions:
         
           - `parse_title`, returning a dict
         
@@ -383,17 +416,19 @@
         
         - Fixed a bug in .groups.groupinfo_factory(pretty);
           for this to work, we need visaplan.plone.groups.
         
         Improvements:
         
         - The label of the default logger of the ``@@step`` decorator
-          now includes the name of the worker, e.g. ``instance`` or ``client``
+          now includes the name of the worker, e.g. ``instance`` or ``client``.
+        
+          (*Note:* this decorator is renamed in release 1.5.3!)
         
-        New features: 
+        New features:
         
         - New `.env` module, providing the `worker_name()`
         
         [tobiasherp]
         
         
         1.4.12 (2022-02-15)
@@ -420,15 +455,15 @@
         1.4.10 (2022-02-03)
         -------------------
         
         Improvements:
         
         - Converted the .groups module in a subpackage
         
-        New features: 
+        New features:
         
         - New option `missing=False` for
         
           - .groups.groupinfo_factory
         
           If `True`, the resulting function creates an `existing` key,
           and for missing groups, the `group_title` is `None`;
@@ -447,15 +482,15 @@
         
         [tobiasherp]
         
         
         1.4.8 (2021-11-29)
         ------------------
         
-        New features: 
+        New features:
         
         - New ``.setup`` function `load_and_cook`, for use in GenericSetup upgrade steps
         
         [tobiasherp]
         
         
         1.4.7 (2021-11-17)
@@ -489,15 +524,15 @@
         
         Breaking changes:
         
         - Removed the .metadata module which had been added in release 1.4.2;
           we have collective.metadataversion_ now to replace it,
           storing the `metadata_version`_ value persistently in the registry.
         
-        New features: 
+        New features:
         
         - New .attools functions:
         
           - `get_first_text_as_html`
           - `get_all_texts`
           - `generate_all_texts`
         
@@ -544,15 +579,15 @@
         
         [tobiasherp]
         
         
         1.4.3 (2021-08-27)
         ------------------
         
-        New features: 
+        New features:
         
         - ``.search`` module:
         
           - New conversion utilities ...
         
             - `make_querystring_mangle`, a factory, to create
             - `mangleQueryString`, using
```

