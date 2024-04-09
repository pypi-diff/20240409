# Comparing `tmp/kcweb-5.26.tar.gz` & `tmp/kcweb-5.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcweb-5.26.tar", last modified: Thu Apr  4 03:19:27 2024, max compression
+gzip compressed data, was "dist\kcweb-5.27.tar", last modified: Mon Apr  8 15:13:53 2024, max compression
```

## Comparing `kcweb-5.26.tar` & `kcweb-5.27.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:27.000000 kcweb-5.26/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/
--rw-rw-rw-   0        0        0    45674 2024-01-17 12:02:55.000000 kcweb-5.26/kcweb/app.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/common/
--rw-rw-rw-   0        0        0    63612 2024-04-04 02:45:24.000000 kcweb-5.26/kcweb/common/autoload.py
--rw-rw-rw-   0        0        0      151 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/common/globals.py
--rw-rw-rw-   0        0        0     4141 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/common/request.py
--rw-rw-rw-   0        0        0     2144 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/common/session.py
--rw-rw-rw-   0        0        0      120 2023-12-15 12:26:49.000000 kcweb-5.26/kcweb/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/config/
--rw-rw-rw-   0        0        0     6228 2024-04-04 03:19:13.000000 kcweb-5.26/kcweb/config/__init__.py
--rw-rw-rw-   0        0        0     2379 2024-01-17 11:56:40.000000 kcweb-5.26/kcweb/Events.py
--rw-rw-rw-   0        0        0    11440 2024-01-16 11:22:09.000000 kcweb-5.26/kcweb/kcweb.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/tpl/
--rw-rw-rw-   0        0        0     2124 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/tpl/err.html
--rw-rw-rw-   0        0        0      815 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/tpl/error.html
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/
--rw-rw-rw-   0        0        0     1077 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/app.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/cache/
--rw-rw-rw-   0        0        0    10456 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/cache/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/dateutil/
--rw-rw-rw-   0        0        0     2773 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/easter.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/dateutil/parser/
--rw-rw-rw-   0        0        0    13517 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/parser/isoparser.py
--rw-rw-rw-   0        0        0    59262 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/parser/_parser.py
--rw-rw-rw-   0        0        0     1787 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/parser/__init__.py
--rw-rw-rw-   0        0        0    25502 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/relativedelta.py
--rw-rw-rw-   0        0        0    68282 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/rrule.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/dateutil/tz/
--rw-rw-rw-   0        0        0    64282 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/tz/tz.py
--rw-rw-rw-   0        0        0    13305 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/tz/win.py
--rw-rw-rw-   0        0        0    13394 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/tz/_common.py
--rw-rw-rw-   0        0        0     2374 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/tz/_factories.py
--rw-rw-rw-   0        0        0      568 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/tz/__init__.py
--rw-rw-rw-   0        0        0       61 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/tzwin.py
--rw-rw-rw-   0        0        0     2034 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/dateutil/zoneinfo/
--rw-rw-rw-   0        0        0     1772 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/zoneinfo/rebuild.py
--rw-rw-rw-   0        0        0     6056 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/zoneinfo/__init__.py
--rw-rw-rw-   0        0        0      975 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/_common.py
--rw-rw-rw-   0        0        0      120 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/_version.py
--rw-rw-rw-   0        0        0      230 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/dateutil/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb/utill/db/
--rw-rw-rw-   0        0        0     6576 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/model.py
--rw-rw-rw-   0        0        0    12043 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/mongodb.py
--rw-rw-rw-   0        0        0    59544 2023-10-08 13:11:36.000000 kcweb-5.26/kcweb/utill/db/mysql.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:27.000000 kcweb-5.26/kcweb/utill/db/pymysql/
--rw-rw-rw-   0        0        0    10542 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/charset.py
--rw-rw-rw-   0        0        0    50320 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/connections.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:27.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/
--rw-rw-rw-   0        0        0      884 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/CLIENT.py
--rw-rw-rw-   0        0        0      713 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/COMMAND.py
--rw-rw-rw-   0        0        0     2296 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/CR.py
--rw-rw-rw-   0        0        0    12772 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/ER.py
--rw-rw-rw-   0        0        0      405 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/FIELD_TYPE.py
--rw-rw-rw-   0        0        0      229 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/FLAG.py
--rw-rw-rw-   0        0        0      345 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/SERVER_STATUS.py
--rw-rw-rw-   0        0        0        0 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/constants/__init__.py
--rw-rw-rw-   0        0        0    12646 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/converters.py
--rw-rw-rw-   0        0        0    17774 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/cursors.py
--rw-rw-rw-   0        0        0     3825 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/err.py
--rw-rw-rw-   0        0        0      681 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/optionfile.py
--rw-rw-rw-   0        0        0    12365 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/protocol.py
--rw-rw-rw-   0        0        0      380 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/times.py
--rw-rw-rw-   0        0        0      193 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/util.py
--rw-rw-rw-   0        0        0     7985 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/_auth.py
--rw-rw-rw-   0        0        0      502 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/_compat.py
--rw-rw-rw-   0        0        0     4183 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/_socketio.py
--rw-rw-rw-   0        0        0     4873 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/pymysql/__init__.py
--rw-rw-rw-   0        0        0    23069 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/sqlite copy.py
--rw-rw-rw-   0        0        0    21956 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/db/sqlite.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:27.000000 kcweb-5.26/kcweb/utill/filetype/
--rw-rw-rw-   0        0        0     2220 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/filetype.py
--rw-rw-rw-   0        0        0     2643 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/helpers.py
--rw-rw-rw-   0        0        0     2568 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/match.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:27.000000 kcweb-5.26/kcweb/utill/filetype/types/
--rw-rw-rw-   0        0        0    13116 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/archive.py
--rw-rw-rw-   0        0        0     3998 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/audio.py
--rw-rw-rw-   0        0        0      706 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/base.py
--rw-rw-rw-   0        0        0     2411 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/font.py
--rw-rw-rw-   0        0        0     6616 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/image.py
--rw-rw-rw-   0        0        0      961 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/isobmff.py
--rw-rw-rw-   0        0        0     5570 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/video.py
--rw-rw-rw-   0        0        0     1531 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/types/__init__.py
--rw-rw-rw-   0        0        0     1742 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/utils.py
--rw-rw-rw-   0        0        0      233 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/filetype/__init__.py
--rw-rw-rw-   0        0        0     3752 2023-01-10 15:00:12.000000 kcweb-5.26/kcweb/utill/http.py
--rw-rw-rw-   0        0        0    12030 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/queues.py
--rw-rw-rw-   0        0        0     8146 2023-12-11 09:13:59.000000 kcweb-5.26/kcweb/utill/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:27.000000 kcweb-5.26/kcweb/utill/rediss/
--rw-rw-rw-   0        0        0   150458 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/client.py
--rw-rw-rw-   0        0        0    48878 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/connection.py
--rw-rw-rw-   0        0        0     1057 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/exceptions.py
--rw-rw-rw-   0        0        0    11109 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/lock.py
--rw-rw-rw-   0        0        0    11644 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/sentinel.py
--rw-rw-rw-   0        0        0      699 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/utils.py
--rw-rw-rw-   0        0        0     4150 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/_compat.py
--rw-rw-rw-   0        0        0     1033 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/utill/rediss/__init__.py
--rw-rw-rw-   0        0        0       45 2022-05-13 07:34:10.000000 kcweb-5.26/kcweb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      579 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      106 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/requires.txt
--rw-rw-rw-   0        0        0     5346 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      339 2024-04-04 03:19:26.000000 kcweb-5.26/kcweb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2024-01-15 09:20:34.000000 kcweb-5.26/LICENSE
--rw-rw-rw-   0        0        0      579 2024-04-04 03:19:27.000000 kcweb-5.26/PKG-INFO
--rw-rw-rw-   0        0        0      678 2024-01-16 14:15:14.000000 kcweb-5.26/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 03:19:27.000000 kcweb-5.26/setup.cfg
--rw-rw-rw-   0        0        0     2781 2024-04-04 03:19:07.000000 kcweb-5.26/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/
+-rw-rw-rw-   0        0        0    45674 2024-01-17 12:02:55.000000 kcweb-5.27/kcweb/app.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/common/
+-rw-rw-rw-   0        0        0    63613 2024-04-08 14:26:59.000000 kcweb-5.27/kcweb/common/autoload.py
+-rw-rw-rw-   0        0        0      151 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/common/globals.py
+-rw-rw-rw-   0        0        0     4141 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/common/request.py
+-rw-rw-rw-   0        0        0     2144 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/common/session.py
+-rw-rw-rw-   0        0        0      120 2023-12-15 12:26:49.000000 kcweb-5.27/kcweb/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/config/
+-rw-rw-rw-   0        0        0     6228 2024-04-08 14:27:12.000000 kcweb-5.27/kcweb/config/__init__.py
+-rw-rw-rw-   0        0        0     2379 2024-01-17 11:56:40.000000 kcweb-5.27/kcweb/Events.py
+-rw-rw-rw-   0        0        0    11440 2024-01-16 11:22:09.000000 kcweb-5.27/kcweb/kcweb.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/tpl/
+-rw-rw-rw-   0        0        0     2124 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/tpl/err.html
+-rw-rw-rw-   0        0        0      815 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/tpl/error.html
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/
+-rw-rw-rw-   0        0        0     1077 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/app.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/cache/
+-rw-rw-rw-   0        0        0    10456 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/cache/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/dateutil/
+-rw-rw-rw-   0        0        0     2773 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/easter.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/dateutil/parser/
+-rw-rw-rw-   0        0        0    13517 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/parser/isoparser.py
+-rw-rw-rw-   0        0        0    59262 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/parser/_parser.py
+-rw-rw-rw-   0        0        0     1787 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/parser/__init__.py
+-rw-rw-rw-   0        0        0    25502 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/relativedelta.py
+-rw-rw-rw-   0        0        0    68282 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/rrule.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/dateutil/tz/
+-rw-rw-rw-   0        0        0    64282 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/tz/tz.py
+-rw-rw-rw-   0        0        0    13305 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/tz/win.py
+-rw-rw-rw-   0        0        0    13394 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/tz/_common.py
+-rw-rw-rw-   0        0        0     2374 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/tz/_factories.py
+-rw-rw-rw-   0        0        0      568 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/tz/__init__.py
+-rw-rw-rw-   0        0        0       61 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/tzwin.py
+-rw-rw-rw-   0        0        0     2034 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/dateutil/zoneinfo/
+-rw-rw-rw-   0        0        0     1772 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/zoneinfo/rebuild.py
+-rw-rw-rw-   0        0        0     6056 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/zoneinfo/__init__.py
+-rw-rw-rw-   0        0        0      975 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/_common.py
+-rw-rw-rw-   0        0        0      120 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/_version.py
+-rw-rw-rw-   0        0        0      230 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/dateutil/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/db/
+-rw-rw-rw-   0        0        0     6576 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/model.py
+-rw-rw-rw-   0        0        0    12043 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/mongodb.py
+-rw-rw-rw-   0        0        0    59544 2023-10-08 13:11:36.000000 kcweb-5.27/kcweb/utill/db/mysql.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/db/pymysql/
+-rw-rw-rw-   0        0        0    10542 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/charset.py
+-rw-rw-rw-   0        0        0    50320 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/connections.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/
+-rw-rw-rw-   0        0        0      884 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/CLIENT.py
+-rw-rw-rw-   0        0        0      713 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/COMMAND.py
+-rw-rw-rw-   0        0        0     2296 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/CR.py
+-rw-rw-rw-   0        0        0    12772 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/ER.py
+-rw-rw-rw-   0        0        0      405 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/FIELD_TYPE.py
+-rw-rw-rw-   0        0        0      229 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/FLAG.py
+-rw-rw-rw-   0        0        0      345 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/SERVER_STATUS.py
+-rw-rw-rw-   0        0        0        0 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/constants/__init__.py
+-rw-rw-rw-   0        0        0    12646 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/converters.py
+-rw-rw-rw-   0        0        0    17774 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/cursors.py
+-rw-rw-rw-   0        0        0     3825 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/err.py
+-rw-rw-rw-   0        0        0      681 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/optionfile.py
+-rw-rw-rw-   0        0        0    12365 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/protocol.py
+-rw-rw-rw-   0        0        0      380 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/times.py
+-rw-rw-rw-   0        0        0      193 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/util.py
+-rw-rw-rw-   0        0        0     7985 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/_auth.py
+-rw-rw-rw-   0        0        0      502 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/_compat.py
+-rw-rw-rw-   0        0        0     4183 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/_socketio.py
+-rw-rw-rw-   0        0        0     4873 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/pymysql/__init__.py
+-rw-rw-rw-   0        0        0    23069 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/sqlite copy.py
+-rw-rw-rw-   0        0        0    21956 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/db/sqlite.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/filetype/
+-rw-rw-rw-   0        0        0     2220 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/filetype.py
+-rw-rw-rw-   0        0        0     2643 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/helpers.py
+-rw-rw-rw-   0        0        0     2568 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/match.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/filetype/types/
+-rw-rw-rw-   0        0        0    13116 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/archive.py
+-rw-rw-rw-   0        0        0     3998 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/audio.py
+-rw-rw-rw-   0        0        0      706 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/base.py
+-rw-rw-rw-   0        0        0     2411 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/font.py
+-rw-rw-rw-   0        0        0     6616 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/image.py
+-rw-rw-rw-   0        0        0      961 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/isobmff.py
+-rw-rw-rw-   0        0        0     5570 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/video.py
+-rw-rw-rw-   0        0        0     1531 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/types/__init__.py
+-rw-rw-rw-   0        0        0     1742 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/utils.py
+-rw-rw-rw-   0        0        0      233 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/filetype/__init__.py
+-rw-rw-rw-   0        0        0     3752 2023-01-10 15:00:12.000000 kcweb-5.27/kcweb/utill/http.py
+-rw-rw-rw-   0        0        0    12030 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/queues.py
+-rw-rw-rw-   0        0        0     8146 2023-12-11 09:13:59.000000 kcweb-5.27/kcweb/utill/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb/utill/rediss/
+-rw-rw-rw-   0        0        0   150458 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/client.py
+-rw-rw-rw-   0        0        0    48878 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/connection.py
+-rw-rw-rw-   0        0        0     1057 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/exceptions.py
+-rw-rw-rw-   0        0        0    11109 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/lock.py
+-rw-rw-rw-   0        0        0    11644 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/sentinel.py
+-rw-rw-rw-   0        0        0      699 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/utils.py
+-rw-rw-rw-   0        0        0     4150 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/_compat.py
+-rw-rw-rw-   0        0        0     1033 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/utill/rediss/__init__.py
+-rw-rw-rw-   0        0        0       45 2022-05-13 07:34:10.000000 kcweb-5.27/kcweb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:13:52.000000 kcweb-5.27/kcweb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-08 15:13:52.000000 kcweb-5.27/kcweb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      579 2024-04-08 15:13:52.000000 kcweb-5.27/kcweb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2024-04-08 15:13:52.000000 kcweb-5.27/kcweb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     5346 2024-04-08 15:13:53.000000 kcweb-5.27/kcweb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      339 2024-04-08 15:13:52.000000 kcweb-5.27/kcweb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2024-01-15 09:20:34.000000 kcweb-5.27/LICENSE
+-rw-rw-rw-   0        0        0      579 2024-04-08 15:13:53.000000 kcweb-5.27/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2024-01-16 14:15:14.000000 kcweb-5.27/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:13:53.000000 kcweb-5.27/setup.cfg
+-rw-rw-rw-   0        0        0     2800 2024-04-08 14:56:13.000000 kcweb-5.27/setup.py
```

### Comparing `kcweb-5.26/kcweb/app.py` & `kcweb-5.27/kcweb/app.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/common/autoload.py` & `kcweb-5.27/kcweb/common/autoload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1268,15 +1268,15 @@
                 servertext=('#生产环境运行文件，请务修改\n'+
                         'from kcweb import web\n'+
                         'import '+self.appname+' as application\n'+
                         'app=web(__name__,application)\n'+
                         '# 以下代码兼容老版本框架\n'+
                         'if __name__ == "__main__":\n'+
                         '   #host监听ip port端口 name python解释器名字 (windows一般是python  linux一般是python3)\n'+
-                        '   app.run(host="0.0.0.0",port="30000",name="python")\n'
+                        '   app.run(host="0.0.0.0",port="30000",name="python3")\n'
                         )
                 f=open("./"+self.project+"server.py","w+",encoding='utf-8')
                 f.write(servertext)
                 f.close()
             # f=open(self.project+self.appname+"/common/autoload.py","w",encoding='utf-8')
             # f.write("from kcweb.common import *\n"+
             #         "from "+self.appname+" import config\n"+
```

### Comparing `kcweb-5.26/kcweb/common/request.py` & `kcweb-5.27/kcweb/common/request.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/common/session.py` & `kcweb-5.27/kcweb/common/session.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/config/__init__.py` & `kcweb-5.27/kcweb/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 email['pwd']='' #发件人邮箱密码(如申请的smtp给的口令)
 email['sendNick']='' #发件人昵称
 email['theme']='' #默认主题
 email['recNick']='' #默认收件人昵称
 
 kcweb={}
 kcweb['name']='kcweb'                             #项目的名称
-kcweb['version']='5.26'							#项目版本
+kcweb['version']='5.27'							#项目版本
 kcweb['description']='python web框架'       #项目的简单描述
 kcweb['long_description']='kcweb作为web开发而设计的高性能框架，采用全新的架构思想，注重易用性。遵循MIT开源许可协议发布，意味着个人和企业可以免费使用kcweb，甚至允许把你基于kcweb开发的应用开源或商业产品发布或销售'     #项目详细描述
 kcweb['license']='MIT'                    #开源协议   mit开源
 kcweb['url']=''
 kcweb['author']='百里-坤坤'  					 #名字
 kcweb['author_email']='fk1402936534@qq.com' 	     #邮件地址
 kcweb['maintainer']='坤坤' 						 #维护人员的名字
```

### Comparing `kcweb-5.26/kcweb/Events.py` & `kcweb-5.27/kcweb/Events.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/kcweb.py` & `kcweb-5.27/kcweb/kcweb.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/tpl/err.html` & `kcweb-5.27/kcweb/tpl/err.html`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/tpl/error.html` & `kcweb-5.27/kcweb/tpl/error.html`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/app.py` & `kcweb-5.27/kcweb/utill/app.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/cache/cache.py` & `kcweb-5.27/kcweb/utill/cache/cache.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/easter.py` & `kcweb-5.27/kcweb/utill/dateutil/easter.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/parser/isoparser.py` & `kcweb-5.27/kcweb/utill/dateutil/parser/isoparser.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/parser/_parser.py` & `kcweb-5.27/kcweb/utill/dateutil/parser/_parser.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/parser/__init__.py` & `kcweb-5.27/kcweb/utill/dateutil/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/relativedelta.py` & `kcweb-5.27/kcweb/utill/dateutil/relativedelta.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/rrule.py` & `kcweb-5.27/kcweb/utill/dateutil/rrule.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/tz/tz.py` & `kcweb-5.27/kcweb/utill/dateutil/tz/tz.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/tz/win.py` & `kcweb-5.27/kcweb/utill/dateutil/tz/win.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/tz/_common.py` & `kcweb-5.27/kcweb/utill/dateutil/tz/_common.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/tz/_factories.py` & `kcweb-5.27/kcweb/utill/dateutil/tz/_factories.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/tz/__init__.py` & `kcweb-5.27/kcweb/utill/dateutil/tz/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/utils.py` & `kcweb-5.27/kcweb/utill/dateutil/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/zoneinfo/rebuild.py` & `kcweb-5.27/kcweb/utill/dateutil/zoneinfo/rebuild.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/zoneinfo/__init__.py` & `kcweb-5.27/kcweb/utill/dateutil/zoneinfo/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/dateutil/_common.py` & `kcweb-5.27/kcweb/utill/dateutil/_common.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/model.py` & `kcweb-5.27/kcweb/utill/db/model.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/mongodb.py` & `kcweb-5.27/kcweb/utill/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/mysql.py` & `kcweb-5.27/kcweb/utill/db/mysql.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/charset.py` & `kcweb-5.27/kcweb/utill/db/pymysql/charset.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/connections.py` & `kcweb-5.27/kcweb/utill/db/pymysql/connections.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/constants/CLIENT.py` & `kcweb-5.27/kcweb/utill/db/pymysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/constants/COMMAND.py` & `kcweb-5.27/kcweb/utill/db/pymysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/constants/CR.py` & `kcweb-5.27/kcweb/utill/db/pymysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/constants/ER.py` & `kcweb-5.27/kcweb/utill/db/pymysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/converters.py` & `kcweb-5.27/kcweb/utill/db/pymysql/converters.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/cursors.py` & `kcweb-5.27/kcweb/utill/db/pymysql/cursors.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/err.py` & `kcweb-5.27/kcweb/utill/db/pymysql/err.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/optionfile.py` & `kcweb-5.27/kcweb/utill/db/pymysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/protocol.py` & `kcweb-5.27/kcweb/utill/db/pymysql/protocol.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/_auth.py` & `kcweb-5.27/kcweb/utill/db/pymysql/_auth.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/_socketio.py` & `kcweb-5.27/kcweb/utill/db/pymysql/_socketio.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/pymysql/__init__.py` & `kcweb-5.27/kcweb/utill/db/pymysql/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/sqlite copy.py` & `kcweb-5.27/kcweb/utill/db/sqlite copy.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/db/sqlite.py` & `kcweb-5.27/kcweb/utill/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/filetype.py` & `kcweb-5.27/kcweb/utill/filetype/filetype.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/helpers.py` & `kcweb-5.27/kcweb/utill/filetype/helpers.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/match.py` & `kcweb-5.27/kcweb/utill/filetype/match.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/archive.py` & `kcweb-5.27/kcweb/utill/filetype/types/archive.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/audio.py` & `kcweb-5.27/kcweb/utill/filetype/types/audio.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/base.py` & `kcweb-5.27/kcweb/utill/filetype/types/base.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/font.py` & `kcweb-5.27/kcweb/utill/filetype/types/font.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/image.py` & `kcweb-5.27/kcweb/utill/filetype/types/image.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/isobmff.py` & `kcweb-5.27/kcweb/utill/filetype/types/isobmff.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/video.py` & `kcweb-5.27/kcweb/utill/filetype/types/video.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/types/__init__.py` & `kcweb-5.27/kcweb/utill/filetype/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/filetype/utils.py` & `kcweb-5.27/kcweb/utill/filetype/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/http.py` & `kcweb-5.27/kcweb/utill/http.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/queues.py` & `kcweb-5.27/kcweb/utill/queues.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/redis.py` & `kcweb-5.27/kcweb/utill/redis.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/client.py` & `kcweb-5.27/kcweb/utill/rediss/client.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/connection.py` & `kcweb-5.27/kcweb/utill/rediss/connection.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/exceptions.py` & `kcweb-5.27/kcweb/utill/rediss/exceptions.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/lock.py` & `kcweb-5.27/kcweb/utill/rediss/lock.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/sentinel.py` & `kcweb-5.27/kcweb/utill/rediss/sentinel.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/utils.py` & `kcweb-5.27/kcweb/utill/rediss/utils.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/_compat.py` & `kcweb-5.27/kcweb/utill/rediss/_compat.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb/utill/rediss/__init__.py` & `kcweb-5.27/kcweb/utill/rediss/__init__.py`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/kcweb.egg-info/PKG-INFO` & `kcweb-5.27/kcweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kcweb
-Version: 5.26
+Version: 5.27
 Summary: kcweb作为web开发而设计的高性能框架，采用全新的架构思想，注重易用性。遵循MIT开源许可协议发布，意味着个人和企业可以免费使用kcweb，甚至允许把你基于kcweb开发的应用开源或商业产品发布或销售
 Home-page: UNKNOWN
 Author: 禄可集团-坤坤
 Author-email: fk1402936534@qq.com
 Maintainer: 坤坤
 Maintainer-email: fk1402936534@qq.com
 License: MIT License
-Keywords: kcweb5.26
+Keywords: kcweb5.27
 Platform: UNKNOWN
 License-File: LICENSE
 
 增加 kcweb 命令
```

### Comparing `kcweb-5.26/kcweb.egg-info/SOURCES.txt` & `kcweb-5.27/kcweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/LICENSE` & `kcweb-5.27/LICENSE`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/PKG-INFO` & `kcweb-5.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: kcweb
-Version: 5.26
+Version: 5.27
 Summary: kcweb作为web开发而设计的高性能框架，采用全新的架构思想，注重易用性。遵循MIT开源许可协议发布，意味着个人和企业可以免费使用kcweb，甚至允许把你基于kcweb开发的应用开源或商业产品发布或销售
 Home-page: UNKNOWN
 Author: 禄可集团-坤坤
 Author-email: fk1402936534@qq.com
 Maintainer: 坤坤
 Maintainer-email: fk1402936534@qq.com
 License: MIT License
-Keywords: kcweb5.26
+Keywords: kcweb5.27
 Platform: UNKNOWN
 License-File: LICENSE
 
 增加 kcweb 命令
```

### Comparing `kcweb-5.26/README.md` & `kcweb-5.27/README.md`

 * *Files identical despite different names*

### Comparing `kcweb-5.26/setup.py` & `kcweb-5.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
 00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
 00000260: 6527 5d3d 276b 6377 6562 2720 2020 2020  e']='kcweb'     
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 23e9 a1b9 e79b aee7          #.......
 00000290: 9a84 e590 8de7 a7b0 200d 0a63 6f6e 666b  ........ ..confk
 000002a0: 6377 5b27 7665 7273 696f 6e27 5d3d 2735  cw['version']='5
-000002b0: 2e32 3627 0909 0909 0909 0923 e9a1 b9e7  .26'.......#....
+000002b0: 2e32 3727 0909 0909 0909 0923 e9a1 b9e7  .27'.......#....
 000002c0: 9bae e789 88e6 9cac 0d0a 636f 6e66 6b63  ..........confkc
 000002d0: 775b 2764 6573 6372 6970 7469 6f6e 275d  w['description']
 000002e0: 3d27 6b63 7765 62e4 bd9c e4b8 ba77 6562  ='kcweb......web
 000002f0: e5bc 80e5 8f91 e880 8ce8 aebe e8ae a1e7  ................
 00000300: 9a84 e9ab 98e6 80a7 e883 bde6 a186 e69e  ................
 00000310: b6ef bc8c e987 87e7 94a8 e585 a8e6 96b0  ................
 00000320: e79a 84e6 9eb6 e69e 84e6 809d e683 b3ef  ................
@@ -153,22 +153,23 @@
 00000980: 5b27 6775 6e69 636f 726e 3d3d 3230 2e30  ['gunicorn==20.0
 00000990: 2e34 272c 2770 796d 6f6e 676f 3e3d 332e  .4','pymongo>=3.
 000009a0: 3130 2e30 272c 274d 616b 6f3e 3d31 2e31  10.0','Mako>=1.1
 000009b0: 2e32 272c 2772 6571 7565 7374 733e 3d32  .2','requests>=2
 000009c0: 2e32 332e 3027 2c27 7369 783e 3d31 2e31  .23.0','six>=1.1
 000009d0: 322e 3027 2c27 7761 7463 6864 6f67 3e3d  2.0','watchdog>=
 000009e0: 302e 392e 3027 2c27 7765 6273 6f63 6b65  0.9.0','websocke
-000009f0: 7473 3d3d 382e 3127 5d2c 2023 e7ac ace4  ts==8.1'], #....
-00000a00: b889 e696 b9e5 8c85 0d0a 2020 2020 7061  ..........    pa
-00000a10: 636b 6167 655f 6461 7461 203d 207b 0d0a  ckage_data = {..
-00000a20: 2020 2020 2020 2020 2727 3a20 5b27 2a2e          '': ['*.
-00000a30: 6874 6d6c 272c 2027 2a2e 6a73 272c 272a  html', '*.js','*
-00000a40: 2e63 7373 272c 272a 2e6a 7067 272c 272a  .css','*.jpg','*
-00000a50: 2e70 6e67 272c 272a 2e67 6966 275d 2c0d  .png','*.gif'],.
-00000a60: 0a20 2020 207d 2c0d 0a20 2020 2065 6e74  .    },..    ent
-00000a70: 7279 5f70 6f69 6e74 7320 3d20 7b0d 0a20  ry_points = {.. 
-00000a80: 2020 2020 2020 2027 636f 6e73 6f6c 655f         'console_
-00000a90: 7363 7269 7074 7327 3a5b 0d0a 2020 2020  scripts':[..    
-00000aa0: 2020 2020 2020 2020 276b 6377 6562 203d          'kcweb =
-00000ab0: 206b 6377 6562 2e6b 6377 6562 3a65 7865   kcweb.kcweb:exe
-00000ac0: 6375 7461 626c 6527 0d0a 2020 2020 2020  cutable'..      
-00000ad0: 2020 5d0d 0a20 2020 207d 0d0a 29           ]..    }..)
+000009f0: 7473 3d3d 382e 3127 2c27 7572 6c6c 6962  ts==8.1','urllib
+00000a00: 333d 3d31 2e32 352e 3131 275d 2c20 23e7  3==1.25.11'], #.
+00000a10: acac e4b8 89e6 96b9 e58c 850d 0a20 2020  .............   
+00000a20: 2070 6163 6b61 6765 5f64 6174 6120 3d20   package_data = 
+00000a30: 7b0d 0a20 2020 2020 2020 2027 273a 205b  {..        '': [
+00000a40: 272a 2e68 746d 6c27 2c20 272a 2e6a 7327  '*.html', '*.js'
+00000a50: 2c27 2a2e 6373 7327 2c27 2a2e 6a70 6727  ,'*.css','*.jpg'
+00000a60: 2c27 2a2e 706e 6727 2c27 2a2e 6769 6627  ,'*.png','*.gif'
+00000a70: 5d2c 0d0a 2020 2020 7d2c 0d0a 2020 2020  ],..    },..    
+00000a80: 656e 7472 795f 706f 696e 7473 203d 207b  entry_points = {
+00000a90: 0d0a 2020 2020 2020 2020 2763 6f6e 736f  ..        'conso
+00000aa0: 6c65 5f73 6372 6970 7473 273a 5b0d 0a20  le_scripts':[.. 
+00000ab0: 2020 2020 2020 2020 2020 2027 6b63 7765             'kcwe
+00000ac0: 6220 3d20 6b63 7765 622e 6b63 7765 623a  b = kcweb.kcweb:
+00000ad0: 6578 6563 7574 6162 6c65 270d 0a20 2020  executable'..   
+00000ae0: 2020 2020 205d 0d0a 2020 2020 7d0d 0a29       ]..    }..)
```

