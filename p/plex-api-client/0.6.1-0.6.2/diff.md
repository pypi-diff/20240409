# Comparing `tmp/plex-api-client-0.6.1.tar.gz` & `tmp/plex-api-client-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-api-client-0.6.1.tar", last modified: Sat Apr  6 01:12:54 2024, max compression
+gzip compressed data, was "plex-api-client-0.6.2.tar", last modified: Tue Apr  9 01:14:59 2024, max compression
```

## Comparing `plex-api-client-0.6.1.tar` & `plex-api-client-0.6.2.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.673853 plex-api-client-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-06 01:12:54.673853 plex-api-client-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 01:12:54.673853 plex-api-client-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.649852 plex-api-client-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.653852 plex-api-client-0.6.1/src/plex_api/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.653852 plex-api-client-0.6.1/src/plex_api/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    18205 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/hubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42832 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.653852 plex-api-client-0.6.1/src/plex_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.653852 plex-api-client-0.6.1/src/plex_api/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.661852 plex-api-client-0.6.1/src/plex_api/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/errors/uploadplaylist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.673853 plex-api-client-0.6.1/src/plex_api/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/addplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/applyupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/cancelserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/checkforupdates.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/clearplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/createplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/deletelibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/deleteplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/enablepapertrail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getavailableclients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getbutlertasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getfilehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getglobalhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getlibraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getlibraryhubs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getlibraryitems.py
--rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getmetadatachildren.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getmyplexaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getondeck.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getpin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getplaylistcontents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getplaylists.py
--rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getrecentlyadded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getresizedphoto.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getsearchresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getserveractivities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getservercapabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getserveridentity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getserverlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getserverpreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getsessionhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getsessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getsourceconnectioninformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getstatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/gettimeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/gettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/gettranscodesessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/gettransienttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/getupdatestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/logline.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/logmultiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/markplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/markunplayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/performsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/performvoicesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/refreshlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/searchlibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/startalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/starttask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/startuniversaltranscode.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/stopalltasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/stoptask.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/stoptranscodesession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/updateplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/updateplayprogress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/models/operations/uploadplaylist.py
--rw-r--r--   0 runner    (1001) docker     (127)    34761 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/plex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    28065 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14385 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.673853 plex-api-client-0.6.1/src/plex_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-06 01:12:43.000000 plex-api-client-0.6.1/src/plex_api/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:12:54.673853 plex-api-client-0.6.1/src/plex_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-06 01:12:54.000000 plex-api-client-0.6.1/src/plex_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-06 01:12:54.000000 plex-api-client-0.6.1/src/plex_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:12:54.000000 plex-api-client-0.6.1/src/plex_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 01:12:54.000000 plex-api-client-0.6.1/src/plex_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 01:12:54.000000 plex-api-client-0.6.1/src/plex_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14178 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.289967 plex-api-client-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18207 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/hubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42834 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.293967 plex-api-client-0.6.2/src/plex_api/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.301967 plex-api-client-0.6.2/src/plex_api/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/errors/uploadplaylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/src/plex_api/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/addplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/applyupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/cancelserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/checkforupdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/clearplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/createplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/deletelibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/deleteplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/enablepapertrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getavailableclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getbutlertasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7952 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getglobalhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6294 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18873 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryhubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21445 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26862 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getmetadatachildren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getmyplexaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18560 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getondeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getpin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getplaylistcontents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getplaylists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getrecentlyadded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getresizedphoto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsearchresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserveractivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getservercapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserveridentity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserverlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getserverpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsessionhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getsourceconnectioninformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettimeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettranscodesessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/gettransienttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/getupdatestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/logline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/logmultiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/markplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/markunplayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/performsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/performvoicesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/refreshlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/searchlibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/startalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/starttask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/startuniversaltranscode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/stopalltasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/stoptask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/stoptranscodesession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/updateplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/updateplayprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/models/operations/uploadplaylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34763 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/plex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/src/plex_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-09 01:14:50.000000 plex-api-client-0.6.2/src/plex_api/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:14:59.313967 plex-api-client-0.6.2/src/plex_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21032 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 01:14:59.000000 plex-api-client-0.6.2/src/plex_api_client.egg-info/top_level.txt
```

### Comparing `plex-api-client-0.6.1/LICENSE.md` & `plex-api-client-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/PKG-INFO` & `plex-api-client-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.1 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.2 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
```

### Comparing `plex-api-client-0.6.1/README.md` & `plex-api-client-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/setup.py` & `plex-api-client-0.6.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='plex-api-client',
-    version='0.6.1',
+    version='0.6.2',
     author='LukeHagar',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/LukeHagar/plexpy.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
@@ -40,14 +40,16 @@
         "six>=1.16.0",
         "typing-inspect>=0.9.0",
         "typing_extensions>=4.7.1",
         "urllib3>=1.26.18",
     ],
     extras_require={
         "dev": [
-            "pylint==2.16.2",
+            "pylint==3.1.0",
         ],
     },
     package_dir={'': 'src'},
     python_requires='>=3.8',
-    package_data={'plex-api-client': ['py.typed']},
+    package_data={
+        'plex-api-client': ['py.typed']
+    },
 )
```

### Comparing `plex-api-client-0.6.1/src/plex_api/_hooks/registration.py` & `plex-api-client-0.6.2/src/plex_api/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/_hooks/sdkhooks.py` & `plex-api-client-0.6.2/src/plex_api/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/_hooks/types.py` & `plex-api-client-0.6.2/src/plex_api/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/activities.py` & `plex-api-client-0.6.2/src/plex_api/activities.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/authentication.py` & `plex-api-client-0.6.2/src/plex_api/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/butler.py` & `plex-api-client-0.6.2/src/plex_api/butler.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,8 +326,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/hubs.py` & `plex-api-client-0.6.2/src/plex_api/hubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,8 +151,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/library.py` & `plex-api-client-0.6.2/src/plex_api/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -801,8 +801,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/log.py` & `plex-api-client-0.6.2/src/plex_api/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,8 +218,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/media.py` & `plex-api-client-0.6.2/src/plex_api/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,8 +203,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/__init__.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/addplaylistcontents.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/applyupdates.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/cancelserveractivities.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/checkforupdates.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/clearplaylistcontents.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/createplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/deletelibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/deleteplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/enablepapertrail.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getavailableclients.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getbutlertasks.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getdevices.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getfilehash.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getglobalhubs.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getlibraries.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getlibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getlibraryhubs.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getmetadata.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getmetadatachildren.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getmyplexaccount.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getondeck.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getpin.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getplaylistcontents.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getplaylists.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getrecentlyadded.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getresizedphoto.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getsearchresults.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getserveractivities.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getservercapabilities.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getserveridentity.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getserverlist.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getserverpreferences.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getsessionhistory.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getsessions.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getsourceconnectioninformation.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getstatistics.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/gettimeline.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/gettoken.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/gettranscodesessions.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/gettransienttoken.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/getupdatestatus.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/logline.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/logmultiline.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/markplayed.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/markunplayed.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/performsearch.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/performvoicesearch.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/refreshlibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/sdkerror.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/startalltasks.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/starttask.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/startuniversaltranscode.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/stopalltasks.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/stoptask.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/stoptranscodesession.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/updateplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/updateplayprogress.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/errors/uploadplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/errors/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/__init__.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/addplaylistcontents.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/addplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/applyupdates.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/applyupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/cancelserveractivities.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/cancelserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/checkforupdates.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/checkforupdates.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/clearplaylistcontents.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/clearplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/createplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/createplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/deletelibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/deletelibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/deleteplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/deleteplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/enablepapertrail.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/enablepapertrail.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getavailableclients.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getavailableclients.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getbutlertasks.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getbutlertasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getdevices.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getdevices.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getfilehash.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getfilehash.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getglobalhubs.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getglobalhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getlibraries.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getlibraries.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getlibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getlibraryhubs.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryhubs.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getlibraryitems.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getlibraryitems.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getmetadata.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getmetadata.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getmetadatachildren.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getmetadatachildren.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getmyplexaccount.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getmyplexaccount.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getondeck.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getondeck.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getpin.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getpin.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getplaylistcontents.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getplaylistcontents.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getplaylists.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getplaylists.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getrecentlyadded.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getrecentlyadded.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getresizedphoto.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getresizedphoto.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getsearchresults.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getsearchresults.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getserveractivities.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getserveractivities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getservercapabilities.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getservercapabilities.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getserveridentity.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getserveridentity.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getserverlist.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getserverlist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getserverpreferences.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getserverpreferences.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getsessionhistory.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getsessionhistory.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getsessions.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getsessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getsourceconnectioninformation.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getsourceconnectioninformation.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getstatistics.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getstatistics.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/gettimeline.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/gettimeline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/gettoken.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/gettoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/gettranscodesessions.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/gettranscodesessions.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/gettransienttoken.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/gettransienttoken.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/getupdatestatus.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/getupdatestatus.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/logline.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/logline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/logmultiline.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/logmultiline.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/markplayed.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/markplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/markunplayed.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/markunplayed.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/performsearch.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/performsearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/performvoicesearch.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/performvoicesearch.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/refreshlibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/refreshlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/searchlibrary.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/searchlibrary.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/startalltasks.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/startalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/starttask.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/starttask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/startuniversaltranscode.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/startuniversaltranscode.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/stopalltasks.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/stopalltasks.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/stoptask.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/stoptask.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/stoptranscodesession.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/stoptranscodesession.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/updateplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/updateplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/updateplayprogress.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/updateplayprogress.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/models/operations/uploadplaylist.py` & `plex-api-client-0.6.2/src/plex_api/models/operations/uploadplaylist.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/playlists.py` & `plex-api-client-0.6.2/src/plex_api/playlists.py`

 * *Files 0% similar despite different names*

```diff
@@ -622,8 +622,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/plex.py` & `plex-api-client-0.6.2/src/plex_api/plex.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,8 +147,9 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/sdk.py` & `plex-api-client-0.6.2/src/plex_api/sdk.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/sdkconfiguration.py` & `plex-api-client-0.6.2/src/plex_api/sdkconfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     server_defaults: List[Dict[str, str]] = field(default_factory=List)
     globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.0.3'
-    sdk_version: str = '0.6.1'
-    gen_version: str = '2.298.2'
-    user_agent: str = 'speakeasy-sdk/python 0.6.1 2.298.2 0.0.3 plex-api-client'
+    sdk_version: str = '0.6.2'
+    gen_version: str = '2.300.0'
+    user_agent: str = 'speakeasy-sdk/python 0.6.2 2.300.0 0.0.3 plex-api-client'
     retry_config: Optional[RetryConfig] = None
     _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
```

### Comparing `plex-api-client-0.6.1/src/plex_api/search.py` & `plex-api-client-0.6.2/src/plex_api/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,8 +225,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/server.py` & `plex-api-client-0.6.2/src/plex_api/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,8 +518,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/sessions.py` & `plex-api-client-0.6.2/src/plex_api/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,8 +265,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/statistics.py` & `plex-api-client-0.6.2/src/plex_api/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/updater.py` & `plex-api-client-0.6.2/src/plex_api/updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,8 +205,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api/utils/retries.py` & `plex-api-client-0.6.2/src/plex_api/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `plex-api-client-0.6.1/src/plex_api/utils/utils.py` & `plex-api-client-0.6.2/src/plex_api/utils/utils.py`

 * *Files identical despite different names*

### Comparing `plex-api-client-0.6.1/src/plex_api/video.py` & `plex-api-client-0.6.2/src/plex_api/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,8 +129,9 @@
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `plex-api-client-0.6.1/src/plex_api_client.egg-info/PKG-INFO` & `plex-api-client-0.6.2/src/plex_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-api-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/LukeHagar/plexpy.git
 Author: LukeHagar
 License: UNKNOWN
 Description: # plexpy
         
         <div align="left">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.1 Summary: Python
+Metadata-Version: 2.1 Name: plex-api-client Version: 0.6.2 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/LukeHagar/
 plexpy.git Author: LukeHagar License: UNKNOWN Description: # plexpy
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## SDK Installation ```bash pip install plex-api-client ``` ## SDK Example
 Usage ### Example ```python import plex_api s = plex_api.PlexAPI
```

### Comparing `plex-api-client-0.6.1/src/plex_api_client.egg-info/SOURCES.txt` & `plex-api-client-0.6.2/src/plex_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

