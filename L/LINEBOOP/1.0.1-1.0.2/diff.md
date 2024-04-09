# Comparing `tmp/LINEBOOP-1.0.1.tar.gz` & `tmp/LINEBOOP-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LINEBOOP-1.0.1.tar", last modified: Sun Feb 11 09:09:00 2024, max compression
+gzip compressed data, was "LINEBOOP-1.0.2.tar", last modified: Tue Apr  9 11:33:19 2024, max compression
```

## Comparing `LINEBOOP-1.0.1.tar` & `LINEBOOP-1.0.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.896303 LINEBOOP-1.0.1/
--rw-rw-rw-   0        0        0     1545 2024-02-10 18:24:20.000000 LINEBOOP-1.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.836608 LINEBOOP-1.0.1/LINEBOOP/
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.842592 LINEBOOP-1.0.1/LINEBOOP/BIZ/
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.843845 LINEBOOP-1.0.1/LINEBOOP/BIZ/TL/
--rw-rw-rw-   0        0        0     6497 2024-02-10 18:09:22.000000 LINEBOOP-1.0.1/LINEBOOP/BIZ/TL/ST.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.1/LINEBOOP/BIZ/TL/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.1/LINEBOOP/BIZ/__init__.py
--rw-rw-rw-   0        0        0      251 2024-02-11 09:05:35.000000 LINEBOOP-1.0.1/LINEBOOP/__init__.py
--rw-rw-rw-   0        0        0    26562 2024-02-10 18:09:50.000000 LINEBOOP-1.0.1/LINEBOOP/api.py
--rw-rw-rw-   0        0        0     5833 2024-02-11 09:02:59.000000 LINEBOOP-1.0.1/LINEBOOP/client.py
--rw-rw-rw-   0        0        0     9322 2024-02-10 18:09:50.000000 LINEBOOP-1.0.1/LINEBOOP/config.py
--rw-rw-rw-   0        0        0     1842 2024-02-10 18:10:19.000000 LINEBOOP-1.0.1/LINEBOOP/cube.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.845841 LINEBOOP-1.0.1/LINEBOOP/dyher/
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.1/LINEBOOP/dyher/__init__.py
--rw-rw-rw-   0        0        0     7763 2024-02-10 18:09:21.000000 LINEBOOP-1.0.1/LINEBOOP/dyher/conn.py
--rw-rw-rw-   0        0        0    15544 2024-02-11 09:01:28.000000 LINEBOOP-1.0.1/LINEBOOP/dyher/connManager.py
--rw-rw-rw-   0        0        0    17273 2024-02-10 18:10:19.000000 LINEBOOP-1.0.1/LINEBOOP/e2ee.py
--rw-rw-rw-   0        0        0      982 2024-02-10 18:10:20.000000 LINEBOOP-1.0.1/LINEBOOP/exceptions.py
--rw-rw-rw-   0        0        0    15273 2024-02-10 18:10:19.000000 LINEBOOP-1.0.1/LINEBOOP/helpers.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.849830 LINEBOOP-1.0.1/LINEBOOP/hksc/
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.1/LINEBOOP/hksc/__init__.py
--rw-rw-rw-   0        0        0     3439 2024-02-10 18:09:19.000000 LINEBOOP-1.0.1/LINEBOOP/hksc/database.py
--rw-rw-rw-   0        0        0      335 2024-02-10 18:09:19.000000 LINEBOOP-1.0.1/LINEBOOP/hksc/events.py
--rw-rw-rw-   0        0        0     6220 2024-02-10 18:09:17.000000 LINEBOOP-1.0.1/LINEBOOP/hksc/types.py
--rw-rw-rw-   0        0        0     2494 2024-02-10 18:09:17.000000 LINEBOOP-1.0.1/LINEBOOP/hksc/utility.py
--rw-rw-rw-   0        0        0     4110 2024-02-10 18:10:41.000000 LINEBOOP-1.0.1/LINEBOOP/hooks.py
--rw-rw-rw-   0        0        0    39147 2024-02-10 18:09:50.000000 LINEBOOP-1.0.1/LINEBOOP/models.py
--rw-rw-rw-   0        0        0    29795 2024-02-10 18:10:18.000000 LINEBOOP-1.0.1/LINEBOOP/object.py
--rw-rw-rw-   0        0        0     2426 2024-02-10 18:10:18.000000 LINEBOOP-1.0.1/LINEBOOP/poll.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.850826 LINEBOOP-1.0.1/LINEBOOP/serializers/
--rw-rw-rw-   0        0        0     2300 2024-02-10 18:09:15.000000 LINEBOOP-1.0.1/LINEBOOP/serializers/DummyProtocol.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.1/LINEBOOP/serializers/__init__.py
--rw-rw-rw-   0        0        0     2760 2024-02-10 18:10:20.000000 LINEBOOP-1.0.1/LINEBOOP/server.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.875757 LINEBOOP-1.0.1/LINEBOOP/services/
--rw-rw-rw-   0        0        0      933 2024-02-10 18:09:56.000000 LINEBOOP-1.0.1/LINEBOOP/services/AccessTokenRefreshService.py
--rw-rw-rw-   0        0        0     2425 2024-02-10 18:10:01.000000 LINEBOOP-1.0.1/LINEBOOP/services/AccountAuthFactorEapConnectService.py
--rw-rw-rw-   0        0        0    13334 2024-02-10 18:09:55.000000 LINEBOOP-1.0.1/LINEBOOP/services/AuthService.py
--rw-rw-rw-   0        0        0      467 2024-02-11 09:03:35.000000 LINEBOOP-1.0.1/LINEBOOP/services/BaseService.py
--rw-rw-rw-   0        0        0     1285 2024-02-10 18:10:19.000000 LINEBOOP-1.0.1/LINEBOOP/services/BotExternalService.py
--rw-rw-rw-   0        0        0    11397 2024-02-10 18:09:54.000000 LINEBOOP-1.0.1/LINEBOOP/services/BuddyService.py
--rw-rw-rw-   0        0        0    11695 2024-02-10 18:09:57.000000 LINEBOOP-1.0.1/LINEBOOP/services/CallService.py
--rw-rw-rw-   0        0        0    13827 2024-02-10 18:09:53.000000 LINEBOOP-1.0.1/LINEBOOP/services/ChannelService.py
--rw-rw-rw-   0        0        0      975 2024-02-10 18:10:01.000000 LINEBOOP-1.0.1/LINEBOOP/services/ChatAppService.py
--rw-rw-rw-   0        0        0     1509 2024-02-10 18:10:01.000000 LINEBOOP-1.0.1/LINEBOOP/services/E2EEKeyBackupService.py
--rw-rw-rw-   0        0        0     2037 2024-02-10 18:10:02.000000 LINEBOOP-1.0.1/LINEBOOP/services/HomeSafetyCheckService.py
--rw-rw-rw-   0        0        0     1946 2024-02-10 18:10:16.000000 LINEBOOP-1.0.1/LINEBOOP/services/InterlockService.py
--rw-rw-rw-   0        0        0     2651 2024-02-10 18:09:53.000000 LINEBOOP-1.0.1/LINEBOOP/services/LiffService.py
--rw-rw-rw-   0        0        0     2570 2024-02-11 09:01:42.000000 LINEBOOP-1.0.1/LINEBOOP/services/LoginService.py
--rw-rw-rw-   0        0        0     2513 2024-02-10 18:10:18.000000 LINEBOOP-1.0.1/LINEBOOP/services/OaMembershipService.py
--rw-rw-rw-   0        0        0     9898 2024-02-10 18:09:54.000000 LINEBOOP-1.0.1/LINEBOOP/services/PrimaryAccountInitService.py
--rw-rw-rw-   0        0        0      899 2024-02-10 18:10:02.000000 LINEBOOP-1.0.1/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py
--rw-rw-rw-   0        0        0     1132 2024-02-10 18:10:02.000000 LINEBOOP-1.0.1/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py
--rw-rw-rw-   0        0        0     1400 2024-02-10 18:10:18.000000 LINEBOOP-1.0.1/LINEBOOP/services/PwlessPrimaryRegistrationService.py
--rw-rw-rw-   0        0        0     5773 2024-02-10 18:10:17.000000 LINEBOOP-1.0.1/LINEBOOP/services/RelationService.py
--rw-rw-rw-   0        0        0     6045 2024-02-10 18:10:18.000000 LINEBOOP-1.0.1/LINEBOOP/services/SearchService.py
--rw-rw-rw-   0        0        0      937 2024-02-10 18:10:00.000000 LINEBOOP-1.0.1/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py
--rw-rw-rw-   0        0        0     3207 2024-02-10 18:10:00.000000 LINEBOOP-1.0.1/LINEBOOP/services/SecondaryPwlessLoginService.py
--rw-rw-rw-   0        0        0     3908 2024-02-10 18:09:55.000000 LINEBOOP-1.0.1/LINEBOOP/services/SettingsService.py
--rw-rw-rw-   0        0        0      311 2024-02-10 18:10:17.000000 LINEBOOP-1.0.1/LINEBOOP/services/ShopAuthService.py
--rw-rw-rw-   0        0        0    57050 2024-02-10 18:09:51.000000 LINEBOOP-1.0.1/LINEBOOP/services/ShopService.py
--rw-rw-rw-   0        0        0      413 2024-02-10 18:10:01.000000 LINEBOOP-1.0.1/LINEBOOP/services/SquareBotService.py
--rw-rw-rw-   0        0        0    12199 2024-02-11 09:01:34.000000 LINEBOOP-1.0.1/LINEBOOP/services/SquareLiveTalkService.py
--rw-rw-rw-   0        0        0    45459 2024-02-11 09:02:15.000000 LINEBOOP-1.0.1/LINEBOOP/services/SquareService.py
--rw-rw-rw-   0        0        0   226578 2024-02-10 18:09:50.000000 LINEBOOP-1.0.1/LINEBOOP/services/TalkService.py
--rw-rw-rw-   0        0        0      732 2024-02-10 18:10:02.000000 LINEBOOP-1.0.1/LINEBOOP/services/TestService.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:22.000000 LINEBOOP-1.0.1/LINEBOOP/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.886727 LINEBOOP-1.0.1/LINEBOOP/services/thrift/
--rw-rw-rw-   0        0        0     8674 2024-02-10 18:09:50.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/AccessTokenRefreshService.py
--rw-rw-rw-   0        0        0     8916 2024-02-10 18:09:50.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/BuddyService.py
--rw-rw-rw-   0        0        0     8811 2024-02-10 18:09:49.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/CallService.py
--rw-rw-rw-   0        0        0     9240 2024-02-10 18:09:41.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/E2EEKeyBackupService.py
--rw-rw-rw-   0        0        0    19853 2024-02-10 18:09:40.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/HomeSafetyCheckService.py
--rw-rw-rw-   0        0        0    14578 2024-02-10 18:09:39.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py
--rw-rw-rw-   0        0        0   171508 2024-02-10 18:09:39.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/SquareLiveTalkService.py
--rw-rw-rw-   0        0        0   108217 2024-02-10 18:09:38.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/SquareService.py
--rw-rw-rw-   0        0        0     7671 2024-02-10 18:09:38.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/SyncService.py
--rw-rw-rw-   0        0        0   546935 2024-02-10 18:09:37.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/TalkService.py
--rw-rw-rw-   0        0        0      248 2024-02-10 18:09:37.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.893216 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/
--rw-rw-rw-   0        0        0     2909 2024-02-10 18:09:24.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TBase.py
--rw-rw-rw-   0        0        0     9403 2024-02-10 18:09:24.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TBinaryProtocol.py
--rw-rw-rw-   0        0        0    15223 2024-02-10 18:09:24.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TCompactProtocol.py
--rw-rw-rw-   0        0        0    13780 2024-02-10 18:09:23.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TProtocol.py
--rw-rw-rw-   0        0        0     1781 2024-02-10 18:09:23.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TProtocolDecorator.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:23.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/__init__.py
--rw-rw-rw-   0        0        0      419 2024-02-10 18:09:25.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/compat.py
--rw-rw-rw-   0        0        0      380 2024-02-10 18:09:41.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/constants.py
--rw-rw-rw-   0        0        0  1144513 2024-02-10 18:09:37.000000 LINEBOOP-1.0.1/LINEBOOP/services/thrift/ttypes.py
--rw-rw-rw-   0        0        0    39544 2024-02-10 18:10:17.000000 LINEBOOP-1.0.1/LINEBOOP/thrift.py
--rw-rw-rw-   0        0        0    68112 2024-02-10 18:10:18.000000 LINEBOOP-1.0.1/LINEBOOP/timeline.py
--rw-rw-rw-   0        0        0     3531 2024-02-10 18:10:19.000000 LINEBOOP-1.0.1/LINEBOOP/timelineBiz.py
-drwxrwxrwx   0        0        0        0 2024-02-11 09:09:00.894306 LINEBOOP-1.0.1/LINEBOOP.egg-info/
--rw-rw-rw-   0        0        0      713 2024-02-11 09:09:00.000000 LINEBOOP-1.0.1/LINEBOOP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3023 2024-02-11 09:09:00.000000 LINEBOOP-1.0.1/LINEBOOP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-11 09:09:00.000000 LINEBOOP-1.0.1/LINEBOOP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-02-11 09:09:00.000000 LINEBOOP-1.0.1/LINEBOOP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-11 09:09:00.000000 LINEBOOP-1.0.1/LINEBOOP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2024-02-11 09:09:00.895305 LINEBOOP-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      114 2024-02-10 18:16:30.000000 LINEBOOP-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-02-11 09:09:00.896303 LINEBOOP-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2024-02-10 18:15:11.000000 LINEBOOP-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.562736 LINEBOOP-1.0.2/
+-rw-rw-rw-   0        0        0     1545 2024-02-10 18:24:20.000000 LINEBOOP-1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.490692 LINEBOOP-1.0.2/LINEBOOP/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.504166 LINEBOOP-1.0.2/LINEBOOP/BIZ/
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.505163 LINEBOOP-1.0.2/LINEBOOP/BIZ/TL/
+-rw-rw-rw-   0        0        0     6497 2024-02-10 18:09:22.000000 LINEBOOP-1.0.2/LINEBOOP/BIZ/TL/ST.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.2/LINEBOOP/BIZ/TL/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.2/LINEBOOP/BIZ/__init__.py
+-rw-rw-rw-   0        0        0      251 2024-04-09 11:32:02.000000 LINEBOOP-1.0.2/LINEBOOP/__init__.py
+-rw-rw-rw-   0        0        0    26562 2024-02-10 18:09:50.000000 LINEBOOP-1.0.2/LINEBOOP/api.py
+-rw-rw-rw-   0        0        0     5833 2024-02-11 09:02:59.000000 LINEBOOP-1.0.2/LINEBOOP/client.py
+-rw-rw-rw-   0        0        0     9317 2024-04-09 11:22:18.000000 LINEBOOP-1.0.2/LINEBOOP/config.py
+-rw-rw-rw-   0        0        0     1842 2024-02-10 18:10:19.000000 LINEBOOP-1.0.2/LINEBOOP/cube.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.507668 LINEBOOP-1.0.2/LINEBOOP/dyher/
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.2/LINEBOOP/dyher/__init__.py
+-rw-rw-rw-   0        0        0     7763 2024-02-10 18:09:21.000000 LINEBOOP-1.0.2/LINEBOOP/dyher/conn.py
+-rw-rw-rw-   0        0        0    15544 2024-02-11 09:01:28.000000 LINEBOOP-1.0.2/LINEBOOP/dyher/connManager.py
+-rw-rw-rw-   0        0        0    17273 2024-02-10 18:10:19.000000 LINEBOOP-1.0.2/LINEBOOP/e2ee.py
+-rw-rw-rw-   0        0        0      982 2024-02-10 18:10:20.000000 LINEBOOP-1.0.2/LINEBOOP/exceptions.py
+-rw-rw-rw-   0        0        0    15273 2024-02-10 18:10:19.000000 LINEBOOP-1.0.2/LINEBOOP/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.511893 LINEBOOP-1.0.2/LINEBOOP/hksc/
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.2/LINEBOOP/hksc/__init__.py
+-rw-rw-rw-   0        0        0     3439 2024-02-10 18:09:19.000000 LINEBOOP-1.0.2/LINEBOOP/hksc/database.py
+-rw-rw-rw-   0        0        0      335 2024-02-10 18:09:19.000000 LINEBOOP-1.0.2/LINEBOOP/hksc/events.py
+-rw-rw-rw-   0        0        0     6220 2024-02-10 18:09:17.000000 LINEBOOP-1.0.2/LINEBOOP/hksc/types.py
+-rw-rw-rw-   0        0        0     2494 2024-02-10 18:09:17.000000 LINEBOOP-1.0.2/LINEBOOP/hksc/utility.py
+-rw-rw-rw-   0        0        0     4110 2024-02-10 18:10:41.000000 LINEBOOP-1.0.2/LINEBOOP/hooks.py
+-rw-rw-rw-   0        0        0    39147 2024-02-10 18:09:50.000000 LINEBOOP-1.0.2/LINEBOOP/models.py
+-rw-rw-rw-   0        0        0    29790 2024-04-09 11:22:18.000000 LINEBOOP-1.0.2/LINEBOOP/object.py
+-rw-rw-rw-   0        0        0     2426 2024-02-10 18:10:18.000000 LINEBOOP-1.0.2/LINEBOOP/poll.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.513888 LINEBOOP-1.0.2/LINEBOOP/serializers/
+-rw-rw-rw-   0        0        0     2300 2024-02-10 18:09:15.000000 LINEBOOP-1.0.2/LINEBOOP/serializers/DummyProtocol.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.2/LINEBOOP/serializers/__init__.py
+-rw-rw-rw-   0        0        0     2760 2024-02-10 18:10:20.000000 LINEBOOP-1.0.2/LINEBOOP/server.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.541469 LINEBOOP-1.0.2/LINEBOOP/services/
+-rw-rw-rw-   0        0        0      933 2024-02-10 18:09:56.000000 LINEBOOP-1.0.2/LINEBOOP/services/AccessTokenRefreshService.py
+-rw-rw-rw-   0        0        0     2425 2024-02-10 18:10:01.000000 LINEBOOP-1.0.2/LINEBOOP/services/AccountAuthFactorEapConnectService.py
+-rw-rw-rw-   0        0        0    13334 2024-02-10 18:09:55.000000 LINEBOOP-1.0.2/LINEBOOP/services/AuthService.py
+-rw-rw-rw-   0        0        0      467 2024-02-11 09:03:35.000000 LINEBOOP-1.0.2/LINEBOOP/services/BaseService.py
+-rw-rw-rw-   0        0        0     1285 2024-02-10 18:10:19.000000 LINEBOOP-1.0.2/LINEBOOP/services/BotExternalService.py
+-rw-rw-rw-   0        0        0    11397 2024-02-10 18:09:54.000000 LINEBOOP-1.0.2/LINEBOOP/services/BuddyService.py
+-rw-rw-rw-   0        0        0    11695 2024-02-10 18:09:57.000000 LINEBOOP-1.0.2/LINEBOOP/services/CallService.py
+-rw-rw-rw-   0        0        0    13827 2024-02-10 18:09:53.000000 LINEBOOP-1.0.2/LINEBOOP/services/ChannelService.py
+-rw-rw-rw-   0        0        0      975 2024-02-10 18:10:01.000000 LINEBOOP-1.0.2/LINEBOOP/services/ChatAppService.py
+-rw-rw-rw-   0        0        0     1509 2024-02-10 18:10:01.000000 LINEBOOP-1.0.2/LINEBOOP/services/E2EEKeyBackupService.py
+-rw-rw-rw-   0        0        0     2037 2024-02-10 18:10:02.000000 LINEBOOP-1.0.2/LINEBOOP/services/HomeSafetyCheckService.py
+-rw-rw-rw-   0        0        0     1946 2024-02-10 18:10:16.000000 LINEBOOP-1.0.2/LINEBOOP/services/InterlockService.py
+-rw-rw-rw-   0        0        0     2651 2024-02-10 18:09:53.000000 LINEBOOP-1.0.2/LINEBOOP/services/LiffService.py
+-rw-rw-rw-   0        0        0     2570 2024-02-11 09:01:42.000000 LINEBOOP-1.0.2/LINEBOOP/services/LoginService.py
+-rw-rw-rw-   0        0        0     2513 2024-02-10 18:10:18.000000 LINEBOOP-1.0.2/LINEBOOP/services/OaMembershipService.py
+-rw-rw-rw-   0        0        0     9898 2024-02-10 18:09:54.000000 LINEBOOP-1.0.2/LINEBOOP/services/PrimaryAccountInitService.py
+-rw-rw-rw-   0        0        0      899 2024-02-10 18:10:02.000000 LINEBOOP-1.0.2/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py
+-rw-rw-rw-   0        0        0     1132 2024-02-10 18:10:02.000000 LINEBOOP-1.0.2/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py
+-rw-rw-rw-   0        0        0     1400 2024-02-10 18:10:18.000000 LINEBOOP-1.0.2/LINEBOOP/services/PwlessPrimaryRegistrationService.py
+-rw-rw-rw-   0        0        0     5773 2024-02-10 18:10:17.000000 LINEBOOP-1.0.2/LINEBOOP/services/RelationService.py
+-rw-rw-rw-   0        0        0     6045 2024-02-10 18:10:18.000000 LINEBOOP-1.0.2/LINEBOOP/services/SearchService.py
+-rw-rw-rw-   0        0        0      937 2024-02-10 18:10:00.000000 LINEBOOP-1.0.2/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py
+-rw-rw-rw-   0        0        0     3207 2024-02-10 18:10:00.000000 LINEBOOP-1.0.2/LINEBOOP/services/SecondaryPwlessLoginService.py
+-rw-rw-rw-   0        0        0     3908 2024-02-10 18:09:55.000000 LINEBOOP-1.0.2/LINEBOOP/services/SettingsService.py
+-rw-rw-rw-   0        0        0      311 2024-02-10 18:10:17.000000 LINEBOOP-1.0.2/LINEBOOP/services/ShopAuthService.py
+-rw-rw-rw-   0        0        0    57050 2024-02-10 18:09:51.000000 LINEBOOP-1.0.2/LINEBOOP/services/ShopService.py
+-rw-rw-rw-   0        0        0      413 2024-02-10 18:10:01.000000 LINEBOOP-1.0.2/LINEBOOP/services/SquareBotService.py
+-rw-rw-rw-   0        0        0    12199 2024-02-11 09:01:34.000000 LINEBOOP-1.0.2/LINEBOOP/services/SquareLiveTalkService.py
+-rw-rw-rw-   0        0        0    45459 2024-02-11 09:02:15.000000 LINEBOOP-1.0.2/LINEBOOP/services/SquareService.py
+-rw-rw-rw-   0        0        0   226578 2024-02-10 18:09:50.000000 LINEBOOP-1.0.2/LINEBOOP/services/TalkService.py
+-rw-rw-rw-   0        0        0      732 2024-02-10 18:10:02.000000 LINEBOOP-1.0.2/LINEBOOP/services/TestService.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:22.000000 LINEBOOP-1.0.2/LINEBOOP/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.552951 LINEBOOP-1.0.2/LINEBOOP/services/thrift/
+-rw-rw-rw-   0        0        0     8674 2024-02-10 18:09:50.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/AccessTokenRefreshService.py
+-rw-rw-rw-   0        0        0     8916 2024-02-10 18:09:50.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/BuddyService.py
+-rw-rw-rw-   0        0        0     8811 2024-02-10 18:09:49.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/CallService.py
+-rw-rw-rw-   0        0        0     9240 2024-02-10 18:09:41.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/E2EEKeyBackupService.py
+-rw-rw-rw-   0        0        0    19853 2024-02-10 18:09:40.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/HomeSafetyCheckService.py
+-rw-rw-rw-   0        0        0    14578 2024-02-10 18:09:39.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py
+-rw-rw-rw-   0        0        0   171508 2024-02-10 18:09:39.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/SquareLiveTalkService.py
+-rw-rw-rw-   0        0        0   108217 2024-02-10 18:09:38.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/SquareService.py
+-rw-rw-rw-   0        0        0     7671 2024-02-10 18:09:38.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/SyncService.py
+-rw-rw-rw-   0        0        0   546935 2024-02-10 18:09:37.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/TalkService.py
+-rw-rw-rw-   0        0        0      248 2024-02-10 18:09:37.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.559744 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/
+-rw-rw-rw-   0        0        0     2909 2024-02-10 18:09:24.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TBase.py
+-rw-rw-rw-   0        0        0     9403 2024-02-10 18:09:24.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TBinaryProtocol.py
+-rw-rw-rw-   0        0        0    15223 2024-02-10 18:09:24.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TCompactProtocol.py
+-rw-rw-rw-   0        0        0    13780 2024-02-10 18:09:23.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TProtocol.py
+-rw-rw-rw-   0        0        0     1781 2024-02-10 18:09:23.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TProtocolDecorator.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:23.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/__init__.py
+-rw-rw-rw-   0        0        0      419 2024-02-10 18:09:25.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/compat.py
+-rw-rw-rw-   0        0        0      380 2024-02-10 18:09:41.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/constants.py
+-rw-rw-rw-   0        0        0  1144513 2024-02-10 18:09:37.000000 LINEBOOP-1.0.2/LINEBOOP/services/thrift/ttypes.py
+-rw-rw-rw-   0        0        0    39544 2024-02-10 18:10:17.000000 LINEBOOP-1.0.2/LINEBOOP/thrift.py
+-rw-rw-rw-   0        0        0    68112 2024-02-10 18:10:18.000000 LINEBOOP-1.0.2/LINEBOOP/timeline.py
+-rw-rw-rw-   0        0        0     3531 2024-02-10 18:10:19.000000 LINEBOOP-1.0.2/LINEBOOP/timelineBiz.py
+drwxrwxrwx   0        0        0        0 2024-04-09 11:33:19.560741 LINEBOOP-1.0.2/LINEBOOP.egg-info/
+-rw-rw-rw-   0        0        0      713 2024-04-09 11:33:19.000000 LINEBOOP-1.0.2/LINEBOOP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3023 2024-04-09 11:33:19.000000 LINEBOOP-1.0.2/LINEBOOP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 11:33:19.000000 LINEBOOP-1.0.2/LINEBOOP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-04-09 11:33:19.000000 LINEBOOP-1.0.2/LINEBOOP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 11:33:19.000000 LINEBOOP-1.0.2/LINEBOOP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      713 2024-04-09 11:33:19.561739 LINEBOOP-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2024-02-10 18:16:30.000000 LINEBOOP-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 11:33:19.562736 LINEBOOP-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      862 2024-02-10 18:15:11.000000 LINEBOOP-1.0.2/setup.py
```

### Comparing `LINEBOOP-1.0.1/LICENSE` & `LINEBOOP-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/BIZ/TL/ST.py` & `LINEBOOP-1.0.2/LINEBOOP/BIZ/TL/ST.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/api.py` & `LINEBOOP-1.0.2/LINEBOOP/api.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/client.py` & `LINEBOOP-1.0.2/LINEBOOP/client.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/config.py` & `LINEBOOP-1.0.2/LINEBOOP/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     LINE_LAN_ANDROID_URL = "https://lan.line.me/v1/line/android/notification"
     LINE_LAN_IOS_URL = "https://lan.line.me/v1/line/ios/notification"
     LINE_MUSIC_WEBAPP_URL = "https://music.line.me/webapp"
     LINE_AMP_LOG_URL = "https://log1-amp.line-apps.com/log"
     LINE_SECONDYARY_REGISTER_API_URL = "https://w.line.me/lrs/r"
 
-    LINE_LANGUAGE = "zh-Hant_TW"
+    LINE_LANGUAGE = "th_TH"
     LINE_SERVICE_REGION = "TW"
 
     APP_TYPE = "CHROMEOS"
     APP_VER = "11.19.2"
     SYSTEM_NAME = "DeachSword"
     SYSTEM_VER = "12.1.4"
     IP_ADDR = "8.8.8.8"
```

### Comparing `LINEBOOP-1.0.1/LINEBOOP/cube.py` & `LINEBOOP-1.0.2/LINEBOOP/cube.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/dyher/conn.py` & `LINEBOOP-1.0.2/LINEBOOP/dyher/conn.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/dyher/connManager.py` & `LINEBOOP-1.0.2/LINEBOOP/dyher/connManager.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/e2ee.py` & `LINEBOOP-1.0.2/LINEBOOP/e2ee.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/exceptions.py` & `LINEBOOP-1.0.2/LINEBOOP/exceptions.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/helpers.py` & `LINEBOOP-1.0.2/LINEBOOP/helpers.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/hksc/database.py` & `LINEBOOP-1.0.2/LINEBOOP/hksc/database.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/hksc/types.py` & `LINEBOOP-1.0.2/LINEBOOP/hksc/types.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/hksc/utility.py` & `LINEBOOP-1.0.2/LINEBOOP/hksc/utility.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/hooks.py` & `LINEBOOP-1.0.2/LINEBOOP/hooks.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/models.py` & `LINEBOOP-1.0.2/LINEBOOP/models.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/object.py` & `LINEBOOP-1.0.2/LINEBOOP/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,15 +450,15 @@
             "filters": {"OCR": {"params": {"useColorPicker": "true"}}},
         }
 
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
                 "x-client-channel": "chat_viewer",
-                "x-lal": "zh-Hant_TW",
+                "x-lal": "th_TH",
                 "x-recognition-input-type": "obs",
                 "Content-Type": "application/json",
             },
         )
         r = self.server.postContent(
             self.LINE_OBS_DOMAIN + "/px/talk/m/%s/recognition.obs" % msgId,
             data=json.dumps(data),
```

### Comparing `LINEBOOP-1.0.1/LINEBOOP/poll.py` & `LINEBOOP-1.0.2/LINEBOOP/poll.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/serializers/DummyProtocol.py` & `LINEBOOP-1.0.2/LINEBOOP/serializers/DummyProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/server.py` & `LINEBOOP-1.0.2/LINEBOOP/server.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/AccessTokenRefreshService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/AccessTokenRefreshService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/AccountAuthFactorEapConnectService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/AccountAuthFactorEapConnectService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/AuthService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/AuthService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/BotExternalService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/BotExternalService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/BuddyService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/BuddyService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/CallService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/CallService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/ChannelService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/ChannelService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/ChatAppService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/ChatAppService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/E2EEKeyBackupService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/E2EEKeyBackupService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/HomeSafetyCheckService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/HomeSafetyCheckService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/InterlockService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/InterlockService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/LiffService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/LiffService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/LoginService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/LoginService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/OaMembershipService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/OaMembershipService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/PrimaryAccountInitService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/PrimaryAccountInitService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/PwlessPrimaryRegistrationService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/PwlessPrimaryRegistrationService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/RelationService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/RelationService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/SearchService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/SearchService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/SecondaryPwlessLoginService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/SecondaryPwlessLoginService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/SettingsService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/ShopService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/ShopService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/SquareLiveTalkService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/SquareLiveTalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/SquareService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/SquareService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/TalkService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/TalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/TestService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/TestService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/AccessTokenRefreshService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/AccessTokenRefreshService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/BuddyService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/BuddyService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/CallService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/CallService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/E2EEKeyBackupService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/E2EEKeyBackupService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/HomeSafetyCheckService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/HomeSafetyCheckService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/SquareLiveTalkService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/SquareLiveTalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/SquareService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/SquareService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/SyncService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/SyncService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/TalkService.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/TalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TBase.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TBase.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TBinaryProtocol.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TBinaryProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TCompactProtocol.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TCompactProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TProtocol.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/ap/TProtocolDecorator.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/ap/TProtocolDecorator.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/services/thrift/ttypes.py` & `LINEBOOP-1.0.2/LINEBOOP/services/thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/thrift.py` & `LINEBOOP-1.0.2/LINEBOOP/thrift.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/timeline.py` & `LINEBOOP-1.0.2/LINEBOOP/timeline.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP/timelineBiz.py` & `LINEBOOP-1.0.2/LINEBOOP/timelineBiz.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/LINEBOOP.egg-info/PKG-INFO` & `LINEBOOP-1.0.2/LINEBOOP.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LINEBOOP
-Version: 1.0.1
+Version: 1.0.2
 Summary: LINE API! Upgrade Proxy
 Home-page: https://github.com/DeachSword/CHRLINE
 Author: DeachSword
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome==3.9.8
```

### Comparing `LINEBOOP-1.0.1/LINEBOOP.egg-info/SOURCES.txt` & `LINEBOOP-1.0.2/LINEBOOP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.1/PKG-INFO` & `LINEBOOP-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LINEBOOP
-Version: 1.0.1
+Version: 1.0.2
 Summary: LINE API! Upgrade Proxy
 Home-page: https://github.com/DeachSword/CHRLINE
 Author: DeachSword
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome==3.9.8
```

### Comparing `LINEBOOP-1.0.1/setup.py` & `LINEBOOP-1.0.2/setup.py`

 * *Files identical despite different names*

