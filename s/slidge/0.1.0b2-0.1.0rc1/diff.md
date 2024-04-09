# Comparing `tmp/slidge-0.1.0b2.tar.gz` & `tmp/slidge-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidge-0.1.0b2.tar", max compression
+gzip compressed data, was "slidge-0.1.0rc1.tar", max compression
```

## Comparing `slidge-0.1.0b2.tar` & `slidge-0.1.0rc1.tar`

### file list

```diff
@@ -1,81 +1,99 @@
--rw-r--r--   0        0        0    34523 2022-10-30 13:34:03.847762 slidge-0.1.0b2/LICENSE
--rw-r--r--   0        0        0     5806 2022-10-30 13:34:03.847762 slidge-0.1.0b2/README.md
--rw-r--r--   0        0        0     1730 2022-10-30 14:13:39.658180 slidge-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0      707 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/__init__.py
--rw-r--r--   0        0        0     5656 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/__main__.py
--rw-r--r--   0        0        0       36 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/core/__init__.py
--rw-r--r--   0        0        0    30717 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/core/contact.py
--rw-r--r--   0        0        0    34192 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/core/gateway.py
--rw-r--r--   0        0        0    12277 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/core/pubsub.py
--rw-r--r--   0        0        0    18164 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/core/session.py
--rw-r--r--   0        0        0        0 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/__init__.py
--rw-r--r--   0        0        0     2768 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/discord/__init__.py
--rw-r--r--   0        0        0     3852 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/discord/client.py
--rw-r--r--   0        0        0     5726 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/discord/session.py
--rw-r--r--   0        0        0     6386 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/dummy.py
--rw-r--r--   0        0        0    19335 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/facebook.py
--rw-r--r--   0        0        0     7710 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/hackernews.py
--rw-r--r--   0        0        0       38 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/mattermost/__init__.py
--rw-r--r--   0        0        0     9494 2022-10-30 13:34:03.867762 slidge-0.1.0b2/slidge/plugins/mattermost/api.py
--rw-r--r--   0        0        0    14091 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/mattermost/gateway.py
--rw-r--r--   0        0        0     8519 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/mattermost/websocket.py
--rw-r--r--   0        0        0       95 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/signal/__init__.py
--rw-r--r--   0        0        0     3376 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/signal/contact.py
--rw-r--r--   0        0        0     9435 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/signal/gateway.py
--rw-r--r--   0        0        0    16466 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/signal/session.py
--rw-r--r--   0        0        0     1775 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/signal/txt.py
--rw-r--r--   0        0        0    12247 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/skype.py
--rw-r--r--   0        0        0    11077 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/steam.py
--rw-r--r--   0        0        0      161 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/telegram/__init__.py
--rw-r--r--   0        0        0     9318 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/telegram/client.py
--rw-r--r--   0        0        0      329 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/telegram/config.py
--rw-r--r--   0        0        0     6600 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/telegram/contact.py
--rw-r--r--   0        0        0     5239 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/telegram/gateway.py
--rw-r--r--   0        0        0     9100 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/plugins/telegram/session.py
--rw-r--r--   0        0        0      299 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/__init__.py
--rw-r--r--   0        0        0     7059 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/db.py
--rw-r--r--   0        0        0     3160 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/test.py
--rw-r--r--   0        0        0      197 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/types.py
--rw-r--r--   0        0        0     3756 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/util.py
--rw-r--r--   0        0        0      372 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0030/__init__.py
--rw-r--r--   0        0        0    31617 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0030/disco.py
--rw-r--r--   0        0        0      292 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0030/stanza/__init__.py
--rw-r--r--   0        0        0    10428 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0030/stanza/info.py
--rw-r--r--   0        0        0     4608 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0030/stanza/items.py
--rw-r--r--   0        0        0    17117 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0030/static.py
--rw-r--r--   0        0        0      106 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0055/__init__.py
--rw-r--r--   0        0        0     2466 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0055/search.py
--rw-r--r--   0        0        0      231 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0055/stanza.py
--rw-r--r--   0        0        0      325 2022-10-30 13:34:03.871095 slidge-0.1.0b2/slidge/util/xep_0077/__init__.py
--rw-r--r--   0        0        0     9891 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0077/register.py
--rw-r--r--   0        0        0     2186 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0077/stanza.py
--rw-r--r--   0        0        0      334 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0084/__init__.py
--rw-r--r--   0        0        0     3915 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0084/avatar.py
--rw-r--r--   0        0        0     2773 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0084/stanza.py
--rw-r--r--   0        0        0      107 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0100/__init__.py
--rw-r--r--   0        0        0     4101 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0100/gateway.py
--rw-r--r--   0        0        0      358 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0115/__init__.py
--rw-r--r--   0        0        0    13541 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0115/caps.py
--rw-r--r--   0        0        0      431 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0115/stanza.py
--rw-r--r--   0        0        0     5185 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0115/static.py
--rw-r--r--   0        0        0       29 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0292/__init__.py
--rw-r--r--   0        0        0     3782 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0292/stanza.py
--rw-r--r--   0        0        0     2148 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0292/vcard4.py
--rw-r--r--   0        0        0      325 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0333/__init__.py
--rw-r--r--   0        0        0     3025 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0333/markers.py
--rw-r--r--   0        0        0      726 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0333/stanza.py
--rw-r--r--   0        0        0      166 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356/__init__.py
--rw-r--r--   0        0        0      625 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356/permissions.py
--rw-r--r--   0        0        0     5204 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356/privilege.py
--rw-r--r--   0        0        0     1206 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356/stanza.py
--rw-r--r--   0        0        0      180 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356_old/__init__.py
--rw-r--r--   0        0        0     5299 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356_old/privilege.py
--rw-r--r--   0        0        0     1229 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0356_old/stanza.py
--rw-r--r--   0        0        0      405 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0363/__init__.py
--rw-r--r--   0        0        0     7999 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0363/http_upload.py
--rw-r--r--   0        0        0     1137 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0363/stanza.py
--rw-r--r--   0        0        0      127 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0461/__init__.py
--rw-r--r--   0        0        0     1383 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0461/reply.py
--rw-r--r--   0        0        0     1357 2022-10-30 13:34:03.874428 slidge-0.1.0b2/slidge/util/xep_0461/stanza.py
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 slidge-0.1.0b2/setup.py
--rw-r--r--   0        0        0     7356 1970-01-01 00:00:00.000000 slidge-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-01-08 11:57:11.502146 slidge-0.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     5897 2023-01-08 11:57:11.502146 slidge-0.1.0rc1/README.md
+-rw-r--r--   0        0        0     1792 2023-01-08 12:30:23.708005 slidge-0.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      841 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/__init__.py
+-rw-r--r--   0        0        0     4257 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/__main__.py
+-rw-r--r--   0        0        0       36 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/core/__init__.py
+-rw-r--r--   0        0        0    17007 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/core/adhoc.py
+-rw-r--r--   0        0        0     2918 2023-01-08 11:57:11.525481 slidge-0.1.0rc1/slidge/core/cache.py
+-rw-r--r--   0        0        0     7020 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/chat_command.py
+-rw-r--r--   0        0        0     3215 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/config.py
+-rw-r--r--   0        0        0    14880 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/contact.py
+-rw-r--r--   0        0        0     1707 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/disco.py
+-rw-r--r--   0        0        0    33682 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/gateway.py
+-rw-r--r--   0        0        0      307 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/__init__.py
+-rw-r--r--   0        0        0     1072 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/base.py
+-rw-r--r--   0        0        0     2113 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/disco.py
+-rw-r--r--   0        0        0    14819 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/message.py
+-rw-r--r--   0        0        0     3770 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/mixins/presence.py
+-rw-r--r--   0        0        0      119 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/__init__.py
+-rw-r--r--   0        0        0     2697 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/bookmarks.py
+-rw-r--r--   0        0        0     5148 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/participant.py
+-rw-r--r--   0        0        0    11126 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/muc/room.py
+-rw-r--r--   0        0        0    12305 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/pubsub.py
+-rw-r--r--   0        0        0    24193 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/core/session.py
+-rw-r--r--   0        0        0        0 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/plugins/__init__.py
+-rw-r--r--   0        0        0     3759 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/plugins/discord/__init__.py
+-rw-r--r--   0        0        0     4357 2023-01-08 11:57:11.528815 slidge-0.1.0rc1/slidge/plugins/discord/client.py
+-rw-r--r--   0        0        0     5841 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/discord/session.py
+-rw-r--r--   0        0        0    10479 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/dummy.py
+-rw-r--r--   0        0        0    22184 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/facebook.py
+-rw-r--r--   0        0        0     7604 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/hackernews.py
+-rw-r--r--   0        0        0       38 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/__init__.py
+-rw-r--r--   0        0        0     9601 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/api.py
+-rw-r--r--   0        0        0    16234 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/gateway.py
+-rw-r--r--   0        0        0     8504 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/mattermost/websocket.py
+-rw-r--r--   0        0        0      115 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/__init__.py
+-rw-r--r--   0        0        0      124 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/config.py
+-rw-r--r--   0        0        0     3572 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/contact.py
+-rw-r--r--   0        0        0    12953 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/gateway.py
+-rw-r--r--   0        0        0     2403 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/group.py
+-rw-r--r--   0        0        0    18611 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/session.py
+-rw-r--r--   0        0        0      555 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/txt.py
+-rw-r--r--   0        0        0     1112 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/signal/util.py
+-rw-r--r--   0        0        0    11606 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/skype.py
+-rw-r--r--   0        0        0    14752 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/steam.py
+-rw-r--r--   0        0        0      185 2023-01-08 11:57:11.532148 slidge-0.1.0rc1/slidge/plugins/telegram/__init__.py
+-rw-r--r--   0        0        0    13681 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/client.py
+-rw-r--r--   0        0        0      667 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/config.py
+-rw-r--r--   0        0        0     5527 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/contact.py
+-rw-r--r--   0        0        0     6687 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/gateway.py
+-rw-r--r--   0        0        0     6566 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/group.py
+-rw-r--r--   0        0        0     9339 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/session.py
+-rw-r--r--   0        0        0     6523 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/telegram/util.py
+-rw-r--r--   0        0        0      112 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/__init__.py
+-rw-r--r--   0        0        0      574 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/config.py
+-rw-r--r--   0        0        0     1095 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/contact.py
+-rw-r--r--   0        0        0    15365 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/event.go
+-rw-r--r--   0        0        0     4997 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/gateway.go
+-rw-r--r--   0        0        0     2281 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/gateway.py
+-rw-r--r--   0        0        0      484 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/go.mod
+-rw-r--r--   0        0        0     2064 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/go.sum
+-rw-r--r--   0        0        0    12445 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/session.go
+-rw-r--r--   0        0        0    14739 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/plugins/whatsapp/session.py
+-rw-r--r--   0        0        0      299 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/__init__.py
+-rw-r--r--   0        0        0     5708 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/conf.py
+-rw-r--r--   0        0        0     7758 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/db.py
+-rw-r--r--   0        0        0     9295 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/test.py
+-rw-r--r--   0        0        0     1633 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/types.py
+-rw-r--r--   0        0        0     3596 2023-01-08 11:57:11.535482 slidge-0.1.0rc1/slidge/util/util.py
+-rw-r--r--   0        0        0      372 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/__init__.py
+-rw-r--r--   0        0        0    31653 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/disco.py
+-rw-r--r--   0        0        0      292 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/stanza/__init__.py
+-rw-r--r--   0        0        0    10428 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/stanza/info.py
+-rw-r--r--   0        0        0     4608 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/stanza/items.py
+-rw-r--r--   0        0        0    17117 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0030/static.py
+-rw-r--r--   0        0        0      305 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0050/__init__.py
+-rw-r--r--   0        0        0    22499 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0050/adhoc.py
+-rw-r--r--   0        0        0     5814 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0050/stanza.py
+-rw-r--r--   0        0        0      325 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0077/__init__.py
+-rw-r--r--   0        0        0    10402 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0077/register.py
+-rw-r--r--   0        0        0     2186 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0077/stanza.py
+-rw-r--r--   0        0        0      107 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0100/__init__.py
+-rw-r--r--   0        0        0     4312 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0100/gateway.py
+-rw-r--r--   0        0        0      232 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0100/stanza.py
+-rw-r--r--   0        0        0       29 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0292/__init__.py
+-rw-r--r--   0        0        0     3782 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0292/stanza.py
+-rw-r--r--   0        0        0     2102 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0292/vcard4.py
+-rw-r--r--   0        0        0      166 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/__init__.py
+-rw-r--r--   0        0        0      625 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/permissions.py
+-rw-r--r--   0        0        0     5204 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/privilege.py
+-rw-r--r--   0        0        0     1206 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356/stanza.py
+-rw-r--r--   0        0        0      180 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356_old/__init__.py
+-rw-r--r--   0        0        0     5299 2023-01-08 11:57:11.538815 slidge-0.1.0rc1/slidge/util/xep_0356_old/privilege.py
+-rw-r--r--   0        0        0     1229 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0356_old/stanza.py
+-rw-r--r--   0        0        0      126 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0461/__init__.py
+-rw-r--r--   0        0        0     1383 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0461/reply.py
+-rw-r--r--   0        0        0     2390 2023-01-08 11:57:11.542149 slidge-0.1.0rc1/slidge/util/xep_0461/stanza.py
+-rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 slidge-0.1.0rc1/setup.py
+-rw-r--r--   0        0        0     7457 1970-01-01 00:00:00.000000 slidge-0.1.0rc1/PKG-INFO
```

### Comparing `slidge-0.1.0b2/LICENSE` & `slidge-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/README.md` & `slidge-0.1.0rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,51 +18,51 @@
 It's a work in progress, but it should make
 [writing gateways to other chat networks](https://slidge.readthedocs.io/en/latest/dev/tutorial.html)
 (*plugins*) as frictionless as possible.
 
 It comes with a few plugins included, implementing at least basic direct messaging and often more "advanced"
 instant messaging features:
 
-|            | Presences[¹] | Typing[²] | Marks[³] | Upload[⁴] | Edit[⁵] | React[⁶] | Retract[⁷] | Reply[⁸] | 
-|------------|--------------|-----------|----------|-----------|---------|----------|------------|----------|
-| Signal     | N/A          | ✅         | ✅        | ✅         | N/A     | ✅        | ✅          | ✅        |
-| Telegram   | ✅            | ✅         | ✅        | ✅         | ✅       | ✅        | ✅          | ✅        |
-| Discord    | ❌            | ✅         | N/A      | ✅         | ✅       | ~        | ✅          | ✅        |
-| Steam      | ✅            | ✅         | N/A      | ❌         | N/A     | ~        | N/A        | N/A      |
-| Mattermost | ✅            | ✅         | ~        | ✅         | ✅       | ✅        | ✅          | ❌        |
-| Facebook   | ❌            | ✅         | ✅        | ✅         | ✅       | ✅        | ✅          | ✅        |
-| Skype      | ✅            | ✅         | ❌        | ✅         | ✅       | ❌        | ✅          | ❌        |
+|            | Presences[¹] | Typing[²] | Marks[³] | Upload[⁴] | Edit[⁵] | React[⁶] | Retract[⁷] | Reply[⁸] | Groups[⁹] |
+|------------|--------------|-----------|----------|-----------|---------|----------|------------|----------|-----------|
+| Signal     | N/A          | ✅        | ✅       | ✅        | N/A     | ✅       | ✅         | ✅       | ~         |
+| Telegram   | ✅           | ✅        | ✅       | ✅        | ✅      | ✅       | ✅         | ✅       | ~         |
+| Discord    | ❌           | ✅        | N/A      | ✅        | ✅      | ~        | ✅         | ✅       | ❌         |
+| Steam      | ✅           | ✅        | N/A      | ❌        | N/A     | ~        | N/A        | N/A      | ❌         |
+| Mattermost | ✅           | ✅        | ~        | ✅        | ✅      | ✅       | ✅         | ❌       | ❌         |
+| Facebook   | ❌           | ✅        | ✅       | ✅        | ✅      | ✅       | ✅         | ✅       | ❌         |
+| Skype      | ✅           | ✅        | ❌       | ✅        | ✅      | ❌       | ✅         | ❌       | ❌         |
+| WhatsApp   | ✅           | ✅        | ✅       | ✅        | N/A     | ✅       | ✅         | ✅       | ❌         |
 
 
 [¹]: https://xmpp.org/rfcs/rfc6121.html#presence
 [²]: https://xmpp.org/extensions/xep-0085.html
 [³]: https://xmpp.org/extensions/xep-0333.html
 [⁴]: https://xmpp.org/extensions/xep-0363.html
 [⁵]: https://xmpp.org/extensions/xep-0308.html
 [⁶]: https://xmpp.org/extensions/xep-0444.html
 [⁷]: https://xmpp.org/extensions/xep-0424.html
 [⁸]: https://xmpp.org/extensions/xep-0461.html
+[⁹]: https://xmpp.org/extensions/xep-0045.html
 
 
 This table may not be entirely accurate, but **in theory**, stuff marked ✅ works.
 N/A means that the legacy network does not have an equivalent of this XMPP feature
 (because XMPP is better, what did you think?).
 
 **WARNING**: you may break the terms of use of a legacy network and end up getting your account locked
 by using slidge. Refer to the
 [keeping a low profile](https://slidge.readthedocs.io/en/latest/user/low_profile.html)
 documentation page for more info.
 
 Status
 ------
 
-Slidge is beta-grade software.
-Right now, only direct messages are implemented, no group chat stuff at all.
-Direct messaging does (more or less) work though.
-Any contribution whatsoever (testing, patches, suggestions, beer, …) is more than welcome.
+Slidge is **beta**-grade software for 1:1 chats.
+Group chat support is **experimental**.
 
 Try slidge and give us some
 feedback, through the [MUC](xmpp:slidge@conference.nicoco.fr?join), the
 [issue tracker](https://todo.sr.ht/~nicoco/slidge) or in the
 [public inbox](https://lists.sr.ht/~nicoco/public-inbox).
 Don't be shy!
```

### Comparing `slidge-0.1.0b2/pyproject.toml` & `slidge-0.1.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [tool.poetry]
 name = "slidge"
-version = "0.1.0-beta2"
+version = "0.1.0rc1"
 description = "XMPP bridging framework"
 authors = ["Nicolas Cedilnik <nicoco@nicoco.fr>"]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://sr.ht/~nicoco/slidge/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-slixmpp = "^1.8.2"
+slixmpp = "^1.8.3"
 qrcode = ">=7.3"
 Pillow = ">=8.1.0"
 aiohttp = ">=3.6.0"
 ConfigArgParse = "^1.5.3"
 
 aiotdlib = { version = "^0.19.2", optional = true }
 pydantic = { version = "*", optional = true }
 aiosignald = { version = "^0.3.4", optional = true }
-mautrix-facebook = { version = "^0.4.0", optional = true }
+mautrix-facebook = { version = "^0.4.1", optional = true }
 mattermost-api-reference-client = { version =  "^4.0.0", optional = true }
 emoji = { version =  "^2.0.0", optional = true }
 SkPy = { version =  "^0.10.4", optional = true }
 steam = {extras = ["client"], version = "^1.3.0", optional = true }
 "discord.py-self" = { version = "^1.9.2", optional = true }
 pickle-secure = "^0.9.99"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-asyncio = "*"
 black = { version = "*", extras = ["d"] }
-Sphinx = "^5"
+Sphinx = "^6"
 Pygments = "^2.8.0"
-sphinx-argparse = "^0.3.1"
+sphinx-argparse = "^0.4.0"
 sphinx-autoapi = "^2.0.0"
 furo = "^2022.6.21"
-mypy = "^0.982"
+mypy = "^0.991"
 types-requests = "^2.28.1"
-isort = "^5.10.1"
+isort = "^5.11.4"
 types-emoji = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
@@ -53,12 +53,13 @@
 skype = ["SkPy"]
 steam = ["steam", "asyncio-gevent"]
 
 [tool.poetry.scripts]
 slidge = 'slidge.__main__:main'
 
 [tool.mypy]
-exclude = "slidge.util.xep*"
+exclude = ["slidge.util.xep*", "slidge/plugins/whatsapp/generated"]
 ignore_missing_imports = true
+check_untyped_defs = true
 
 [tool.black]
 exclude = "xep_*"
```

### Comparing `slidge-0.1.0b2/slidge/core/contact.py` & `slidge-0.1.0rc1/slidge/core/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,891 +1,700 @@
 import functools
 import logging
-from datetime import date, datetime, timezone
-from io import BytesIO
-from pathlib import Path
-from typing import (
-    IO,
-    TYPE_CHECKING,
-    Any,
-    Generic,
-    Iterable,
-    Literal,
-    Optional,
-    Type,
-    TypeVar,
-    Union,
-)
+from typing import Generic, Optional, Type, Union, cast
 
-import aiohttp
-from slixmpp import JID, Message
+from slixmpp import JID, Message, Presence
+from slixmpp.exceptions import XMPPError
 
-from ..util import SubclassableOnce
+from ..util import ABCSubclassableOnceAtMost, BiDict
+from ..util.db import GatewayUser, user_store
 from ..util.types import (
-    AvatarType,
-    LegacyContactIdType,
+    BookmarksType,
+    Chat,
+    GatewayType,
+    LegacyContactType,
     LegacyMessageType,
-    LegacyUserIdType,
+    LegacyMUCType,
+    LegacyParticipantType,
+    LegacyRosterType,
+    PresenceShow,
+    SessionType,
 )
-from ..util.xep_0292.stanza import VCard4
-from ..util.xep_0363 import FileUploadError
+from ..util.util import SearchResult
+from .contact import LegacyRoster
+from .muc.bookmarks import LegacyBookmarks
+from .muc.room import LegacyMUC
 
-if TYPE_CHECKING:
-    from .session import SessionType
-else:
-    SessionType = TypeVar("SessionType")
 
+def ignore_sent_carbons(func):
+    @functools.wraps(func)
+    async def wrapped(self: SessionType, msg: Message):
+        if (i := msg.get_id()) in self.ignore_messages:
+            self.log.debug("Ignored sent carbon: %s", i)
+            self.ignore_messages.remove(i)
+        else:
+            return await func(self, msg)
 
-class LegacyContact(Generic[SessionType], metaclass=SubclassableOnce):
-    """
-    This class centralizes actions in relation to a specific legacy contact.
+    return wrapped
 
-    You shouldn't create instances of contacts manually, but rather rely on
-    :meth:`.LegacyRoster.by_legacy_id` to ensure that contact instances are
-    singletons. The :class:`.LegacyRoster` instance of a session is accessible
-    through the :attr:`.BaseSession.contacts` attribute.
-
-    Typically, your plugin should have methods hook to the legacy events and
-    call appropriate methods here to transmit the "legacy action" to the xmpp
-    user. This should look like this:
-
-    .. code-block:python
-
-        class Session(BaseSession):
-            ...
-
-            async def on_cool_chat_network_new_text_message(self, legacy_msg_event):
-                contact = self.contacts.by_legacy_id(legacy_msg_event.from)
-                contact.send_text(legacy_msg_event.text)
-
-            async def on_cool_chat_network_new_typing_event(self, legacy_typing_event):
-                contact = self.contacts.by_legacy_id(legacy_msg_event.from)
-                contact.composing()
-            ...
-    """
 
-    RESOURCE: str = "slidge"
-    """
-    A full JID, including a resource part is required for chat states (and maybe other stuff)
-    to work properly. This is the name of the resource the contacts will use.
+def ignore_message_to_component(func):
+    @functools.wraps(func)
+    async def wrapped(self: SessionType, msg: Message):
+        if msg.get_to() != self.xmpp.boundjid.bare:
+            return await func(self, msg)
+        else:
+            log.debug("Ignoring message to component: %s %s", self, msg)
+
+    return wrapped
+
+
+class BaseSession(
+    Generic[
+        GatewayType,
+        LegacyMessageType,
+        LegacyRosterType,
+        LegacyContactType,
+        BookmarksType,
+        LegacyMUCType,
+        LegacyParticipantType,
+    ],
+    metaclass=ABCSubclassableOnceAtMost,
+):
     """
+    Represents a gateway user logged in to the legacy network and performing actions.
 
-    AVATAR = True
-    RECEIPTS = True
-    MARKS = True
-    CHAT_STATES = True
-    UPLOAD = True
-    CORRECTION = True
-    REACTION = True
-    RETRACTION = True
-    REPLIES = True
+    Will be instantiated automatically when a user sends an online presence to the gateway
+    component, as per :xep:`0100`.
 
+    Must be subclassed for a functional slidge plugin.
     """
-    A list of features advertised through service discovery and client capabilities.
+
+    sent: BiDict[LegacyMessageType, str]
+    """
+    Since we cannot set the XMPP ID of messages sent by XMPP clients, we need to keep a mapping
+    between XMPP IDs and legacy message IDs if we want to further refer to a message that was sent
+    by the user. This also applies to 'carboned' messages, ie, messages sent by the user from
+    the official client of a legacy network.
     """
 
-    CLIENT_TYPE = "pc"
+    xmpp: "GatewayType"
     """
-    https://xmpp.org/registrar/disco-categories.html#client
+    The gateway instance singleton. Use it for low-level XMPP calls or custom methods that are not
+    session-specific.
     """
 
-    def __init__(
-        self,
-        session: "SessionType",
-        legacy_id: LegacyContactIdType,
-        jid_username: str,
-    ):
-        """
-        :param session: The session this contact is part of
-        :param legacy_id: The contact's legacy ID
-        :param jid_username: User part of this contact's 'puppet' JID.
-            NB: case-insensitive, and some special characters are not allowed
-        """
-        self.session = session
-        self.user = session.user
-        self.legacy_id = legacy_id
-        self.jid_username = jid_username
+    def __init__(self, user: GatewayUser):
+        self._roster_cls: Type[
+            LegacyRosterType
+        ] = LegacyRoster.get_self_or_unique_subclass()
 
-        self.added_to_roster = False
+        self.log = logging.getLogger(user.bare_jid)
 
-        self._name: Optional[str] = None
-        self._avatar: Optional[AvatarType] = None
+        self.user = user
+        self.sent = BiDict[LegacyMessageType, str]()  # TODO: set a max size for this
+        # message ids (*not* stanza-ids), needed for last msg correction
+        self.muc_sent_msg_ids = BiDict[LegacyMessageType, str]()
 
-        self._subscribe_from = True
-        self._subscribe_to = True
+        self.ignore_messages = set[str]()
 
-        self.xmpp = session.xmpp
-        self.xmpp.loop.create_task(self.__make_caps())
+        self.contacts: LegacyRosterType = self._roster_cls(self)
+        self.never_logged = True
 
-    def __repr__(self):
-        return f"<LegacyContact <{self.jid}> ('{self.legacy_id}') of <{self.user}>"
+        self.bookmarks: BookmarksType = LegacyBookmarks.get_self_or_unique_subclass()(
+            self
+        )
 
-    def __get_subscription_string(self):
-        if self._subscribe_from and self._subscribe_to:
-            return "both"
-        if self._subscribe_from:
-            return "from"
-        if self._subscribe_to:
-            return "to"
-        return "none"
+    def shutdown(self):
+        for c in self.contacts:
+            c.offline()
+        for m in self.bookmarks:
+            m.shutdown()
+        self.xmpp.loop.create_task(self.logout())
 
-    async def __make_caps(self):
-        """
-        Configure slixmpp to correctly advertise this contact's capabilities.
+    @staticmethod
+    def legacy_msg_id_to_xmpp_msg_id(legacy_msg_id: LegacyMessageType) -> str:
         """
-        jid = self.jid
-        xmpp = self.xmpp
+        Convert a legacy msg ID to a valid XMPP msg ID.
+        Needed for read marks and message corrections.
 
-        xmpp["xep_0030"].add_identity(
-            jid=jid, category="client", itype=self.CLIENT_TYPE
-        )
-        add_feature = functools.partial(xmpp["xep_0030"].add_feature, jid=jid)
-        if self.CHAT_STATES:
-            await add_feature("http://jabber.org/protocol/chatstates")
-        if self.RECEIPTS:
-            await add_feature("urn:xmpp:receipts")
-        if self.CORRECTION:
-            await add_feature("urn:xmpp:message-correct:0")
-        if self.MARKS:
-            await add_feature("urn:xmpp:chat-markers:0")
-        if self.UPLOAD:
-            await add_feature("jabber:x:oob")
-        if self.REACTION:
-            await add_feature("urn:xmpp:reactions:0")
-        if self.RETRACTION:
-            await add_feature("urn:xmpp:message-retract:0")
-        if self.REPLIES:
-            await add_feature("urn:xmpp:reply:0")
-
-        await add_feature("urn:ietf:params:xml:ns:vcard-4.0")
-        await xmpp["xep_0115"].update_caps(jid=self.jid)
-
-    @property
-    def jid(self) -> JID:
-        """
-        Full JID (including the 'puppet' resource) of the contact
-        """
-        j = JID(self.jid_username + "@" + self.xmpp.boundjid.bare)
-        j.resource = self.RESOURCE
-        return j
-
-    @property
-    def name(self):
-        """
-        Friendly name of the contact, as it should appear in the user's roster
-        """
-        return self._name
-
-    @name.setter
-    def name(self, n: Optional[str]):
-        if self._name == n:
-            return
-        self._name = n
-        self.xmpp.pubsub.set_nick(
-            jid=self.jid.bare, nick=n, restrict_to=self.user.jid.bare
-        )
+        The default implementation just converts the legacy ID to a :class:`str`,
+        but this should be overridden in case some characters needs to be escaped,
+        or to add some additional, legacy network-specific logic.
 
-    @property
-    def avatar(self):
-        """
-        An image that represents this contact
+        :param legacy_msg_id:
+        :return: Should return a string that is usable as an XMPP stanza ID
         """
-        return self._avatar
-
-    @avatar.setter
-    def avatar(self, a: Optional[AvatarType]):
-        if a == self._avatar:
-            return
-        self.xmpp.loop.create_task(
-            self.xmpp.pubsub.set_avatar(
-                jid=self.jid.bare, avatar=a, restrict_to=self.user.jid.bare
-            )
-        )
-        self._avatar = a
-
-    def set_vcard(
-        self,
-        /,
-        full_name: Optional[str] = None,
-        given: Optional[str] = None,
-        surname: Optional[str] = None,
-        birthday: Optional[date] = None,
-        phone: Optional[str] = None,
-        note: Optional[str] = None,
-        url: Optional[str] = None,
-        email: Optional[str] = None,
-        country: Optional[str] = None,
-        locality: Optional[str] = None,
-    ):
-        vcard = VCard4()
-        vcard.add_impp(f"xmpp:{self.jid.bare}")
+        return str(legacy_msg_id)
 
-        if n := self.name:
-            vcard.add_nickname(n)
-        if full_name:
-            vcard["full_name"] = full_name
-        elif n:
-            vcard["full_name"] = n
-
-        if given:
-            vcard["given"] = given
-        if surname:
-            vcard["surname"] = surname
-        if birthday:
-            vcard["birthday"] = birthday
+    @staticmethod
+    def xmpp_msg_id_to_legacy_msg_id(i: str) -> LegacyMessageType:
+        """
+        Convert a legacy XMPP ID to a valid XMPP msg ID.
+        Needed for read marks and message corrections.
 
-        if note:
-            vcard.add_note(note)
-        if url:
-            vcard.add_url(url)
-        if email:
-            vcard.add_email(email)
-        if phone:
-            vcard.add_tel(phone)
-        if country and locality:
-            vcard.add_address(country, locality)
-        elif country:
-            vcard.add_address(country, locality)
+        The default implementation just converts the legacy ID to a :class:`str`,
+        but this should be overridden in case some characters needs to be escaped,
+        or to add some additional, legacy network-specific logic.
 
-        self.xmpp.vcard.set_vcard(self.jid.bare, vcard, {self.user.jid.bare})
+        The default implementation is an identity function
 
-    async def add_to_roster(self):
+        :param i: The XMPP stanza ID
+        :return: An ID that can be used to identify a message on the legacy network
         """
-        Add this contact to the user roster using :xep:`0356`
-        """
-        if self.xmpp.no_roster_push:
-            log.debug("Roster push request by plugin ignored (--no-roster-push)")
-            return
-        item = {
-            "subscription": self.__get_subscription_string(),
-            "groups": [self.xmpp.ROSTER_GROUP],
-        }
-        if (n := self.name) is not None:
-            item["name"] = n
-        kw = dict(
-            jid=self.user.jid,
-            roster_items={self.jid.bare: item},
-        )
-        try:
-            await self.xmpp["xep_0356"].set_roster(**kw)
-        except PermissionError:
-            try:
-                await self.xmpp["xep_0356_old"].set_roster(**kw)
-            except PermissionError:
-                log.warning(
-                    "Slidge does not have privileges to add contacts to the roster."
-                    "Refer to https://slidge.readthedocs.io/en/latest/admin/xmpp_server.html "
-                    "for more info."
-                )
-                return
+        return cast(LegacyMessageType, i)
 
-        self.added_to_roster = True
+    @classmethod
+    def _from_user_or_none(cls, user):
+        if user is None:
+            raise XMPPError(
+                text="User not found", condition="subscription-required", etype="auth"
+            )
 
-    def online(self, status: Optional[str] = None):
-        """
-        Send an "online" presence from this contact to the user.
+        session = _sessions.get(user)
+        if session is None:
+            _sessions[user] = session = cls(user)
+        return session
 
-        :param status: Arbitrary text, details of the status, eg: "Listening to Britney Spears"
-        """
-        self.xmpp.send_presence(pfrom=self.jid, pto=self.user.jid.bare, pstatus=status)
+    @classmethod
+    def from_user(cls, user):
+        return cls._from_user_or_none(user)
 
-    def away(self, status: Optional[str] = None):
+    @classmethod
+    def from_stanza(cls: Type[SessionType], s) -> SessionType:
         """
-        Send an "away" presence from this contact to the user.
+        Get a user's :class:`.LegacySession` using the "from" field of a stanza
 
-        This is a global status, as opposed to :meth:`.LegacyContact.inactive`
-        which concerns a specific conversation, ie a specific "chat window"
+        Meant to be called from :class:`BaseGateway` only.
 
-        :param status: Arbitrary text, details of the status, eg: "Gone to fight capitalism"
+        :param s:
+        :return:
         """
-        self.xmpp.send_presence(
-            pfrom=self.jid, pto=self.user.jid.bare, pshow="away", pstatus=status
-        )
+        return cls._from_user_or_none(user_store.get_by_stanza(s))
 
-    def extended_away(self, status: Optional[str] = None):
+    @classmethod
+    def from_jid(cls: Type[SessionType], jid: JID) -> SessionType:
         """
-        Send an "extended away" presence from this contact to the user.
+        Get a user's :class:`.LegacySession` using its jid
 
-        This is a global status, as opposed to :meth:`.LegacyContact.inactive`
-        which concerns a specific conversation, ie a specific "chat window"
+        Meant to be called from :class:`BaseGateway` only.
 
-        :param status: Arbitrary text, details of the status, eg: "Gone to fight capitalism"
-        """
-        self.xmpp.send_presence(
-            pfrom=self.jid, pto=self.user.jid.bare, pshow="xa", pstatus=status
-        )
-
-    def busy(self, status: Optional[str] = None):
+        :param jid:
+        :return:
         """
-        Send a "busy" presence from this contact to the user,
+        return cls._from_user_or_none(user_store.get_by_jid(jid))
 
-        :param status: eg: "Trying to make sense of XEP-0100"
+    @classmethod
+    async def kill_by_jid(cls, jid: JID):
         """
-        self.xmpp.send_presence(
-            pfrom=self.jid, pto=self.user.jid.bare, pshow="busy", pstatus=status
-        )
+        Terminate a user session.
 
-    def offline(self):
-        """
-        Send an "offline" presence from this contact to the user.
-        """
-        self.xmpp.send_presence(
-            pfrom=self.jid, pto=self.user.jid.bare, ptype="unavailable"
-        )
+        Meant to be called from :class:`BaseGateway` only.
 
-    def unsubscribe(self):
+        :param jid:
+        :return:
         """
-        Send an "unsubscribed" presence from this contact to the user.
+        log.debug("Killing session of %s", jid)
+        for user, session in _sessions.items():
+            if user.jid == jid.bare:
+                break
+        else:
+            log.debug("Did not find a session for %s", jid)
+            return
+        for c in session.contacts:
+            c.unsubscribe()
+        await session.logout()
+        await cls.xmpp.unregister(user)
+        del _sessions[user]
+        del user
+        del session
+
+    @ignore_message_to_component
+    @ignore_sent_carbons
+    async def send_from_msg(self, m: Message):
         """
-        self.xmpp.send_presence(
-            pfrom=self.jid, pto=self.user.jid.bare, ptype="unsubscribed"
-        )
+        Meant to be called from :class:`BaseGateway` only.
 
-    def status(self, text: str):
-        """
-        Set a contact's status
+        :param m:
+        :return:
         """
-        self.xmpp.send_presence(pfrom=self.jid, pto=self.user.jid.bare, pstatus=text)
+        # we MUST not use `if m["replace"]["id"]` because it adds the tag if not
+        # present. this is a problem for MUC echoed messages
+        if m.xml.find("{urn:xmpp:message-correct:0}replace") is not None:
+            # ignore last message correction (handled by a specific method)
+            return
+        if m.xml.find("{urn:xmpp:fasten:0}apply-to") is not None:
+            # ignore message retraction (handled by a specific method)
+            return
 
-    def __chat_state(self, state: str):
-        msg = self.xmpp.make_message(mfrom=self.jid, mto=self.user.jid, mtype="chat")
-        msg["chat_state"] = state
-        msg.enable("no-store")
-        msg.send()
+        e = await self.__get_entity(m)
+        self.log.debug("Entity %r", e)
 
-    def active(self):
-        """
-        Send an "active" chat state (:xep:`0085`) from this contact to the user.
-        """
-        self.__chat_state("active")
+        if m.xml.find("{jabber:x:oob}x") is not None:
+            url = m["oob"]["url"]
+        else:
+            url = None
 
-    def composing(self):
-        """
-        Send a "composing" (ie "typing notification") chat state (:xep:`0085`) from this contact to the user.
-        """
-        self.__chat_state("composing")
+        text = m["body"]
+        if m.xml.find("{urn:xmpp:fallback:0}fallback") is not None and (
+            isinstance(e, LegacyMUC) or e.REPLIES  # type: ignore
+        ):
+            text = m["feature_fallback"].get_stripped_body()
+            reply_fallback = m["feature_fallback"].get_fallback_body()
+        else:
+            reply_fallback = None
 
-    def paused(self):
-        """
-        Send a "paused" (ie "typing paused notification") chat state (:xep:`0085`) from this contact to the user.
-        """
-        self.__chat_state("paused")
+        # Testing with `is None` is mandatory since a reply element have no
+        # 'data' but only attributes, so the ElementTree is "false-ish".
+        # Grrrrr this took me some time to figure out.
+        reply_to = None
+        if m.xml.find("{urn:xmpp:reply:0}reply") is not None:
+            reply_to_msg_xmpp_id = self.__xmpp_msg_id_to_legacy(m["reply"]["id"])
+            reply_to_jid = JID(m["reply"]["to"])
+            if m["type"] == "chat":
+                if reply_to_jid.bare != self.user.jid.bare:
+                    try:
+                        reply_to = await self.contacts.by_jid(reply_to_jid)
+                    except XMPPError:
+                        pass
+            elif m["type"] == "groupchat":
+                nick = reply_to_jid.resource
+                try:
+                    muc = await self.bookmarks.by_jid(reply_to_jid)
+                except XMPPError:
+                    pass
+                else:
+                    if nick != muc.user_nick:
+                        reply_to = await muc.get_participant(reply_to_jid.resource)
+        else:
+            reply_to_msg_xmpp_id = None
+            reply_to = None
 
-    def inactive(self):
-        """
-        Send an "inactive" (ie "typing paused notification") chat state (:xep:`0085`) from this contact to the user.
-        """
-        log.debug("%s go inactive", self)
-        self.__chat_state("inactive")
+        kwargs = dict(
+            reply_to_msg_id=reply_to_msg_xmpp_id,
+            reply_to_fallback_text=reply_fallback,
+            reply_to=reply_to,
+        )
 
-    def __send_marker(
-        self,
-        legacy_msg_id: LegacyMessageType,
-        marker: Literal["acknowledged", "received", "displayed"],
-    ):
-        """
-        Send a message marker (:xep:`0333`) from this contact to the user.
+        if url:
+            legacy_msg_id = await self.send_file(url, e, **kwargs)
+        elif text:
+            legacy_msg_id = await self.send_text(text, e, **kwargs)
+        else:
+            log.debug("Ignoring %s", m)
+            return
 
-        NB: for the 'received' marker, this also sends a message receipt (:xep:`0184`)
+        if isinstance(e, LegacyMUC):
+            await e.echo(m, legacy_msg_id)
+            if legacy_msg_id is not None:
+                self.muc_sent_msg_ids[legacy_msg_id] = m.get_id()
+        else:
+            if legacy_msg_id is not None:
+                self.sent[legacy_msg_id] = m.get_id()
 
-        :param legacy_msg_id: ID of the message this marker refers to
-        :param marker: The marker type
+    async def __get_entity(self, m: Message) -> Union[LegacyContactType, LegacyMUCType]:
+        if m.get_type() == "groupchat":
+            muc = await self.bookmarks.by_jid(m.get_to())
+            if m.get_from().resource not in muc.user_resources:
+                raise XMPPError("not-acceptable", "You are not connected to this chat")
+            return muc
+        else:
+            return await self.contacts.by_jid(m.get_to())
 
+    @ignore_message_to_component
+    async def active_from_msg(self, m: Message):
         """
-        xmpp_id = self.session.sent.get(legacy_msg_id)
-        if xmpp_id is None:
-            log.debug("Cannot find the XMPP ID of this msg: %s", legacy_msg_id)
-        else:
-            if marker == "received":
-                receipt = self.xmpp.Message()
-                receipt["to"] = self.user.jid
-                receipt["receipt"] = xmpp_id
-                receipt["from"] = self.jid
-                receipt.send()
-            self.xmpp["xep_0333"].send_marker(
-                mto=self.user.jid,
-                id=xmpp_id,
-                marker=marker,
-                mfrom=self.jid,
-            )
+        Meant to be called from :class:`BaseGateway` only.
 
-    def ack(self, legacy_msg_id: LegacyMessageType):
+        :param m:
+        :return:
         """
-        Send an "acknowledged" message marker (:xep:`0333`) from this contact to the user.
+        await self.active(await self.__get_entity(m))
 
-        :param legacy_msg_id: The message this marker refers to
+    @ignore_message_to_component
+    async def inactive_from_msg(self, m: Message):
         """
-        self.__send_marker(legacy_msg_id, "acknowledged")
+        Meant to be called from :class:`BaseGateway` only.
 
-    def received(self, legacy_msg_id: LegacyMessageType):
+        :param m:
+        :return:
         """
-        Send a "received" message marker (:xep:`0333`) and a "message delivery receipt"
-        (:xep:`0184`)
-        from this contact to the user
+        await self.inactive(await self.__get_entity(m))
 
-        :param legacy_msg_id: The message this marker refers to
+    @ignore_message_to_component
+    async def composing_from_msg(self, m: Message):
         """
-        self.__send_marker(legacy_msg_id, "received")
+        Meant to be called from :class:`BaseGateway` only.
 
-    def displayed(self, legacy_msg_id: LegacyMessageType):
+        :param m:
+        :return:
         """
-        Send a "displayed" message marker (:xep:`0333`) from this contact to the user.
+        await self.composing(await self.__get_entity(m))
 
-        :param legacy_msg_id: The message this marker refers to
+    @ignore_message_to_component
+    async def paused_from_msg(self, m: Message):
         """
-        self.__send_marker(legacy_msg_id, "displayed")
+        Meant to be called from :class:`BaseGateway` only.
 
-    def __make_message(self, mtype="chat", **kwargs) -> Message:
-        m = self.xmpp.make_message(
-            mfrom=self.jid, mto=self.user.jid, mtype=mtype, **kwargs
-        )
-        m.enable("markable")
-        return m
+        :param m:
+        :return:
+        """
+        await self.paused(await self.__get_entity(m))
 
-    def __send_message(
-        self,
-        msg: Message,
-        legacy_msg_id: Optional[Any] = None,
-        when: Optional[datetime] = None,
-    ):
-        if legacy_msg_id is not None:
-            msg.set_id(self.session.legacy_msg_id_to_xmpp_msg_id(legacy_msg_id))
-        self._add_delay(msg, when)
-        msg.send()
+    def __xmpp_msg_id_to_legacy(self, xmpp_id: str):
+        sent = self.sent.inverse.get(xmpp_id)
+        if sent:
+            return sent
 
-    def __make_reply(self, msg: Message, reply_to_msg_id: Optional[LegacyMessageType]):
-        if reply_to_msg_id is None:
-            return
-        xmpp_id = self.session.sent.get(
-            reply_to_msg_id
-        ) or self.session.legacy_msg_id_to_xmpp_msg_id(reply_to_msg_id)
-        msg["reply"]["id"] = self.session.legacy_msg_id_to_xmpp_msg_id(xmpp_id)
-        # FIXME: https://xmpp.org/extensions/xep-0461.html#usecases mentions that a full JID must be used here
-        msg["reply"]["to"] = self.user.jid
+        try:
+            return self.xmpp_msg_id_to_legacy_msg_id(xmpp_id)
+        except Exception as e:
+            log.debug(
+                "Couldn't convert xmpp msg ID to legacy ID, ignoring: %r, %s",
+                e,
+                e.args,
+            )
 
-    def send_text(
-        self,
-        body: str = "",
-        *,
-        chat_state: Optional[str] = "active",
-        legacy_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        when: Optional[datetime] = None,
-    ) -> Message:
+    @ignore_message_to_component
+    @ignore_sent_carbons
+    async def displayed_from_msg(self, m: Message):
         """
-        Transmit a message from the contact to the user
-
-        :param body: Context of the message
-        :param chat_state: By default, will send an "active" chat state (:xep:`0085`) along with the
-            message. Set this to ``None`` if this is not desired.
-        :param legacy_msg_id: If you want to be able to transport read markers from the gateway
-            user to the legacy network, specify this
-        :param reply_to_msg_id:
-        :param when: when the message was sent, for a "delay" tag (:xep:`0203`)
-
-        :return: the XMPP message that was sent
-        """
-        msg = self.__make_message(mbody=body)
-        if self.CHAT_STATES and chat_state is not None:
-            msg["chat_state"] = chat_state
-        self.__make_reply(msg, reply_to_msg_id)
-        self.__send_message(msg, legacy_msg_id, when)
-        return msg
+        Meant to be called from :class:`BaseGateway` only.
 
-    async def send_file(
-        self,
-        filename: Union[Path, str],
-        content_type: Optional[str] = None,
-        input_file: Optional[IO[bytes]] = None,
-        url: Optional[str] = None,
-        *,
-        legacy_msg_id: Optional[LegacyMessageType] = None,
-        reply_to_msg_id: Optional[LegacyMessageType] = None,
-        when: Optional[datetime] = None,
-    ) -> Message:
+        :param m:
+        :return:
         """
-        Send a file using HTTP upload (:xep:`0363`)
-
-        :param filename: Filename to use or location on disk to the file to upload
-        :param content_type: MIME type, inferred from filename if not given
-        :param input_file: Optionally, a file like object instead of a file on disk.
-            filename will still be used to give the uploaded file a name
-        :param legacy_msg_id: If you want to be able to transport read markers from the gateway
-            user to the legacy network, specify this
-        :param url: Optionally, a URL of a file that slidge will download and upload to the
-            default file upload service on the xmpp server it's running on. url and input_file
-            are mutually exclusive.
-        :param reply_to_msg_id:
-        :param when: when the file was sent, for a "delay" tag (:xep:`0203`)
-
-        :return: The msg stanza that was sent
-        """
-        msg = self.__make_message()
-        self.__make_reply(msg, reply_to_msg_id)
-        if url is not None:
-            if input_file is not None:
-                raise TypeError("Either a URL or a file-like object")
-            async with aiohttp.ClientSession() as session:
-                async with session.get(url) as r:
-                    input_file = BytesIO(await r.read())
-        try:
-            uploaded_url = await self.xmpp["xep_0363"].upload_file(
-                filename=filename,
-                content_type=content_type,
-                input_file=input_file,
-                ifrom=self.xmpp.upload_requester,
-            )
-        except FileUploadError as e:
-            log.warning(
-                "Something is wrong with the upload service, see the traceback below"
-            )
-            log.exception(e)
-            if url is not None:
-                uploaded_url = url
+        e = await self.__get_entity(m)
+        displayed_msg_id = m["displayed"]["id"]
+        if not isinstance(e, LegacyMUC) and self.xmpp.MARK_ALL_MESSAGES:
+            to_mark = e.get_msg_xmpp_id_up_to(displayed_msg_id)  # type: ignore
+            if to_mark is None:
+                log.debug("Can't mark all messages up to %s", displayed_msg_id)
+                to_mark = [displayed_msg_id]
+        else:
+            to_mark = [displayed_msg_id]
+        for xmpp_id in to_mark:
+            if legacy := self.__xmpp_msg_id_to_legacy(xmpp_id):
+                await self.displayed(legacy, e)
+                if isinstance(e, LegacyMUC):
+                    await e.echo(m, None)
             else:
-                msg["body"] = (
-                    "I tried to send a file, but something went wrong. "
-                    "Tell your XMPP admin to check slidge logs."
-                )
-                self.__send_message(msg, legacy_msg_id, when)
-                return msg
-
-        msg["oob"]["url"] = uploaded_url
-        msg["body"] = uploaded_url
-        self.__send_message(msg, legacy_msg_id, when)
-        return msg
+                log.debug("Ignored displayed marker for msg: %r", xmpp_id)
 
-    def __privileged_send(self, msg: Message, when: Optional[datetime] = None):
-        msg.set_from(self.user.jid.bare)
-        msg.enable("store")
+    @ignore_message_to_component
+    @ignore_sent_carbons
+    async def correct_from_msg(self, m: Message):
+        e = await self.__get_entity(m)
+        xmpp_id = m["replace"]["id"]
+        if isinstance(e, LegacyMUC):
+            legacy_id = self.muc_sent_msg_ids.inverse.get(xmpp_id)
+        else:
+            legacy_id = self.__xmpp_msg_id_to_legacy(xmpp_id)
 
-        self._add_delay(msg, when)
+        if legacy_id is None:
+            log.debug("Did not find legacy ID to correct")
+            new_legacy_msg_id = await self.send_text(m["body"], e)
+        else:
+            new_legacy_msg_id = await self.correct(m["body"], legacy_id, e)
+        if isinstance(e, LegacyMUC):
+            if new_legacy_msg_id is not None:
+                self.muc_sent_msg_ids[new_legacy_msg_id] = m.get_id()
+            await e.echo(m, new_legacy_msg_id)
+        else:
+            if new_legacy_msg_id is not None:
+                self.sent[new_legacy_msg_id] = m.get_id()
 
-        self.session.ignore_messages.add(msg.get_id())
-        try:
-            self.xmpp["xep_0356"].send_privileged_message(msg)
-        except PermissionError:
-            try:
-                self.xmpp["xep_0356_old"].send_privileged_message(msg)
-            except PermissionError:
-                log.warning(
-                    "Slidge does not have privileges to send message on behalf of user."
-                    "Refer to https://slidge.readthedocs.io/en/latest/admin/xmpp_server.html "
-                    "for more info."
+    @ignore_message_to_component
+    @ignore_sent_carbons
+    async def react_from_msg(self, m: Message):
+        e = await self.__get_entity(m)
+        react_to: str = m["reactions"]["id"]
+        legacy_id = self.__xmpp_msg_id_to_legacy(react_to)
+
+        if not legacy_id:
+            log.debug("Ignored reaction from user")
+            raise XMPPError("internal-server-error")
+
+        emojis = [
+            remove_emoji_variation_selector_16(r["value"]) for r in m["reactions"]
+        ]
+        error_msg = None
+
+        if e.REACTIONS_SINGLE_EMOJI and len(emojis) > 1:
+            error_msg = "Maximum 1 emoji/message"
+
+        if not error_msg and (subset := await e.available_emojis(legacy_id)):
+            log.debug("%s %s %s", set(emojis), subset, set(emojis).issubset(subset))
+            if not set(emojis).issubset(subset):
+                error_msg = (
+                    f"You can only react with the following emojis: {''.join(subset)}"
                 )
-                return
-        return msg.get_id()
 
-    def carbon(
+        if error_msg:
+            self.send_gateway_message(error_msg)
+            if not isinstance(e, LegacyMUC):
+                # no need to carbon for groups, we just don't echo the stanza
+                e.react(legacy_id, carbon=True)  # type: ignore
+            await self.react(legacy_id, [], e)
+            raise XMPPError("not-acceptable", text=error_msg)
+
+        await self.react(legacy_id, emojis, e)
+        if isinstance(e, LegacyMUC):
+            await e.echo(m, None)
+
+    @ignore_message_to_component
+    @ignore_sent_carbons
+    async def retract_from_msg(self, m: Message):
+        e = await self.__get_entity(m)
+        xmpp_id: str = m["apply_to"]["id"]
+        legacy_id = self.__xmpp_msg_id_to_legacy(xmpp_id)
+        if legacy_id:
+            await self.retract(legacy_id, e)
+            if isinstance(e, LegacyMUC):
+                await e.echo(m, None)
+        else:
+            log.debug("Ignored retraction from user")
+
+    async def join_groupchat(self, p: Presence):
+        if not self.xmpp.GROUPS:
+            raise XMPPError(
+                "not-implemented", "This gateway does not implement multi-user chats."
+            )
+        muc = await self.bookmarks.by_jid(p.get_to())
+        log.debug("BOOKMARKS: %r", self.bookmarks.__class__)
+        log.debug("JOIN MUC: %r -- %r -- %r", muc, muc.join, muc.__class__)
+        await muc.join(p)
+
+    def send_gateway_status(
         self,
-        body: str,
-        legacy_id: Optional[Any] = None,
-        when: Optional[datetime] = None,
+        status: Optional[str] = None,
+        show=Optional[PresenceShow],
+        **kwargs,
     ):
         """
-        Call this when the user sends a message to a legacy network contact.
+        Send a presence from the gateway to the user.
 
-        This synchronizes the outgoing message history on the XMPP side, using
-        :xep:`0356` to impersonate the XMPP user and send a message from the user to
-        the contact. Thw XMPP server should in turn send carbons (:xep:`0280`) to online
-        XMPP clients +/- write the message in server-side archives (:xep:`0313`),
-        depending on the user's and the server's archiving policy.
-
-        :param body: Body of the message.
-        :param legacy_id: Legacy message ID
-        :param when: When was this message sent.
-        """
-        # we use Message() directly because we need xmlns="jabber:client"
-        msg = Message()
-        msg["to"] = self.jid.bare
-        msg["type"] = "chat"
-        msg["body"] = body
-        if legacy_id:
-            xmpp_id = self.session.legacy_msg_id_to_xmpp_msg_id(legacy_id)
-            msg.set_id(xmpp_id)
-            self.session.sent[legacy_id] = xmpp_id
+        Can be used to indicate the user session status, ie "SMS code required", "connected", …
 
-        return self.__privileged_send(msg, when)
+        :param status: A status message
+        :param show: Presence stanza 'show' element. I suggest using "dnd" to show
+            that the gateway is not fully functional
+        """
+        self.xmpp.send_presence(
+            pto=self.user.bare_jid, pstatus=status, pshow=show, **kwargs
+        )
 
-    def carbon_read(self, legacy_msg_id: Any, when: Optional[datetime] = None):
+    def send_gateway_message(self, text, **msg_kwargs):
         """
-        Synchronize user read state from official clients.
+        Send a message from the gateway component to the user.
 
-        :param legacy_msg_id:
-        :param when:
+        Can be used to indicate the user session status, ie "SMS code required", "connected", …
+
+        :param text: A text
         """
-        # we use Message() directly because we need xmlns="jabber:client"
-        msg = Message()
-        msg["to"] = self.jid.bare
-        msg["type"] = "chat"
-        msg["displayed"]["id"] = self.session.legacy_msg_id_to_xmpp_msg_id(
-            legacy_msg_id
+        self.xmpp.send_message(
+            mto=self.user.jid, mbody=text, mfrom=self.xmpp.boundjid, **msg_kwargs
         )
 
-        return self.__privileged_send(msg, when)
+    async def input(self, text: str, **msg_kwargs):
+        """
+        Request user input via direct messages.
 
-    def carbon_correct(
-        self,
-        legacy_msg_id: LegacyMessageType,
-        text: str,
-        when: Optional[datetime] = None,
-    ):
+        Wraps call to :meth:`.BaseSession.input`
+
+        :param text: The prompt to send to the user
+        :param msg_kwargs: Extra attributes
+        :return:
         """
-        Call this when the user corrects their own (last) message from an official client
+        return await self.xmpp.input(self.user.jid, text, **msg_kwargs)
 
-        :param legacy_msg_id:
-        :param text: The new body of the message
-        :param when:
+    async def send_qr(self, text: str):
         """
-        if (xmpp_id := self.session.sent.get(legacy_msg_id)) is None:
-            log.debug(
-                "Cannot find XMPP ID of msg '%s' corrected from the official client",
-                legacy_msg_id,
-            )
-            return
-        msg = Message()
-        msg.set_to(self.jid.bare)
-        msg.set_type("chat")
-        msg["replace"]["id"] = xmpp_id
-        msg["body"] = text
-        return self.__privileged_send(msg, when)
+        Sends a QR code generated from 'text' via HTTP Upload and send the URL to
+        ``self.user``
 
-    def carbon_react(
-        self,
-        legacy_msg_id: LegacyMessageType,
-        reactions: Iterable[str] = (),
-        when: Optional[datetime] = None,
-    ):
+        :param text: Text to encode as a QR code
         """
-        Call this to modify the user's own reactions (:xep:`0444`) about a message.
+        await self.xmpp.send_qr(text, mto=self.user.jid)
 
-        Can be called when the user reacts from the official client, or to modify a user's
-        reaction when the legacy network has constraints about acceptable reactions.
+    async def login(self) -> Optional[str]:
+        """
+        Login the gateway user to the legacy network.
 
-        :param legacy_msg_id: Legacy message ID this refers to
-        :param reactions: iterable of emojis
-        :param when:
-        """
-        if xmpp_id := self.session.sent.inverse.get(str(legacy_msg_id)):
-            log.debug("This is a reaction to a carbon message")
-            xmpp_id = str(xmpp_id)
-        elif xmpp_id := self.session.sent.get(legacy_msg_id):
-            log.debug("This is a reaction to the user's own message")
-        else:
-            log.debug(
-                "Cannot determine which message this reaction refers to, attempting msg ID conversion"
-            )
-            xmpp_id = self.session.legacy_msg_id_to_xmpp_msg_id(legacy_msg_id)
-        msg = Message()
-        msg["to"] = self.jid.bare
-        msg["type"] = "chat"
-        self.xmpp["xep_0444"].set_reactions(msg, to_id=xmpp_id, reactions=reactions)
-        return self.__privileged_send(msg, when)
+        Triggered when the gateway start and on user registration.
+        It is recommended that this function returns once the user is logged in,
+        so if you need to await forever (for instance to listen to incoming events),
+        it's a good idea to wrap your listener in an asyncio.Task.
 
-    def carbon_retract(
-        self, legacy_msg_id: LegacyMessageType, when: Optional[datetime] = None
-    ):
+        :return: Optionally, a text to use as the gateway status, e.g., "Connected as 'dude@legacy.network'"
         """
-        Call this when the user calls retracts (:xep:`0424`) a message from an official client
+        raise NotImplementedError
 
-        :param legacy_msg_id:
-        :param when:
-        :return:
+    async def logout(self):
+        """
+        Logout the gateway user from the legacy network.
+
+        Called on user unregistration and gateway shutdown.
         """
-        if (xmpp_id := self.session.sent.inverse.get(str(legacy_msg_id))) is None:
-            if (xmpp_id := self.session.sent.get(legacy_msg_id)) is None:
-                log.debug("Cannot find XMPP ID of retracted msg: %s", legacy_msg_id)
-                return
+        raise NotImplementedError
 
-        msg = Message()
-        msg.set_to(self.jid.bare)
-        msg.set_type("chat")
-        msg["apply_to"]["id"] = xmpp_id
-        msg["apply_to"].enable("retract")
-        return self.__privileged_send(msg, when)
+    def re_login(self):
+        """
+        Logout then re-login
 
-    def correct(self, legacy_msg_id: Any, new_text: str):
+        No reason to override this
         """
-        Call this when a legacy contact has modified his last message content.
+        self.xmpp.re_login(self)
 
-        Uses last message correction (:xep:`0308`)
+    async def send_text(
+        self,
+        text: str,
+        chat: Chat,
+        *,
+        reply_to_msg_id: Optional[LegacyMessageType] = None,
+        reply_to_fallback_text: Optional[str] = None,
+        reply_to: Optional[Union["LegacyContactType", "LegacyParticipantType"]] = None,
+    ) -> Optional[LegacyMessageType]:
+        """
+        Triggered when the user sends a text message from XMPP to a bridged entity, e.g.
+        to ``translated_user_name@slidge.example.com``, or ``translated_group_name@slidge.example.com``
+
+        Override this and implement sending a message to the legacy network in this method.
+
+        :param text: Content of the message
+        :param chat: Recipient of the message. :class:`.LegacyContact` instance for 1:1 chat,
+            :class:`.MUC` instance for groups.
+        :param reply_to_msg_id: A legacy message ID if the message references (quotes)
+            another message (:xep:`0461`)
+        :param reply_to_fallback_text: Content of the quoted text. Not necessarily set
+            by XMPP clients
+        :param reply_to: Author of the quoted message. :class:`LegacyContact` instance for
+            1:1 chat, :class:`LegacyParticipant` instance for groups.
 
-        :param legacy_msg_id: Legacy message ID this correction refers to
-        :param new_text: The new text
+        :return: An ID of some sort that can be used later to ack and mark the message
+            as read by the user
         """
-        msg = self.__make_message()
-        msg["replace"]["id"] = self.session.legacy_msg_id_to_xmpp_msg_id(legacy_msg_id)
-        msg["body"] = new_text
-        self.__send_message(msg)
+        raise NotImplementedError
 
-    def react(self, legacy_msg_id: LegacyMessageType, emojis: Iterable[str] = ()):
+    async def send_file(
+        self,
+        url: str,
+        chat: Chat,
+        *,
+        reply_to_msg_id: Optional[LegacyMessageType] = None,
+        reply_to_fallback_text: Optional[str] = None,
+        reply_to: Optional[Union[LegacyContactType, "LegacyParticipantType"]] = None,
+    ) -> Optional[LegacyMessageType]:
         """
-        Call this when a legacy contact reacts to a message
+        Triggered when the user has sends a file using HTTP Upload (:xep:`0363`)
 
-        :param legacy_msg_id: The message which the reaction refers to.
-        :param emojis: A iterable of emojis used as reactions
-        :return:
+        :param url: URL of the file
+        :param chat: See :meth:`.BaseSession.send_text`
+        :param reply_to_msg_id: See :meth:`.BaseSession.send_text`
+        :param reply_to_fallback_text: See :meth:`.BaseSession.send_text`
+        :param reply_to: See :meth:`.BaseSession.send_text`
+
+        :return: An ID of some sort that can be used later to ack and mark the message
+            as read by the user
         """
-        if (xmpp_id := self.session.sent.get(legacy_msg_id)) is None:
-            log.debug(
-                "Cannot determine which message this reaction refers to, attempting msg ID conversion"
-            )
-            xmpp_id = self.session.legacy_msg_id_to_xmpp_msg_id(legacy_msg_id)
-        msg = self.__make_message()
-        self.xmpp["xep_0444"].set_reactions(
-            msg,
-            to_id=xmpp_id,
-            reactions=emojis,
-        )
-        self.__send_message(msg)
-        return msg
+        raise NotImplementedError
 
-    def retract(self, legacy_msg_id: LegacyMessageType):
+    async def active(self, c: Chat):
         """
-        Call this when a legacy contact retracts (:XEP:`0424`) a message
+        Triggered when the user sends an 'active' chat state to the legacy network (:xep:`0085`)
 
-        :param legacy_msg_id: Legacy ID of the message to delete
+        :param c: Recipient of the active chat state
         """
-        self.xmpp["xep_0424"].send_retraction(
-            mto=self.user.jid,
-            mfrom=self.jid,
-            include_fallback=True,
-            fallback_text="I have deleted the message %s, but your XMPP client does not support that"
-            % legacy_msg_id,  # https://github.com/movim/movim/issues/1074
-            id=self.session.legacy_msg_id_to_xmpp_msg_id(legacy_msg_id),
-        )
+        raise NotImplementedError
 
-    def _add_delay(self, msg: Message, when: Optional[datetime] = None):
-        if not when:
-            return
-        if when.tzinfo is None:
-            when = when.astimezone(timezone.utc)
-        if (
-            datetime.now().astimezone(timezone.utc) - when
-            > self.xmpp.ignore_delay_threshold
-        ):
-            msg["delay"].set_stamp(when)
+    async def inactive(self, c: Chat):
+        """
+        Triggered when the user sends an 'inactive' chat state to the legacy network (:xep:`0085`)
 
+        :param c:
+        """
+        raise NotImplementedError
 
-LegacyContactType = TypeVar("LegacyContactType", bound=LegacyContact)
+    async def composing(self, c: Chat):
+        """
+        Triggered when the user starts typing in the window of a legacy contact (:xep:`0085`)
 
+        :param c:
+        """
+        raise NotImplementedError
 
-class LegacyRoster(Generic[LegacyContactType, SessionType], metaclass=SubclassableOnce):
-    """
-    Virtual roster of a gateway user, that allows to represent all
-    of their contacts as singleton instances (if used properly and not too bugged).
+    async def paused(self, c: Chat):
+        """
+        Triggered when the user pauses typing in the window of a legacy contact (:xep:`0085`)
 
-    Every :class:`.BaseSession` instance will have its own :class:`.LegacyRoster` instance
-    accessible via the :attr:`.BaseSession.contacts` attribute.
+        :param c:
+        """
+        raise NotImplementedError
 
-    Typically, you will mostly use the :meth:`.LegacyRoster.by_legacy_id` function to
-    retrieve a contact instance.
+    async def displayed(self, legacy_msg_id: LegacyMessageType, c: Chat):
+        """
+        Triggered when the user reads a message sent by a legacy contact.  (:xep:`0333`)
 
-    You might need to override :meth:`.LegacyRoster.legacy_id_to_jid_username` and/or
-    :meth:`.LegacyRoster.jid_username_to_legacy_id` to incorporate some custom logic
-    if you need some characters when translation JID user parts and legacy IDs.
-    """
+        This is only possible if a valid ``legacy_msg_id`` was passed when transmitting a message
+        from a contact to the user in :meth:`.LegacyContact.sent_text` or :meth:`slidge.LegacyContact.send_file`.
 
-    def __init__(self, session: "SessionType"):
-        self._contact_cls: Type[
-            LegacyContactType
-        ] = LegacyContact.get_self_or_unique_subclass()
-        self._contact_cls.xmpp = session.xmpp
-
-        self.session = session
-        self._contacts_by_bare_jid: dict[str, LegacyContactType] = {}
-        self._contacts_by_legacy_id: dict[LegacyContactIdType, LegacyContactType] = {}
-
-    def __iter__(self):
-        return iter(self._contacts_by_legacy_id.values())
-
-    def by_jid(self, contact_jid: JID) -> LegacyContactType:
-        """
-        Retrieve a contact by their JID
-
-        If the contact was not instantiated before, it will be created
-        using :meth:`slidge.LegacyRoster.jid_username_to_legacy_id` to infer their
-        legacy user ID.
-
-        :param contact_jid:
-        :return:
-        """
-        bare = contact_jid.bare
-        c = self._contacts_by_bare_jid.get(bare)
-        if c is None:
-            jid_username = str(contact_jid.username)
-            log.debug("Contact %s not found", contact_jid)
-            c = self._contact_cls(
-                self.session,
-                self.jid_username_to_legacy_id(jid_username),
-                jid_username,
-            )
-            self._contacts_by_legacy_id[c.legacy_id] = self._contacts_by_bare_jid[
-                bare
-            ] = c
-        return c
+        :param legacy_msg_id: Identifier of the message, passed to :meth:`slidge.LegacyContact.send_text`
+            or :meth:`slidge.LegacyContact.send_file`
+        :param c:
+        """
+        raise NotImplementedError
 
-    def by_legacy_id(self, legacy_id: Any) -> LegacyContactType:
+    async def correct(
+        self, text: str, legacy_msg_id: LegacyMessageType, c: Chat
+    ) -> Optional[LegacyMessageType]:
         """
-        Retrieve a contact by their legacy_id
+        Triggered when the user corrected a message using :xep:`0308`
 
-        If the contact was not instantiated before, it will be created
-        using :meth:`slidge.LegacyRoster.legacy_id_to_jid_username` to infer their
-        legacy user ID.
+        This is only possible if a valid ``legacy_msg_id`` was passed when transmitting a message
+        from a contact to the user in :meth:`.LegacyContact.send_text` or :meth:`slidge.LegacyContact.send_file`.
 
-        :param legacy_id:
-        :return:
+        :param text:
+        :param legacy_msg_id:
+        :param c:
         """
-        c = self._contacts_by_legacy_id.get(legacy_id)
-        if c is None:
-            log.debug("Contact %s not found in roster", legacy_id)
-            c = self._contact_cls(
-                self.session, legacy_id, self.legacy_id_to_jid_username(legacy_id)
-            )
-            self._contacts_by_bare_jid[c.jid.bare] = self._contacts_by_legacy_id[
-                legacy_id
-            ] = c
-        return c
+        raise NotImplementedError
 
-    def by_stanza(self, s) -> LegacyContactType:
+    async def search(self, form_values: dict[str, str]) -> Optional["SearchResult"]:
         """
-        Retrieve a contact by the destination of a stanza
+        Triggered when the user uses Jabber Search (:xep:`0055`) on the component
 
-        See :meth:`slidge.Roster.by_legacy_id` for more info.
+        Form values is a dict in which keys are defined in :attr:`.BaseGateway.SEARCH_FIELDS`
 
-        :param s:
+        :param form_values: search query, defined for a specific plugin by overriding
+            in :attr:`.BaseGateway.SEARCH_FIELDS`
         :return:
         """
-        return self.by_jid(s.get_to())
+        raise NotImplementedError
 
-    @staticmethod
-    def legacy_id_to_jid_username(legacy_id: Any) -> str:
+    async def react(self, legacy_msg_id: LegacyMessageType, emojis: list[str], c: Chat):
         """
-        Convert a legacy ID to a valid 'user' part of a JID
+        Triggered when the user sends message reactions (:xep:`0444`).
 
-        Should be overridden for cases where the str conversion of
-        the legacy_id is not enough, e.g., if it contains forbidden character.
-
-        :param legacy_id:
+        :param legacy_msg_id: ID of the message the user reacts to
+        :param emojis: Unicode characters representing reactions to the message ``legacy_msg_id``.
+            An empty string means "no reaction", ie, remove all reactions if any were present before
+        :param c: Contact or MUC the reaction refers to
         """
-        return str(legacy_id)
+        raise NotImplementedError
 
-    @staticmethod
-    def jid_username_to_legacy_id(jid_username: str) -> LegacyUserIdType:
+    async def retract(self, legacy_msg_id: LegacyMessageType, c: Chat):
         """
-        Convert a JID user part to a legacy ID.
-
-        Should be overridden in case legacy IDs are not strings, or more generally
-        for any case where the username part of a JID is not enough to identify
-        a contact on the legacy network.
+        Triggered when the user retracts (:xep:`0424`) a message.
 
-        Default implementation is an identity operation
-
-        :param jid_username: User part of a JID, ie "user" in "user@example.com"
-        :return: An identifier for the user on the legacy network.
+        :param legacy_msg_id: Legacy ID of the retracted message
+        :param c: The contact this retraction refers to
         """
-        return jid_username  # type:ignore
+        raise NotImplementedError
+
 
+def remove_emoji_variation_selector_16(emoji: str):
+    # this is required for compatibility with dino, and maybe other future clients?
+    return bytes(emoji, encoding="utf-8").replace(b"\xef\xb8\x8f", b"").decode()
 
-LegacyRosterType = TypeVar("LegacyRosterType", bound=LegacyRoster)
 
+_sessions: dict[GatewayUser, BaseSession] = {}
 log = logging.getLogger(__name__)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `slidge-0.1.0b2/slidge/core/gateway.py` & `slidge-0.1.0rc1/slidge/core/gateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 This module extends slixmpp.ComponentXMPP to make writing new LegacyClients easier
 """
 import asyncio
 import logging
 import re
 import tempfile
 from asyncio import Future
-from datetime import timedelta
-from pathlib import Path
-from typing import Any, Generic, Iterable, Optional, Sequence, Type, TypeVar
+from typing import Callable, Generic, Iterable, Optional, Sequence, Type
 
 import qrcode
-from slixmpp import JID, ComponentXMPP, Iq, Message
+from slixmpp import JID, ComponentXMPP, CoroutineCallback, Iq, Message, StanzaPath
 from slixmpp.exceptions import IqError, IqTimeout, XMPPError
+from slixmpp.plugins.xep_0363 import FileUploadError
 from slixmpp.types import MessageTypes
 
 from ..util import ABCSubclassableOnceAtMost, FormField
 from ..util.db import GatewayUser, RosterBackend, user_store
 from ..util.types import AvatarType
 from ..util.xep_0292.vcard4 import VCard4Provider
-from ..util.xep_0363 import FileUploadError
+from . import config
+from .adhoc import AdhocProvider, RegistrationType
+from .chat_command import ChatCommandProvider
+from .disco import Disco
 from .pubsub import PubSubComponent
 from .session import BaseSession, SessionType
 
 
 class BaseGateway(
     Generic[SessionType], ComponentXMPP, metaclass=ABCSubclassableOnceAtMost
 ):
@@ -59,14 +61,23 @@
     `extended <https://xmpp.org/extensions/xep-0077.html#extensibility>`_ by :xep:`0004`.
     """
     REGISTRATION_INSTRUCTIONS: str = "Enter your credentials"
     """
     The text presented to a user that wants to register (or modify) their legacy account
     configuration.
     """
+    REGISTRATION_TYPE = RegistrationType.SINGLE_STEP_FORM
+    """
+    SINGLE_STEP_FORM: 1 step, 1 form, compatible with :xep:`0077` (in-band registration)
+    
+    QRCODE: The registration requires flashing a QR code in an official client.
+    See :meth:`.BaseGateway.`
+    
+    TWO_FACTOR_CODE: The registration requires confirming login with a 2FA code
+    """
 
     COMPONENT_NAME: str = NotImplemented
     """Name of the component, as seen in service discovery by XMPP clients"""
     COMPONENT_TYPE: Optional[str] = ""
     """Type of the gateway, should ideally follow https://xmpp.org/registrar/disco-categories.html"""
     COMPONENT_AVATAR: Optional[AvatarType] = None
     """
@@ -86,117 +97,188 @@
     """
     Fields used for searching items via the component, through :xep:`0055` (jabber search).
     A common use case is to allow users to search for legacy contacts by something else than
     their usernames, eg their phone number.
     
     Plugins should implement search by overriding :meth:`.BaseSession.search`, effectively
     restricting search to registered users by default.
+    
+    If there is only one field, it can also be used via the ``jabber:iq:gateway`` protocol
+    described in :xep:`0100`. Limitation: this only works if the search request returns
+    one result item, and if this item has a 'jid' var.
     """
     SEARCH_TITLE: str = "Search for legacy contacts"
     """
     Title of the search form.
     """
     SEARCH_INSTRUCTIONS: str = ""
     """
     Instructions of the search form.
     """
 
     _BASE_CHAT_COMMANDS = {
         "find": "_chat_command_search",
         "help": "_chat_command_help",
         "register": "_chat_command_register",
+        "unregister": "_chat_command_unregister",
         "contacts": "_chat_command_list_contacts",
+        "groups": "_chat_command_list_groups",
     }
     CHAT_COMMANDS: dict[str, str] = {}
     """
     Keys of this dict can be used to trigger a command by a simple chat message to the gateway
     component. Extra words after the key are passed as *args to the handler. Values of the dict
     are strings, and handlers are resolved using ``getattr()`` on the :class:`.BaseGateway`
     instance.
     
     Handlers are coroutines with following signature:
     
-    .. code-block::python
+    .. code-block:: python
     
         async def _chat_command_xxx(*args, msg: Message, session: Optional[Session] = None)
             ...
     
     The original :class:`slixmpp.stanza.Message` is also passed to the handler as the
     msg kwarg. If the command comes from a registered gateway user, its session attribute is also
     passed to the handler.
+    
+    Refer to the :class:`slixmpp.plugins.xep_0050.XEP_0050` for more details on how to use ad-hoc
+    commands.
     """
 
     WELCOME_MESSAGE = (
         "Thank you for registering. Type 'help' to list the available commands, "
         "or just start messaging away!"
     )
     """
     A welcome message displayed to users on registration.
     This is useful notably for clients that don't consider component JIDs as a valid recipient in their UI,
     yet still open a functional chat window on incoming messages from components.
     """
 
-    def __init__(self, args):
-        """
+    MARK_ALL_MESSAGES = False
+    """
+    Set this to True for legacy networks that expects read marks for *all* messages and not just
+    the latest one that was read (as most XMPP clients will only send a reak mark for the latest msg).
+    """
 
-        :param args: CLI arguments parsed by :func:`.slidge.__main__.get_parser`
-        """
+    REGISTRATION_2FA_TITLE = "Enter your 2FA code"
+    REGISTRATION_2FA_INSTRUCTIONS = (
+        "You should have received something via email or SMS, or something"
+    )
+    REGISTRATION_QR_INSTRUCTIONS = "Flash this code or follow this link"
+
+    GROUPS = False
+
+    def __init__(self):
         super().__init__(
-            args.jid,
-            args.secret,
-            args.server,
-            args.port,
+            config.JID,
+            config.SECRET,
+            config.SERVER,
+            config.PORT,
             plugin_whitelist=SLIXMPP_PLUGINS,
             plugin_config={
                 "xep_0077": {
                     "form_fields": None,
                     "form_instructions": self.REGISTRATION_INSTRUCTIONS,
+                    "enable_subscription": self.REGISTRATION_TYPE
+                    == RegistrationType.SINGLE_STEP_FORM,
                 },
                 "xep_0100": {
                     "component_name": self.COMPONENT_NAME,
                     "user_store": user_store,
                     "type": self.COMPONENT_TYPE,
                 },
                 "xep_0184": {
                     "auto_ack": False,
                     "auto_request": True,
                 },
                 "xep_0363": {
-                    "upload_service": args.upload_service,
+                    "upload_service": config.UPLOAD_SERVICE,
                 },
             },
         )
         self.loop.set_exception_handler(self.__exception_handler)
         self.has_crashed = False
 
-        self.home_dir = Path(args.home_dir)
-        self._jid_validator = re.compile(args.user_jid_validator)
-        self._config = args
-        self.no_roster_push = args.no_roster_push
-        self.upload_requester = args.upload_requester or self.boundjid.bare
-        self.ignore_delay_threshold = timedelta(seconds=args.ignore_delay_threshold)
+        self.jid_validator = re.compile(config.USER_JID_VALIDATOR)
 
-        self._session_cls: Type[SessionType] = BaseSession.get_unique_subclass()
-        self._session_cls.xmpp = self
+        self.session_cls: Type[SessionType] = BaseSession.get_unique_subclass()
+        self.session_cls.xmpp = self
 
-        self._get_session_from_stanza = self._session_cls.from_stanza
-        self._get_session_from_user = self._session_cls.from_user
+        self.get_session_from_stanza = self.session_cls.from_stanza
+        self.get_session_from_user = self.session_cls.from_user
         self.register_plugins()
         self.__register_slixmpp_api()
         self.__register_handlers()
         self._input_futures: dict[str, Future] = {}
 
-        self._chat_commands = {
-            k: getattr(self, v)
-            for k, v in (self._BASE_CHAT_COMMANDS | self.CHAT_COMMANDS).items()
-        }
-
         self.register_plugin("pubsub", {"component_name": self.COMPONENT_NAME})
         self.pubsub: PubSubComponent = self["pubsub"]
         self.vcard: VCard4Provider = self["xep_0292_provider"]
+        if self.GROUPS:
+            self.plugin["xep_0030"].add_feature("http://jabber.org/protocol/muc")
+            self.plugin["xep_0030"].add_identity(
+                category="conference",
+                name="Slidged rooms",
+                itype="text",
+                jid=self.boundjid,
+            )
+
+        self.adhoc = AdhocProvider(self)
+        self.add_adhoc_commands()
+
+        self.disco = Disco(self)
+
+        self.chat_commands = chat = ChatCommandProvider(self)
+        self._chat_commands: dict[str, Callable] = {
+            k: getattr(self, v, None) or getattr(chat, v)
+            for k, v in (self._BASE_CHAT_COMMANDS | self.CHAT_COMMANDS).items()
+        }
+
+        self.use_origin_id = False
+
+        self.remove_handler("Ping")
+        self.register_handler(
+            CoroutineCallback(
+                "Ping",
+                StanzaPath("iq@type=get/ping"),
+                self.__handle_ping,  # type:ignore
+            )
+        )
+
+        self.qr_pending_registrations = dict[str, asyncio.Future[bool]]()
+
+    async def __handle_ping(self, iq: Iq):
+        ito = iq.get_to()
+
+        if ito == self.boundjid.bare:
+            iq.reply().send()
+
+        ifrom = iq.get_from()
+        user = user_store.get_by_jid(ifrom)
+        if user is None:
+            raise XMPPError("registration-required")
+
+        session = self.get_session_from_user(user)
+
+        try:
+            muc = await session.bookmarks.by_jid(ito)
+        except XMPPError:
+            pass
+        else:
+            muc.handle_ping(iq)
+            return
+
+        try:
+            await session.contacts.by_jid(ito)
+        except XMPPError:
+            pass
+        else:
+            iq.reply().send()
 
     def __exception_handler(self, loop: asyncio.AbstractEventLoop, context):
         """
         Called when a task created by loop.create_task() raises an Exception
 
         :param loop:
         :param context:
@@ -209,21 +291,28 @@
         elif isinstance(exc, SystemExit):
             log.debug("SystemExit called in an asyncio task")
         else:
             log.exception("Crash in an asyncio task: %s", context)
             self.has_crashed = True
             loop.stop()
 
+    def _raise_if_not_allowed_jid(self, jid: JID):
+        if not self.jid_validator.match(jid.bare):
+            raise XMPPError(
+                condition="not-allowed",
+                text="Your account is not allowed to use this gateway.",
+            )
+
     def exception(self, exception: Exception):
         """
         Called when a task created by slixmpp's internal (eg, on slix events) raises an Exception.
 
         Stop the event loop and exit on unhandled exception.
 
-        The default :class:slixmpp.basexmpp.BaseXMPP` behaviour is just to
+        The default :class:`slixmpp.basexmpp.BaseXMPP` behaviour is just to
         log the exception, but we want to avoid undefined behaviour.
 
         :param exception: An unhandled :class:`Exception` object.
         """
         if isinstance(exception, IqError):
             iq = exception.iq
             log.error("%s: %s", iq["error"]["condition"], iq["error"]["text"])
@@ -247,188 +336,170 @@
             "user_get",
         )
         self["xep_0077"].api.register(
             user_store.remove,
             "user_remove",
         )
         self["xep_0077"].api.register(
-            self._make_registration_form,
-            "make_registration_form",
+            self.make_registration_form, "make_registration_form"
         )
         self["xep_0077"].api.register(self._user_validate, "user_validate")
         self["xep_0077"].api.register(self._user_modify, "user_modify")
 
-        self["xep_0055"].api.register(self._search_get_form, "search_get_form")
+        self["xep_0055"].api.register(self.search_get_form, "search_get_form")
         self["xep_0055"].api.register(self._search_query, "search_query")
 
         self.roster.set_backend(RosterBackend)
 
     def __register_handlers(self):
         self.add_event_handler("session_start", self.__on_session_start)
         self.add_event_handler("disconnected", self.connect)
         self.add_event_handler("gateway_message", self._on_gateway_message_private)
         self.add_event_handler("user_register", self._on_user_register)
         self.add_event_handler("user_unregister", self._on_user_unregister)
-        get_session = self._get_session_from_stanza
+        get_session = self.get_session_from_stanza
 
         # fmt: off
         async def msg(m): await get_session(m).send_from_msg(m)
         async def disp(m): await get_session(m).displayed_from_msg(m)
         async def active(m): await get_session(m).active_from_msg(m)
         async def inactive(m): await get_session(m).inactive_from_msg(m)
         async def composing(m): await get_session(m).composing_from_msg(m)
         async def paused(m): await get_session(m).paused_from_msg(m)
         async def correct(m): await get_session(m).correct_from_msg(m)
         async def react(m): await get_session(m).react_from_msg(m)
         async def retract(m): await get_session(m).retract_from_msg(m)
+        async def groupchat_join(p): await get_session(p).join_groupchat(p)
         # fmt: on
 
         self.add_event_handler("legacy_message", msg)
         self.add_event_handler("marker_displayed", disp)
         self.add_event_handler("chatstate_active", active)
         self.add_event_handler("chatstate_inactive", inactive)
         self.add_event_handler("chatstate_composing", composing)
         self.add_event_handler("chatstate_paused", paused)
         self.add_event_handler("message_correction", correct)
         self.add_event_handler("reactions", react)
         self.add_event_handler("message_retract", retract)
 
+        self.add_event_handler("groupchat_join", groupchat_join)
+        self.add_event_handler("groupchat_message", msg)
+
+        self.register_handler(
+            CoroutineCallback(
+                f"muc#admin",
+                StanzaPath(f"iq/mucadmin_query"),
+                self._handle_admin,  # type: ignore
+            )
+        )
+
+        self.plugin["xep_0030"].add_feature("jabber:iq:gateway")
+        self.register_handler(
+            CoroutineCallback(
+                f"iq:gateway",
+                StanzaPath(f"iq/gateway"),
+                self._handle_gateway_iq,  # type: ignore
+            )
+        )
+
+    async def _handle_admin(self, iq: Iq):
+        log.debug("MUC ADMIN request %s", iq)
+        raise XMPPError("not-authorized")
+
+    async def _handle_gateway_iq(self, iq: Iq):
+        user = user_store.get_by_jid(iq.get_from())
+        if user is None:
+            raise XMPPError("not-authorized", "Register to the gateway first")
+
+        if len(self.SEARCH_FIELDS) > 1:
+            raise XMPPError("not-implemented", "Use jabber search for this gateway")
+
+        field = self.SEARCH_FIELDS[0]
+
+        reply = iq.reply()
+        if iq["type"] == "get":
+            reply["gateway"]["desc"] = self.SEARCH_TITLE
+            reply["gateway"]["prompt"] = field.label
+        elif iq["type"] == "set":
+            prompt = iq["gateway"]["prompt"]
+            session = self.session_cls.from_user(user)
+            result = await session.search({field.var: prompt})
+            if result is None or not result.items:
+                raise XMPPError(
+                    "item-not-found", "No contact was found with the info you provided."
+                )
+            if len(result.items) > 1:
+                raise XMPPError(
+                    "bad-request", "Your search yielded more than one result."
+                )
+            reply["gateway"]["jid"] = result.items[0]["jid"]
+
+        reply.send()
+
     async def __on_session_start(self, event):
         log.debug("Gateway session start: %s", event)
 
         # prevents XMPP clients from considering the gateway as an HTTP upload
         disco = self.plugin["xep_0030"]
-        await disco.del_feature(
-            feature="urn:xmpp:http:upload:0", jid=self.boundjid.bare
-        )
-        await self.plugin["xep_0115"].update_caps(jid=self.boundjid.bare)
+        await disco.del_feature(feature="urn:xmpp:http:upload:0", jid=self.boundjid)
+        await self.plugin["xep_0115"].update_caps(jid=self.boundjid)
 
-        self.__add_adhoc_commands()
-        self.add_adhoc_commands()
         await self.pubsub.set_avatar(
             jid=self.boundjid.bare, avatar=self.COMPONENT_AVATAR
         )
 
         for user in user_store.get_all():
             # TODO: before this, we should check if the user has removed us from their roster
             #       while we were offline and trigger unregister from there. Presence probe does not seem
             #       to work in this case, there must be another way. privileged entity could be used
             #       as last resort.
             await self["xep_0100"].add_component_to_roster(user.jid)
             self.send_presence(
                 pto=user.bare_jid, ptype="probe"
             )  # ensure we get all resources for user
-            session = self._session_cls.from_user(user)
+            session = self.session_cls.from_user(user)
             self.loop.create_task(self._login_wrap(session))
-            for c in session.contacts:
-                # we need to receive presences directed at the contacts, in order to
-                # send pubsub events for their +notify features
-                self.send_presence(pfrom=c.jid, pto=user.bare_jid, ptype="probe")
 
         log.info("Slidge has successfully started")
 
-    @staticmethod
-    async def _login_wrap(session: "SessionType"):
+    async def _login_wrap(self, session: "SessionType"):
         session.send_gateway_status("Logging in…", show="dnd")
         try:
             status = await session.login()
         except Exception as e:
             log.warning(f"Login problem for %s: %r", session.user, e)
+            log.exception(e)
             session.send_gateway_status(f"Could not login: {e}", show="busy")
             session.send_gateway_message(
                 f"You are not connected to this gateway! "
                 f"Maybe this message will tell you why: {e}"
             )
         else:
             log.info(f"Login success for %s", session.user)
+            session.never_logged = False
             if status is None:
                 session.send_gateway_status("Logged in", show="chat")
             else:
                 session.send_gateway_status(status, show="chat")
+            for c in session.contacts:
+                # we need to receive presences directed at the contacts, in
+                # order to send pubsub events for their +notify features
+                self.send_presence(
+                    pfrom=c.jid, pto=session.user.bare_jid, ptype="probe"
+                )
 
     def re_login(self, session: "SessionType"):
         async def w():
             await session.logout()
             await self._login_wrap(session)
 
         self.loop.create_task(w())
 
-    def __add_adhoc_commands(self):
-        # TODO: this should only be advertised to admins
-        # Not a big deal since we need to check if 'from' is an admin in the handler
-        # anyway, BUT it would be nice if this simply does not show up in the list
-        # of available commands for regular users.
-        self["xep_0050"].add_command(
-            node="info", name="List registered users", handler=self._handle_info
-        )
-        self.plugin["xep_0050"].add_command(
-            node="search", name="Search for contacts", handler=self._handle_search
-        )
-
-    def _handle_info(self, iq: Iq, session: dict[str, Any]):
-        """
-        List registered users for admins
-        """
-        if iq.get_from().bare not in self._config.admins:
-            raise XMPPError("not-authorized")
-        form = self["xep_0004"].make_form("result", "Component info")
-        form.add_field(
-            ftype="jid-multi",
-            label="Users",
-            value=[u.bare_jid for u in user_store.get_all()],
-        )
-
-        session["payload"] = form
-        session["has_next"] = False
-
-        return session
-
-    async def _handle_search(self, iq: Iq, adhoc_session: dict[str, Any]):
-        """
-        Jabber search, but as an adhoc command (search form)
-        """
-        user = user_store.get_by_jid(iq.get_from())
-        if user is None:
-            raise XMPPError(
-                "not-authorized", text="Search is only allowed for registered users"
-            )
-
-        session = self._get_session_from_stanza(iq)
-
-        reply = await self._search_get_form(None, None, ifrom=iq.get_from(), iq=iq)
-        adhoc_session["payload"] = reply["search"]["form"]
-        adhoc_session["next"] = self._handle_search2
-        adhoc_session["has_next"] = True
-        adhoc_session["session"] = session
-
-        return adhoc_session
-
-    async def _handle_search2(self, form, adhoc_session: dict[str, Any]):
-        """
-        Jabber search, but as an adhoc command (results)
-        """
-
-        search_results = await adhoc_session["session"].search(form.get_values())
-
-        form = self.plugin["xep_0004"].make_form("result", "Contact search results")
-        for field in search_results.fields:
-            form.add_reported(field.var, label=field.label, type=field.type)
-        for item in search_results.items:
-            form.add_item(item)
-
-        adhoc_session["next"] = None
-        adhoc_session["has_next"] = False
-        adhoc_session["payload"] = form
-
-        return adhoc_session
-
-    async def _make_registration_form(self, _jid, _node, _ifrom, iq: Iq):
-        if not self._jid_validator.match(iq.get_from().bare):
-            raise XMPPError(condition="not-allowed")
-
+    async def make_registration_form(self, _jid, _node, _ifrom, iq: Iq):
+        self._raise_if_not_allowed_jid(iq.get_from())
         reg = iq["register"]
         user = user_store.get_by_stanza(iq)
         log.debug("User found: %s", user)
 
         form = reg["form"]
         form.add_field(
             "FORM_TYPE",
@@ -468,70 +539,65 @@
                 value=field.value if user is None else user.get(field.var, field.value),
             )
 
         reply = iq.reply()
         reply.set_payload(reg)
         return reply
 
-    async def _user_prevalidate(self, ifrom: JID, form_dict: dict[str, Optional[str]]):
+    async def user_prevalidate(self, ifrom: JID, form_dict: dict[str, Optional[str]]):
         """
         Pre validate a registration form using the content of self.REGISTRATION_FIELDS
         before passing it to the plugin custom validation logic.
         """
         for field in self.REGISTRATION_FIELDS:
             if field.required and not form_dict.get(field.var):
                 raise ValueError(f"Missing field: '{field.label}'")
 
         await self.validate(ifrom, form_dict)
 
-    async def _user_validate(
-        self, _gateway_jid, _node, ifrom: JID, form_dict: dict[str, Optional[str]]
-    ):
+    async def _user_validate(self, _gateway_jid, _node, ifrom: JID, iq: Iq):
         """
         SliXMPP internal API stuff
         """
         log.debug("User validate: %s", ifrom.bare)
-        if not self._jid_validator.match(ifrom.bare):
-            raise XMPPError(condition="not-allowed")
-        await self._user_prevalidate(ifrom, form_dict)
+        form_dict = {f.var: iq.get(f.var) for f in self.REGISTRATION_FIELDS}
+        self._raise_if_not_allowed_jid(ifrom)
+        await self.user_prevalidate(ifrom, form_dict)
         log.info("New user: %s", ifrom.bare)
         user_store.add(ifrom, form_dict)
 
     async def _user_modify(
         self, _gateway_jid, _node, ifrom: JID, form_dict: dict[str, Optional[str]]
     ):
         """
         SliXMPP internal API stuff
         """
         user = user_store.get_by_jid(ifrom)
         log.debug("Modify user: %s", user)
-        await self._user_prevalidate(ifrom, form_dict)
+        await self.user_prevalidate(ifrom, form_dict)
         user_store.add(ifrom, form_dict)
 
     async def _on_user_register(self, iq: Iq):
-        session = self._get_session_from_stanza(iq)
-        for jid in self._config.admins:
+        session = self.get_session_from_stanza(iq)
+        for jid in config.ADMINS:
             self.send_message(
                 mto=jid,
                 mbody=f"{iq.get_from()} has registered",
                 mtype="headline",
                 mfrom=self.boundjid.bare,
             )
         session.send_gateway_message(self.WELCOME_MESSAGE)
-        await session.login()
+        await self._login_wrap(session)
 
     async def _on_user_unregister(self, iq: Iq):
-        # Mypy: "Type[SessionType?]" has no attribute "kill_by_jid"
-        # I don't understand why ^ this question mark...
-        kill = self._session_cls.kill_by_jid  # type: ignore
-        await kill(iq.get_from())
+        await self.session_cls.kill_by_jid(iq.get_from())
 
-    async def _search_get_form(self, _gateway_jid, _node, ifrom: JID, iq: Iq):
+    async def search_get_form(self, _gateway_jid, _node, ifrom: JID, iq: Iq):
         """
-        Prepare the search form using self.SEARCH_FIELDS
+        Prepare the search form using :attr:`.BaseSession.SEARCH_FIELDS`
         """
         user = user_store.get_by_jid(ifrom)
         if user is None:
             raise XMPPError(text="Search is only allowed for registered users")
 
         reply = iq.reply()
         form = reply["search"]["form"]
@@ -545,152 +611,37 @@
         """
         Handles a search request
         """
         user = user_store.get_by_jid(ifrom)
         if user is None:
             raise XMPPError(text="Search is only allowed for registered users")
 
-        result = await self._get_session_from_stanza(iq).search(
+        result = await self.get_session_from_stanza(iq).search(
             iq["search"]["form"].get_values()
         )
 
         if not result:
             raise XMPPError("item-not-found", text="Nothing was found")
 
         reply = iq.reply()
         form = reply["search"]["form"]
         for field in result.fields:
             form.add_reported(field.var, label=field.label, type=field.type)
         for item in result.items:
             form.add_item(item)
         return reply
 
-    async def _chat_command_search(
-        self, *args, msg: Message, session: Optional[SessionType] = None
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!")
-            return
-
-        search_form = {}
-        diff = len(args) - len(self.SEARCH_FIELDS)
-
-        if diff > 0:
-            session.send_gateway_message("Too many parameters!")
-            return
-
-        for field, arg in zip(self.SEARCH_FIELDS, args):
-            search_form[field.var] = arg
-
-        if diff < 0:
-            for field in self.SEARCH_FIELDS[diff:]:
-                if not field.required:
-                    continue
-                search_form[field.var] = await session.input(
-                    (field.label or field.var) + "?"
-                )
-
-        results = await session.search(search_form)
-        if results is None:
-            session.send_gateway_message("No results!")
-            return
-
-        result_fields = results.fields
-        for result in results.items:
-            text = ""
-            for f in result_fields:
-                if f.type == "jid-single":
-                    text += f"xmpp:{result[f.var]}\n"
-                else:
-                    text += f"{f.label}: {result[f.var]}\n"
-            session.send_gateway_message(text)
-
-    async def _chat_command_help(
-        self, *_args, msg: Message, session: Optional[SessionType]
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!").send()
-        else:
-            t = "|".join(
-                x
-                for x in self._chat_commands.keys()
-                if not x not in ("register", "help")
-            )
-            log.debug("In help: %s", t)
-            msg.reply(f"Available commands: {t}").send()
-
-    @staticmethod
-    async def _chat_command_list_contacts(
-        *_args, msg: Message, session: Optional[SessionType]
-    ):
-        if session is None:
-            msg.reply("Register to the gateway first!").send()
-        else:
-            contacts = sorted(
-                session.contacts, key=lambda c: c.name.casefold() if c.name else ""
-            )
-            t = "\n".join(f"{c.name}: xmpp:{c.jid.bare}" for c in contacts)
-            msg.reply(t).send()
-
-    async def _chat_command_register(
-        self, *args, msg: Message, session: Optional[SessionType]
-    ):
-        if session is not None:
-            msg.reply("You are already registered to this gateway").send()
-            return
-
-        jid = msg.get_from()
-
-        if not self._jid_validator.match(jid.bare):
-            msg.reply("You are not allowed to register to this gateway").send()
-            return
-
-        form: dict[str, Optional[str]] = {}
-        for field in self.REGISTRATION_FIELDS:
-            text = field.label or field.var
-            if field.value != "":
-                text += f" (default: '{field.value}')"
-            if not field.required:
-                text += " (optional, reply with '.' to skip)"
-            if (options := field.options) is not None:
-                for option in options:
-                    label = option["label"]
-                    value = option["value"]
-                    text += f"\n{label}: reply with '{value}'"
-
-            while True:
-                ans = await self.input(jid, text + "?")
-                if ans == "." and not field.required:
-                    form[field.var] = None
-                    break
-                else:
-                    if (options := field.options) is not None:
-                        valid_choices = [x["value"] for x in options]
-                        if ans not in valid_choices:
-                            continue
-                    form[field.var] = ans
-                    break
-
-        try:
-            await self.validate(jid, form)
-            await self["xep_0077"].api["user_validate"](None, None, jid, form)
-        except (ValueError, XMPPError) as e:
-            msg.reply(f"Something went wrong: {e}").send()
-        else:
-            self.event("user_register", msg)
-            msg.reply(f"Success!").send()
-
     def add_adhoc_commands(self):
         """
         Override this if you want to provide custom adhoc commands (:xep:`0050`)
         for your plugin, using :class:`slixmpp.plugins.xep_0050.XEP_0050`
 
         Basic example:
 
-        .. code-block:python
+        .. code-block:: python
 
             def add_adhoc_commands(self):
                 self["xep_0050"].add_command(
                     node="account_info",
                     name="Account Information",
                     handler=self.handle_account_info
                 )
@@ -711,46 +662,36 @@
                 adhoc_session["payload"] = form
                 adhoc_session["has_next"] = False
 
                 return session
         """
         pass
 
-    def config(self, argv: list[str]):
-        """
-        Override this to access CLI args to configure the slidge plugin
-
-        :param argv: CLI args that were not parsed by the slidge main entrypoint parser
-        :func:`slidge.__main__.get_parser`
-        """
-        pass
-
     async def validate(
         self, user_jid: JID, registration_form: dict[str, Optional[str]]
     ):
         """
         Validate a registration form from a user.
 
         Since :xep:`0077` is pretty limited in terms of validation, it is OK to validate
         anything that looks good here and continue the legacy auth process via direct messages
-        to the user (using :meth:`.BaseGateway.input` for instance)
+        to the user (using :meth:`.BaseGateway.input` for instance).
 
         :param user_jid: JID of the user that has just registered
         :param registration_form: A dict where keys are the :attr:`.FormField.var` attributes
          of the :attr:`.BaseGateway.REGISTRATION_FIELDS` iterable
         """
         pass
 
     async def unregister(self, user: GatewayUser):
         """
         Optionally override this if you need to clean additional
         stuff after a user has been removed from the permanent user_store.
 
         :param user:
-        :return:
         """
         pass
 
     async def _on_gateway_message_private(self, msg: Message):
         """
         Called when an XMPP user (not necessarily registered as a gateway user) sends a direct message to
         the gateway.
@@ -765,15 +706,15 @@
             text = msg["body"]
             command, *rest = text.split(" ")
 
             user = user_store.get_by_stanza(msg)
             if user is None:
                 session = None
             else:
-                session = self._get_session_from_user(user)
+                session = self.get_session_from_user(user)
 
             handler = self._chat_commands.get(command)
             if handler is None:
                 await self.on_gateway_message(msg, session=session)
             else:
                 log.debug("Chat command handler: %s", handler)
                 await handler(*rest, msg=msg, session=session)
@@ -802,15 +743,15 @@
 
     async def input(
         self, jid: JID, text=None, mtype: MessageTypes = "chat", **msg_kwargs
     ) -> str:
         """
         Request arbitrary user input using a simple chat message, and await the result.
 
-        You shouldn't need to call directly bust instead user :meth:`.BaseSession.input`
+        You shouldn't need to call directly bust instead use :meth:`.BaseSession.input`
         to directly target a user.
 
         NB: When using this, the next message that the user sent to the component will
         not be transmitted to :meth:`.BaseGateway.on_gateway_message`, but rather intercepted.
         Await the coroutine to get its content.
 
         :param jid: The JID we want input from
@@ -836,15 +777,15 @@
         :param msg_kwargs:
         :return:
         """
         msg = self.make_message(**msg_kwargs)
         msg.set_from(self.boundjid.bare)
         try:
             url = await self["xep_0363"].upload_file(
-                filename=filename, ifrom=self.upload_requester
+                filename=filename, ifrom=config.UPLOAD_REQUESTER
             )
         except FileUploadError as e:
             log.warning(
                 "Something is wrong with the upload service, see the traceback below"
             )
             log.exception(e)
             msg["body"] = (
@@ -876,38 +817,80 @@
 
         Sends offline presences from all contacts of all user sessions and from
         the gateway component itself.
         No need to call this manually, :func:`slidge.__main__.main` should take care of it.
         """
         log.debug("Shutting down")
         for user in user_store.get_all():
-            session = self._session_cls.from_jid(user.jid)
-            for c in session.contacts:
-                c.offline()
-            self.loop.create_task(session.logout())
+            self.session_cls.from_jid(user.jid).shutdown()
             self.send_presence(ptype="unavailable", pto=user.jid)
 
+    async def validate_two_factor_code(self, user: GatewayUser, code: str):
+        """
+        Called when the user enters their 2FA code.
 
-GatewayType = TypeVar("GatewayType", bound=BaseGateway)
+        Should raise the appropriate ``XMPPError`` if the login fails
+
+        :param user: The gateway user whose registration is pending
+            Use their ``.bare_jid`` and/or``.registration_form`` attributes
+            to get what you need
+        :param code: The code they entered, either via "chatbot" message or
+            adhoc command
+        """
+        raise NotImplementedError
+
+    async def get_qr_text(self, user: GatewayUser) -> str:
+        """
+        Plugins should call this to complete registration with QR codes
+
+        :param user: The not-yet-fully-registered GatewayUser.
+            Use its ``.bare_jid`` and/or``.registration_form`` attributes
+            to get what you need
+        """
+        raise NotImplementedError
+
+    async def confirm_qr(
+        self, user_bare_jid: str, exception: Optional[Exception] = None
+    ):
+        """
+        Plugins should call this to complete registration with QR codes
+
+        :param user_bare_jid: The not-yet-fully-registered ``GatewayUser`` instance
+            Use their ``.bare_jid`` and/or``.registration_form`` attributes
+            to get what you need
+        :param exception: Optionally, an XMPPError to be raised to **not** confirm
+            QR code flashing.
+        """
+        fut = self.qr_pending_registrations[user_bare_jid]
+        if exception is None:
+            fut.set_result(True)
+        else:
+            fut.set_exception(exception)
 
 
 SLIXMPP_PLUGINS = [
+    "xep_0030",  # Service discovery
+    "xep_0045",  # Multi-User Chat
     "xep_0050",  # Adhoc commands
     "xep_0055",  # Jabber search
     "xep_0066",  # Out of Band Data
     "xep_0077",  # In-band registration
     "xep_0084",  # User Avatar
     "xep_0085",  # Chat state notifications
     "xep_0100",  # Gateway interaction
+    "xep_0106",  # JID Escaping
     "xep_0115",  # Entity capabilities
     "xep_0172",  # User nickname
     "xep_0184",  # Message Delivery Receipts
+    "xep_0199",  # XMPP Ping
+    "xep_0221",  # Data Forms Media Element
     "xep_0280",  # Carbons
     "xep_0292_provider",  # VCard4
     "xep_0308",  # Last message correction
+    "xep_0319",  # Last User Interaction in Presence
     "xep_0333",  # Chat markers
     "xep_0334",  # Message Processing Hints
     "xep_0356",  # Privileged Entity
     "xep_0356_old",  # Privileged Entity (old namespace)
     "xep_0363",  # HTTP file upload
     "xep_0424",  # Message retraction
     "xep_0444",  # Message reactions
```

### Comparing `slidge-0.1.0b2/slidge/core/pubsub.py` & `slidge-0.1.0rc1/slidge/core/pubsub.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 import asyncio
 import hashlib
 import io
 import logging
 from copy import copy
 from pathlib import Path
-from typing import Optional, TypeVar, Union
+from typing import Optional, Union
 
-import aiohttp
 from PIL import Image, UnidentifiedImageError
 from slixmpp import JID, ComponentXMPP, CoroutineCallback, Iq, Presence, StanzaPath
 from slixmpp.exceptions import XMPPError
 from slixmpp.plugins.base import BasePlugin, register_plugin
 from slixmpp.plugins.xep_0060.stanza import Event, EventItem, EventItems, Item
+from slixmpp.plugins.xep_0084 import Data as AvatarData
+from slixmpp.plugins.xep_0084 import MetaData as AvatarMetadata
 from slixmpp.plugins.xep_0172 import UserNick
 from slixmpp.types import JidStr, OptJidStr
 
-from slidge.util.db import user_store
-from slidge.util.types import AvatarType
-from slidge.util.xep_0084 import Data as AvatarData
-from slidge.util.xep_0084 import MetaData as AvatarMetadata
-from slidge.util.xep_0292.stanza import VCard4
+from ..util.db import user_store
+from ..util.types import AvatarType, PepItemType
+from ..util.xep_0292.stanza import VCard4
+from . import config
+from .cache import avatar_cache
 
 VCARD4_NAMESPACE = "urn:xmpp:vcard4"
 
 
 class PepItem:
     def __init__(self, authorized_jid: Optional[JidStr] = None):
         self.authorized_jid = authorized_jid
 
 
 class PepAvatar(PepItem):
-    AVATAR_SIZE: Optional[int] = None
-
     def __init__(self, authorized_jid: Optional[JidStr] = None):
         super().__init__(authorized_jid)
         self.metadata: Optional[AvatarMetadata] = None
         self.data: Optional[AvatarData] = None
         self.id: Optional[str] = None
 
     async def set_avatar(self, avatar: AvatarType):
-        if isinstance(avatar, bytes):
+        if isinstance(avatar, str):
+            return await self.set_avatar_from_url(avatar)
+        elif isinstance(avatar, bytes):
             img = Image.open(io.BytesIO(avatar))
         elif isinstance(avatar, Path):
             img = Image.open(avatar)
-        elif isinstance(avatar, str):
-            async with aiohttp.ClientSession() as session:
-                async with session.get(avatar) as response:
-                    img = Image.open(io.BytesIO(await response.read()))
         else:
             raise TypeError("Avatar must be bytes, a Path or a str (URL)", avatar)
 
         metadata = AvatarMetadata()
 
         resampled = False
-        if (size := self.AVATAR_SIZE) and any(x > size for x in img.size):
+        if (size := config.AVATAR_SIZE) and any(x > size for x in img.size):
             img.thumbnail((size, size))
             log.debug("Resampled image to %s", img.size)
             resampled = True
 
         if not resampled and img.format == "PNG" and isinstance(avatar, bytes):
             avatar_bytes = avatar
         elif not resampled and img.format == "PNG" and isinstance(avatar, Path):
@@ -79,29 +76,43 @@
         )
         self.metadata = metadata
 
         data = AvatarData()
         data.set_value(avatar_bytes)
         self.data = data
 
+    async def set_avatar_from_url(self, url: str):
+        avatar = await avatar_cache.get_avatar(url)
+        metadata = AvatarMetadata()
+        self.id = avatar.hash
+        metadata.add_info(
+            id=avatar.hash,
+            itype="image/png",
+            ibytes=len(avatar.data),
+            height=str(avatar.height),
+            width=str(avatar.width),
+        )
+        self.metadata = metadata
+
+        data = AvatarData()
+        data.set_value(avatar.data)
+        self.data = data
+
 
 class PepNick(PepItem):
     def __init__(
         self, authorized_jid: Optional[JidStr] = None, nick: Optional[str] = None
     ):
         super().__init__(authorized_jid)
         nickname = UserNick()
         if nick is not None:
             nickname["nick"] = nick
         self.nick = nickname
 
 
-PepItemType = TypeVar("PepItemType", bound=PepItem)
-
-
 class PubSubComponent(BasePlugin):
     xmpp: ComponentXMPP
 
     name = "pubsub"
     description = "Pubsub component"
     dependencies = {
         "xep_0030",
@@ -147,24 +158,22 @@
         disco.add_identity("account", "registered", self.component_name)
         disco.add_feature("http://jabber.org/protocol/pubsub#event")
         disco.add_feature("http://jabber.org/protocol/pubsub#retrieve-items")
         disco.add_feature("http://jabber.org/protocol/pubsub#persistent-items")
 
     async def _on_got_online(self, p: Presence):
         from_ = p.get_from()
-        # async with self.xmpp["xep_0115"].lock:
         ver_string = p["caps"]["ver"]
         info = None
         if ver_string:
             await asyncio.sleep(5)
             info = await self.xmpp.plugin["xep_0115"].get_caps(from_)
         if info is None:
             info = await self.xmpp.plugin["xep_0030"].get_info(from_)
         features = info["features"]
-        log.debug("features of %s: %s", from_, features)
         if AvatarMetadata.namespace + "+notify" in features:
             try:
                 pep_avatar = self._get_authorized_avatar(p)
             except XMPPError:
                 pass
             else:
                 self._broadcast(
@@ -203,19 +212,17 @@
         )
 
     @staticmethod
     def _get_authorized_item(
         store: dict[JID, PepItemType], stanza: Union[Iq, Presence]
     ) -> PepItemType:
         item = store.get(stanza.get_to())
-        log.debug("pep ava: %s", item)
         if item is None:
             raise XMPPError("item-not-found")
 
-        log.debug("auth: %s - %s", item.authorized_jid, stanza.get_from().bare)
         if item.authorized_jid is not None:
             if stanza.get_from().bare != item.authorized_jid:
                 raise XMPPError("item-not-found")
 
         return item
 
     def _get_authorized_avatar(self, stanza: Union[Iq, Presence]):
@@ -228,30 +235,28 @@
         pep_avatar = self._get_authorized_avatar(iq)
 
         requested_items = iq["pubsub"]["items"]
         if len(requested_items) == 0:
             self._reply_with_payload(iq, pep_avatar.data, pep_avatar.id)
         else:
             for item in requested_items:
-                log.debug("item id: %s", item["id"])
                 if item["id"] == pep_avatar.id:
                     self._reply_with_payload(iq, pep_avatar.data, pep_avatar.id)
                     return
             else:
                 raise XMPPError("item-not-found")
 
     async def _get_avatar_metadata(self, iq: Iq):
         pep_avatar = self._get_authorized_avatar(iq)
 
         requested_items = iq["pubsub"]["items"]
         if len(requested_items) == 0:
             self._reply_with_payload(iq, pep_avatar.metadata, pep_avatar.id)
         else:
             for item in requested_items:
-                log.debug("item id: %s", item["id"])
                 if item["id"] == pep_avatar.id:
                     self._reply_with_payload(iq, pep_avatar.metadata, pep_avatar.id)
                     return
             else:
                 raise XMPPError("item-not-found")
 
     async def _get_vcard(self, iq: Iq):
@@ -314,14 +319,15 @@
 
     async def set_avatar(
         self,
         jid: JidStr,
         avatar: Optional[AvatarType] = None,
         restrict_to: OptJidStr = None,
     ):
+        jid = JID(jid)
         if avatar is None:
             try:
                 del self._avatars[jid]
             except KeyError:
                 pass
             self._broadcast(AvatarMetadata(), jid, restrict_to)
         else:
@@ -345,14 +351,15 @@
 
     def set_nick(
         self,
         jid: JidStr,
         nick: Optional[str] = None,
         restrict_to: OptJidStr = None,
     ):
+        jid = JID(jid)
         nickname = PepNick(restrict_to, nick)
         self._nicks[jid] = nickname
         log.debug("NICK: %s", nickname.nick)
         self._broadcast(nickname.nick, jid, restrict_to)
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0b2/slidge/plugins/discord/__init__.py` & `slidge-0.1.0rc1/slidge/plugins/discord/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,58 @@
 import functools
 import logging
-from argparse import ArgumentParser
+from typing import Optional
 
 import discord as di
+from slixmpp import JID
 from slixmpp.exceptions import XMPPError
 
 from slidge import *
 
+from ...util import BiDict
 from .session import Session
 
 
+class Config:
+    DISCORD_VERBOSE = False
+    DISCORD_VERBOSE__DOC = (
+        "Let the discord lib at the same loglevel as others loggers. "
+        "By default, it's set it to WARNING because it's *really* verbose."
+    )
+
+
 class Gateway(BaseGateway[Session]):
     COMPONENT_NAME = "Discord (slidge)"
     COMPONENT_TYPE = "discord"
+    COMPONENT_AVATAR = "https://www.usff.fr/wp-content/uploads/2018/05/Discord_logo.png"
+
     REGISTRATION_INSTRUCTIONS = (
         "Have a look at https://discordpy-self.readthedocs.io/en/latest/token.html"
     )
-    REGISTRATION_FIELDS = [FormField("token", required=True)]
+    REGISTRATION_FIELDS = [FormField("token", label="Discord token", required=True)]
 
     ROSTER_GROUP = "Discord"
 
-    def config(self, argv: list[str]):
-        parser = ArgumentParser()
-        parser.add_argument("--discord-verbose", action="store_true")
-        args = parser.parse_args(argv)
-        if not args.discord_verbose:
+    def __init__(self):
+        super().__init__()
+        if not Config.DISCORD_VERBOSE:
             log.debug("Disabling discord info logs")
             logging.getLogger("discord.gateway").setLevel(logging.WARNING)
             logging.getLogger("discord.client").setLevel(logging.WARNING)
 
+    async def validate(
+        self, user_jid: JID, registration_form: dict[str, Optional[str]]
+    ):
+        try:
+            await di.Client().login(registration_form.get("token"))
+        except di.LoginFailure as e:
+            raise ValueError(str(e))
 
-class Contact(LegacyContact[Session]):
+
+class Contact(LegacyContact[Session, "str"]):
     MARKS = False
 
     @functools.cached_property
     def discord_user(self) -> di.User:
         logging.debug("Searching for user: %s", self.legacy_id)
         if (u := self.session.discord.get_user(self.legacy_id)) is None:
             raise XMPPError(
@@ -69,22 +87,35 @@
         else:
             self.set_vcard(full_name=name, note=profile.bio)
 
         # TODO: use the relationship here
         # relationship = u.relationship
 
 
-class Roster(LegacyRoster[Contact, "Session"]):
-    def by_discord_user(self, u: di.User):
-        return self.by_legacy_id(u.id)
+class Roster(LegacyRoster["Session", Contact, int]):
+    def __init__(self, *a, **k):
+        super().__init__(*a, **k)
+
+    async def by_discord_user(self, u: di.User):
+        return await self.by_legacy_id(u.id)
 
-    @staticmethod
-    def jid_username_to_legacy_id(discord_id: str):
+    async def jid_username_to_legacy_id(self, username: str):
         try:
-            return int(discord_id)
+            user_id = int(username)
         except ValueError:
             raise XMPPError(
-                "not-found", text=f"Not a valid discord user ID: {discord_id}"
+                "bad-request",
+                text=f"Not a valid discord ID: {username}",
             )
+        else:
+            if self.session.discord.get_user(user_id) is None:
+                raise XMPPError(
+                    "item-not-found",
+                    text=f"No discord user was found with ID: {username}",
+                )
+            return user_id
+
+    async def legacy_id_to_jid_username(self, discord_user_id: int) -> str:
+        return str(discord_user_id)
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0b2/slidge/plugins/discord/client.py` & `slidge-0.1.0rc1/slidge/plugins/discord/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,71 +23,82 @@
         if not isinstance(channel, di.DMChannel):
             return
 
         if (author := message.author) == self.user:
             async with self.session.send_lock:
                 fut = self.session.send_futures.get(message.id)
             if fut is None:
-                self.session.contacts.by_discord_user(channel.recipient).carbon(
-                    message.content
-                )
+                (
+                    await self.session.contacts.by_discord_user(channel.recipient)
+                ).send_text(message.content, carbon=True)
             else:
                 fut.set_result(True)
         else:
-            contact = self.session.contacts.by_discord_user(author)
+            contact = await self.session.contacts.by_discord_user(author)
             reply_to = message.reference.message_id if message.reference else None
-            if content := message.content:
+
+            text = message.content
+            attachments = message.attachments
+            msg_id = message.id
+
+            if not attachments:
                 contact.send_text(
-                    content,
-                    legacy_msg_id=message.id,
+                    text,
+                    legacy_msg_id=msg_id,
                     reply_to_msg_id=reply_to,
                 )
-            for attachment in message.attachments:
+                return
+
+            last_attachment_i = len(attachments := message.attachments) - 1
+            for i, attachment in enumerate(attachments):
+                last = i == last_attachment_i
                 await contact.send_file(
                     url=attachment.url,
                     filename=attachment.filename,
                     content_type=attachment.content_type,
-                    reply_to_msg_id=reply_to,
+                    reply_to_msg_id=reply_to if last else None,
+                    legacy_msg_id=msg_id if last else None,
+                    caption=text if last else None,
                 )
 
     async def on_typing(self, channel, user, _when):
         if user != self.user and isinstance(channel, di.DMChannel):
-            self.session.contacts.by_discord_user(user).composing()
+            (await self.session.contacts.by_discord_user(user)).composing()
 
     async def on_message_edit(self, before: di.Message, after: di.Message):
         if not isinstance(after.channel, di.DMChannel):
             return
         if before.content == after.content:
             return
         if (author := after.author) == self.user:
             fut = self.session.edit_futures.get(after.id)
             if fut is None:
-                self.session.contacts.by_discord_user(
-                    after.channel.recipient
-                ).carbon_correct(after.id, after.content)
+                (
+                    await self.session.contacts.by_discord_user(after.channel.recipient)
+                ).correct(after.id, after.content, carbon=True)
             else:
                 fut.set_result(True)
         else:
-            self.session.contacts.by_discord_user(author).correct(
+            (await self.session.contacts.by_discord_user(author)).correct(
                 after.id, after.content
             )
 
     async def on_message_delete(self, m: di.Message):
         if not isinstance(m.channel, di.DMChannel):
             return
         if (author := m.author) == self.user:
             fut = self.session.delete_futures.get(m.id)
             if fut is None:
-                self.session.contacts.by_discord_user(
-                    m.channel.recipient
-                ).carbon_retract(m.id)
+                (
+                    await self.session.contacts.by_discord_user(m.channel.recipient)
+                ).retract(m.id, carbon=True)
             else:
                 fut.set_result(True)
         else:
-            self.session.contacts.by_discord_user(author).retract(m.id)
+            (await self.session.contacts.by_discord_user(author)).retract(m.id)
 
     async def on_reaction_add(
         self, reaction: di.Reaction, user: Union[di.User, di.ClientUser]
     ):
         await self.update_reactions(reaction, user)
 
     async def on_reaction_remove(
@@ -99,10 +110,12 @@
         self, reaction: di.Reaction, user: Union[di.User, di.ClientUser]
     ):
         message: di.Message = reaction.message
         if not isinstance(message.channel, di.DMChannel):
             return
 
         if user == self.user:
-            self.session.update_reactions(message)
+            await self.session.update_reactions(message)
         else:
-            await self.session.contacts.by_discord_user(user).update_reactions(message)
+            await (await self.session.contacts.by_discord_user(user)).update_reactions(
+                message
+            )
```

### Comparing `slidge-0.1.0b2/slidge/plugins/discord/session.py` & `slidge-0.1.0rc1/slidge/plugins/discord/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,113 @@
 import asyncio
-from typing import TYPE_CHECKING, Any, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 import discord as di
 
 from slidge import *
 
+from ...util.types import Chat
+
 if TYPE_CHECKING:
     from . import Contact, Gateway, Roster
     from .client import Discord
 
 
-class Session(BaseSession["Contact", "Roster", "Gateway"]):
-    discord: "Discord"
-    ready_future: asyncio.Future[bool]
-    delete_futures: dict[int, asyncio.Future[bool]]
-    edit_futures: dict[int, asyncio.Future[bool]]
-    send_futures: dict[int, asyncio.Future[bool]]
-    send_lock: asyncio.Lock
-
-    def post_init(self):
+class Session(
+    BaseSession[
+        "Gateway",
+        int,
+        "Roster",
+        "Contact",
+        LegacyBookmarks,
+        LegacyMUC,
+        LegacyParticipant,
+    ]
+):
+    def __init__(self, user):
+        super().__init__(user)
         from .client import Discord
 
         self.discord = Discord(self)
-        self.ready_future = self.xmpp.loop.create_future()
-        self.delete_futures = {}
-        self.edit_futures = {}
-        self.send_futures = {}
+        self.ready_future: asyncio.Future[bool] = self.xmpp.loop.create_future()
+        self.delete_futures = dict[int, asyncio.Future[bool]]()
+        self.edit_futures = dict[int, asyncio.Future[bool]]()
+        self.send_futures = dict[int, asyncio.Future[bool]]()
         self.send_lock = asyncio.Lock()
 
     @staticmethod
-    def xmpp_msg_id_to_legacy_msg_id(i: str) -> Union[int, str]:
-        try:
-            return int(i)
-        except ValueError:
-            return i
+    def xmpp_msg_id_to_legacy_msg_id(i: str):
+        return int(i)
 
     async def login(self):
-        self.xmpp.loop.create_task(
-            self.discord.start(self.user.registration_form["token"])
-        )
+        await self.discord.login(self.user.registration_form["token"])
+        self.xmpp.loop.create_task(self.discord.connect())
+
         await self.ready_future
         for u in self.discord.users:
             if not isinstance(u, di.User):
                 self.log.debug(f"Skipping %s", u)
                 continue
             if not u.is_friend():
                 self.log.debug(f"%s is not a friend", u)
                 continue
-            c = self.contacts.by_legacy_id(u.id)
+            c = await self.contacts.by_legacy_id(u.id)
             await c.update_info()
             await c.add_to_roster()
             # TODO: contribute to discord.py-self so that the presence information
             #       of relationships is parsed. logs show:
             #       'PRESENCE_UPDATE referencing an unknown guild ID: %s. Discarding.'
             #       https://github.com/dolfies/discord.py-self/blob/master/discord/state.py#L1044
             c.online()
         return f"Logged on as {self.discord.user}"
 
-    async def send_text(self, t: str, c: "Contact", *, reply_to_msg_id=None):
+    async def send_text(
+        self,
+        text: str,
+        chat,
+        reply_to_msg_id=None,
+        reply_to_fallback_text: Optional[str] = None,
+        **kwargs,
+    ):
         async with self.send_lock:
             mid = (
-                await c.discord_user.send(
-                    t,
+                await chat.discord_user.send(
+                    text,
                     reference=None
                     if reply_to_msg_id is None
                     else di.MessageReference(
                         message_id=reply_to_msg_id,
-                        channel_id=c.direct_channel_id,
+                        channel_id=chat.direct_channel_id,
                     ),
                 )
             ).id
         f = self.send_futures[mid] = self.xmpp.loop.create_future()
         await f
         return mid
 
     async def logout(self):
         await self.discord.close()
 
-    async def send_file(self, u: str, c: "Contact", *, reply_to_msg_id=None):
+    async def send_file(self, url: str, chat: Chat, **kwargs):
         # discord clients inline previews of external URLs, so no need to actually send on discord servers
-        await c.discord_user.send(u)
+        await chat.discord_user.send(url)
 
     async def active(self, c: "Contact"):
         pass
 
     async def inactive(self, c: "Contact"):
         pass
 
     async def composing(self, c: "Contact"):
         await c.discord_user.trigger_typing()
 
     async def paused(self, c: "Contact"):
         pass
 
-    async def displayed(self, legacy_msg_id: str, c: "Contact"):
+    async def displayed(self, legacy_msg_id: int, c: "Contact"):
         if not isinstance(legacy_msg_id, int):
             self.log.debug("This is not a valid discord msg id: %s", legacy_msg_id)
             return
         u = c.discord_user
         channel: di.DMChannel = u.dm_channel
         if channel is None:
             return
@@ -140,23 +150,23 @@
         if channel is None:
             return
         m = await channel.fetch_message(legacy_msg_id)
         self.delete_futures[legacy_msg_id] = self.xmpp.loop.create_future()
         await m.delete()
         await self.delete_futures[legacy_msg_id]
 
-    def update_reactions(self, message: di.Message):
-        self.contacts.by_discord_user(message.channel.recipient).carbon_react(
-            message.id, self.get_my_legacy_reactions(message)
+    async def update_reactions(self, message: di.Message):
+        (await self.contacts.by_discord_user(message.channel.recipient)).react(
+            message.id, self.get_my_legacy_reactions(message), carbon=True
         )
 
     @staticmethod
     def get_my_legacy_reactions(message: di.Message) -> list[str]:
         reactions = []
         for r in message.reactions:
             if r.me and not r.custom_emoji:
                 reactions.append(r.emoji)
 
         return reactions
 
-    async def search(self, form_values: dict[str, str]) -> SearchResult:
+    async def search(self, form_values: dict[str, str]):
         pass
```

### Comparing `slidge-0.1.0b2/slidge/plugins/facebook.py` & `slidge-0.1.0rc1/slidge/plugins/facebook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,109 @@
 import asyncio
 import io
+import json
 import logging
 import random
 import shelve
+import zlib
 from collections import OrderedDict, defaultdict
 from dataclasses import dataclass
 from mimetypes import guess_type
-from pathlib import Path
 from typing import Optional, Union
 
 import aiohttp
 import maufbapi.types.graphql
 from maufbapi import AndroidAPI, AndroidMQTT, AndroidState
+from maufbapi.mqtt.subscription import RealtimeTopic
+from maufbapi.proxy import ProxyHandler
+from maufbapi.thrift import ThriftObject
 from maufbapi.types import mqtt as mqtt_t
 from maufbapi.types.graphql import Participant, ParticipantNode, Thread
 from maufbapi.types.graphql.responses import FriendshipStatus
+from slixmpp import JID
 from slixmpp.exceptions import XMPPError
 
 from slidge import *
+from slidge.core.adhoc import RegistrationType, TwoFactorNotRequired
+
+
+class Config:
+    CHATS_TO_FETCH = 20
+    CHATS_TO_FETCH__DOC = (
+        "The number of most recent chats to fetch on startup. "
+        "Getting all chats might hit rate limiting and possibly account lock. "
+        "Please report if you try with high values and don't hit any problem!"
+    )
 
 
 class Gateway(BaseGateway):
     REGISTRATION_INSTRUCTIONS = "Enter facebook credentials"
     REGISTRATION_FIELDS = [
         FormField(var="email", label="Email", required=True),
         FormField(var="password", label="Password", required=True, private=True),
     ]
+    REGISTRATION_MULTISTEP = True
+    REGISTRATION_TYPE = RegistrationType.TWO_FACTOR_CODE
 
     ROSTER_GROUP = "Facebook"
 
     COMPONENT_NAME = "Facebook (slidge)"
     COMPONENT_TYPE = "facebook"
     COMPONENT_AVATAR = "https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/Facebook_Messenger_logo_2018.svg/480px-Facebook_Messenger_logo_2018.svg.png"
 
     SEARCH_TITLE = "Search in your facebook friends"
     SEARCH_INSTRUCTIONS = "Enter something that can be used to search for one of your friends, eg, a first name"
     SEARCH_FIELDS = [FormField(var="query", label="Term(s)")]
 
+    def __init__(self):
+        super().__init__()
+        self._pending_reg = dict[str, AndroidAPI]()
+
+    async def validate(
+        self, user_jid: JID, registration_form: dict[str, Optional[str]]
+    ):
+        s = AndroidState()
+        x = ProxyHandler(None)
+        api = AndroidAPI(state=s, proxy_handler=x)
+        s.generate(random.randbytes(30))  # type: ignore
+        await api.mobile_config_sessionless()
+        try:
+            await api.login(
+                email=registration_form["email"], password=registration_form["password"]
+            )
+        except maufbapi.http.errors.TwoFactorRequired:
+            self._pending_reg[user_jid.bare] = api
+        except maufbapi.http.errors.OAuthException as e:
+            raise XMPPError("not-authorized", text=str(e))
+        else:
+            save_state(user_jid.bare, api.state)
+            raise TwoFactorNotRequired
+
+    async def validate_two_factor_code(self, user: GatewayUser, code):
+        api = self._pending_reg.pop(user.bare_jid)
+        try:
+            await api.login_2fa(email=user.registration_form["email"], code=code)
+        except maufbapi.http.errors as e:
+            raise XMPPError("not-authorized", text=str(e))
+        save_state(user.bare_jid, api.state)
+
+
+def get_shelf_path(user_bare_jid):
+    return str(global_config.HOME_DIR / user_bare_jid)
+
+
+def save_state(user_bare_jid: str, state: AndroidState):
+    shelf_path = get_shelf_path(user_bare_jid)
+    with shelve.open(shelf_path) as shelf:
+        shelf["state"] = state
+
 
-class Contact(LegacyContact["Session"]):
-    legacy_id: str  # facebook username, as in facebook.com/name.surname123
+class Contact(LegacyContact["Session", str]):
+    # legacy_id = facebook username, as in facebook.com/name.surname123
+    REACTIONS_SINGLE_EMOJI = True
 
     def __init__(self, *a, **k):
         super(Contact, self).__init__(*a, **k)
         self._fb_id: Optional[int] = None
 
     async def fb_id(self):
         if self._fb_id is None:
@@ -71,23 +131,18 @@
         if self.legacy_id != participant.messaging_actor.username:
             raise RuntimeError(
                 "Attempted to populate a contact with a non-corresponding participant"
             )
         self.name = participant.messaging_actor.name
         self._fb_id = int(participant.id)
         if self.avatar is None or update_avatar:
-            async with aiohttp.ClientSession() as session:
-                async with session.get(
-                    participant.messaging_actor.profile_pic_large.uri
-                ) as response:
-                    response.raise_for_status()
-                    self.avatar = await response.read()
+            self.avatar = participant.messaging_actor.profile_pic_large.uri
 
 
-class Roster(LegacyRoster[Contact, "Session"]):
+class Roster(LegacyRoster["Session", Contact, str]):
     def __init__(self, *a, **k):
         super().__init__(*a, **k)
         self.by_fb_id_dict: dict[int, Contact] = {}
 
     async def by_fb_id(self, fb_id: int) -> "Contact":
         contact = self.by_fb_id_dict.get(fb_id)
         if contact is None:
@@ -113,79 +168,50 @@
             if participant.id != self.session.me.id:
                 break
         else:
             raise RuntimeError(
                 "Couldn't find friend in thread participants", t.all_participants
             )
 
-        contact = self.by_legacy_id(participant.messaging_actor.username)
+        contact = await self.by_legacy_id(participant.messaging_actor.username)
         await contact.populate_from_participant(participant)
         self.by_fb_id_dict[int(participant.id)] = contact
         return contact
 
 
-class Session(BaseSession[Contact, Roster, Gateway]):
-    fb_state: AndroidState
-
-    shelf_path: Path
+class Session(
+    BaseSession[
+        Gateway, str, Roster, Contact, LegacyBookmarks, LegacyMUC, LegacyParticipant
+    ]
+):
     mqtt: AndroidMQTT
     api: AndroidAPI
-
     me: maufbapi.types.graphql.OwnInfo
 
-    sent_messages: defaultdict[int, "Messages"]
-    received_messages: defaultdict[int, "Messages"]
-    # keys = "contact ID"
-
-    ack_futures: dict[int, asyncio.Future["FacebookMessage"]]
-    # keys = "offline thread ID"
-    reaction_futures: dict[str, asyncio.Future[None]]
-    unsend_futures: dict[str, asyncio.Future[None]]
-    # keys = "facebook message id"
-
-    contacts: Roster
-
-    def post_init(self):
-        self.shelf_path = self.xmpp.home_dir / self.user.bare_jid
-        self.ack_futures = {}
-        self.reaction_futures: dict[str, asyncio.Future] = {}
-        self.unsend_futures: dict[str, asyncio.Future] = {}
-        self.sent_messages = defaultdict(Messages)
-        self.received_messages = defaultdict(Messages)
+    def __init__(self, user):
+        super().__init__(user)
+
+        # keys = "offline thread ID"
+        self.ack_futures = dict[int, asyncio.Future[FacebookMessage]]()
+
+        # keys = "facebook message id"
+        self.reaction_futures = dict[str, asyncio.Future]()
+        self.unsend_futures = dict[str, asyncio.Future]()
+
+        # keys = "contact ID"
+        self.sent_messages = defaultdict[int, Messages](Messages)
+        self.received_messages = defaultdict[int, Messages](Messages)
 
     async def login(self):
         shelf: shelve.Shelf[AndroidState]
-        with shelve.open(str(self.shelf_path)) as shelf:
-            try:
-                self.fb_state = s = shelf["state"]
-            except KeyError:
-                s = AndroidState()
-                self.api = api = AndroidAPI(state=s)
-                s.generate(random.randbytes(30))  # type: ignore
-                await api.mobile_config_sessionless()
-                try:
-                    login = await api.login(
-                        email=self.user.registration_form["email"],
-                        password=self.user.registration_form["password"],
-                    )
-                except maufbapi.http.errors.IncorrectPassword:
-                    self.send_gateway_message("Incorrect password")
-                    raise
-                except maufbapi.http.errors.TwoFactorRequired:
-                    code = await self.input(
-                        "Reply to this message with your 2 factor authentication code"
-                    )
-                    login = await api.login_2fa(
-                        email=self.user.registration_form["email"], code=code
-                    )
-                log.debug("Login output: %s", login)
-                self.fb_state = shelf["state"] = api.state
-            else:
-                self.api = api = AndroidAPI(state=s)
-        self.mqtt = AndroidMQTT(api.state)
+        with shelve.open(get_shelf_path(self.user.bare_jid)) as shelf:
+            s = shelf["state"]
+        x = ProxyHandler(None)
+        self.api = AndroidAPI(state=s, proxy_handler=x)
+        self.mqtt = AndroidMQTT(self.api.state, proxy_handler=self.api.proxy_handler)
         self.me = await self.api.get_self()
         self.me.id = int(self.me.id)  # bug in maufbapi?
         await self.add_friends()
         self.mqtt.seq_id_update_callback = lambda i: setattr(self.mqtt, "seq_id", i)
         self.mqtt.add_event_handler(mqtt_t.Message, self.on_fb_message)
         self.mqtt.add_event_handler(mqtt_t.ExtendedMessage, self.on_fb_message)
         self.mqtt.add_event_handler(mqtt_t.ReadReceipt, self.on_fb_message_read)
@@ -203,16 +229,18 @@
         self.mqtt.add_event_handler(mqtt_t.MessageSyncError, self.on_fb_event)
         self.mqtt.add_event_handler(mqtt_t.ForcedFetch, self.on_fb_event)
         # self.mqtt.add_event_handler(Connect, self.on_connect)
         # self.mqtt.add_event_handler(Disconnect, self.on_disconnect)
         self.xmpp.loop.create_task(self.mqtt.listen(self.mqtt.seq_id))
         return f"Connected as '{self.me.name} <{self.me.email}>'"
 
-    async def add_friends(self, n=2):
-        thread_list = await self.api.fetch_thread_list(msg_count=0, thread_count=n)
+    async def add_friends(self):
+        thread_list = await self.api.fetch_thread_list(
+            msg_count=0, thread_count=Config.CHATS_TO_FETCH
+        )
         self.mqtt.seq_id = int(thread_list.sync_sequence_id)
         self.log.debug("SEQ ID: %s", self.mqtt.seq_id)
         self.log.debug("Thread list: %s", thread_list)
         self.log.debug("Thread list page info: %s", thread_list.page_info)
         for t in thread_list.nodes:
             if t.is_group_thread:
                 log.debug("Skipping group: %s", t)
@@ -220,43 +248,45 @@
             c = await self.contacts.by_thread(t)
             await c.add_to_roster()
             c.online()
 
     async def logout(self):
         pass
 
-    async def send_text(self, t: str, c: Contact, *, reply_to_msg_id=None) -> str:
+    async def send_text(
+        self, text: str, chat: Contact, *, reply_to_msg_id=None, **kwargs
+    ) -> str:
         resp: mqtt_t.SendMessageResponse = await self.mqtt.send_message(
-            target=(fb_id := await c.fb_id()),
-            message=t,
+            target=(fb_id := await chat.fb_id()),
+            message=text,
             is_group=False,
             reply_to=reply_to_msg_id,
         )
         fut = self.ack_futures[
             resp.offline_threading_id
         ] = self.xmpp.loop.create_future()
         log.debug("Send message response: %s", resp)
         if not resp.success:
             raise XMPPError(resp.error_message)
         fb_msg = await fut
         self.sent_messages[fb_id].add(fb_msg)
         return fb_msg.mid
 
-    async def send_file(self, u: str, c: Contact, *, reply_to_msg_id=None):
+    async def send_file(self, url: str, chat: Contact, reply_to_msg_id=None, **kwargs):
         async with aiohttp.ClientSession() as s:
-            async with s.get(u) as r:
+            async with s.get(url) as r:
                 data = await r.read()
         oti = self.mqtt.generate_offline_threading_id()
         fut = self.ack_futures[oti] = self.xmpp.loop.create_future()
         resp = await self.api.send_media(
             data=data,
-            file_name=u.split("/")[-1],
-            mimetype=guess_type(u)[0] or "application/octet-stream",
+            file_name=url.split("/")[-1],
+            mimetype=guess_type(url)[0] or "application/octet-stream",
             offline_threading_id=oti,
-            chat_id=await c.fb_id(),
+            chat_id=await chat.fb_id(),
             is_group=False,
             reply_to=reply_to_msg_id,
         )
         ack = await fut
         log.debug("Upload ack: %s", ack)
         return resp.media_id
 
@@ -299,49 +329,63 @@
         log.debug("Facebook message: %s", evt)
         fb_msg = FacebookMessage(mid=meta.id, timestamp_ms=meta.timestamp)
         if meta.sender == self.me.id:
             try:
                 fut = self.ack_futures.pop(meta.offline_threading_id)
             except KeyError:
                 log.debug("Received carbon %s - %s", meta.id, msg.text)
-                contact.carbon(body=msg.text, legacy_id=meta.id)
+                contact.send_text(body=msg.text, legacy_id=meta.id, carbon=True)
                 log.debug("Sent carbon")
                 self.sent_messages[thread_key.other_user_id].add(fb_msg)
             else:
                 log.debug("Received echo of %s", meta.offline_threading_id)
                 fut.set_result(fb_msg)
         else:
-            if msg.text:
-                contact.send_text(
-                    msg.text, legacy_msg_id=meta.id, reply_to_msg_id=reply_to
-                )
-            if msg.attachments:
-                async with aiohttp.ClientSession() as c:
-                    for a in msg.attachments:
-                        try:
-                            url = (
-                                ((v := a.video_info) and v.download_url)
-                                or ((au := a.audio_info) and au.url)
-                                or a.image_info.uri_map.get(0)
-                            )
-                        except AttributeError:
-                            log.warning("Unhandled attachment: %s", a)
+            self.received_messages[thread_key.other_user_id].add(fb_msg)
+
+            text = msg.text
+            msg_id = meta.id
+            if not (attachments := msg.attachments):
+                if text:
+                    contact.send_text(
+                        text, legacy_msg_id=msg_id, reply_to_msg_id=reply_to
+                    )
+                return
+
+            last_attachment_i = len(attachments) - 1
+            async with aiohttp.ClientSession() as c:
+                for i, a in enumerate(attachments):
+                    last = i == last_attachment_i
+                    try:
+                        url = (
+                            ((v := a.video_info) and v.download_url)
+                            or ((au := a.audio_info) and au.url)
+                            or a.image_info.uri_map.get(0)
+                        )
+                    except AttributeError:
+                        log.warning("Unhandled attachment: %s", a)
+                        contact.send_text(
+                            "/me sent an attachment that slidge does not support"
+                        )
+                        continue
+                    if url is None:
+                        if last:
                             contact.send_text(
-                                "/me sent an attachment that slidge does not support"
+                                text, legacy_msg_id=msg_id, reply_to_msg_id=reply_to
                             )
-                            continue
-                        if url is None:
-                            continue
-                        async with c.get(url) as r:
-                            await contact.send_file(
-                                filename=a.file_name,
-                                content_type=a.mime_type,
-                                input_file=io.BytesIO(await r.read()),
-                            )
-            self.received_messages[thread_key.other_user_id].add(fb_msg)
+                        continue
+                    async with c.get(url) as r:
+                        await contact.send_file(
+                            filename=a.file_name,
+                            content_type=a.mime_type,
+                            input_file=io.BytesIO(await r.read()),
+                            caption=text if last else None,
+                            legacy_msg_id=msg_id if last else None,
+                            reply_to_msg_id=reply_to if last else None,
+                        )
 
     async def on_fb_message_read(self, receipt: mqtt_t.ReadReceipt):
         log.debug("Facebook read: %s", receipt)
         try:
             mid = self.sent_messages[receipt.user_id].pop_up_to(receipt.read_to).mid
         except KeyError:
             log.debug("Cannot find MID of %s", receipt.read_to)
@@ -363,27 +407,27 @@
         for thread in receipt.threads:
             c = await self.contacts.by_fb_id(thread.other_user_id)
             try:
                 mid = self.received_messages[await c.fb_id()].pop_up_to(when).mid
             except KeyError:
                 log.debug("Cannot find mid of %s", when)
                 continue
-            c.carbon_read(mid)
+            c.displayed(mid, carbon=True)
 
     async def on_fb_reaction(self, reaction: mqtt_t.Reaction):
         self.log.debug("Reaction: %s", reaction)
         if is_group_thread(tk := reaction.thread):
             return
         contact = await self.contacts.by_thread_key(tk)
         mid = reaction.message_id
         if reaction.reaction_sender_id == self.me.id:
             try:
                 f = self.reaction_futures.pop(mid)
             except KeyError:
-                contact.carbon_react(mid, reaction.reaction or "")
+                contact.react(mid, reaction.reaction or "", carbon=True)
             else:
                 f.set_result(None)
         else:
             contact.react(reaction.message_id, reaction.reaction or "")
 
     async def on_fb_unsend(self, unsend: mqtt_t.UnsendMessage):
         self.log.debug("Unsend: %s", unsend)
@@ -391,31 +435,30 @@
             return
         contact = await self.contacts.by_thread_key(tk)
         mid = unsend.message_id
         if unsend.user_id == self.me.id:
             try:
                 f = self.unsend_futures.pop(mid)
             except KeyError:
-                contact.carbon_retract(mid)
+                contact.retract(mid, carbon=True)
             else:
                 f.set_result(None)
         else:
             contact.retract(unsend.message_id)
 
     async def correct(self, text: str, legacy_msg_id: str, c: Contact):
         await self.api.unsend(legacy_msg_id)
         return await self.send_text(text, c)
 
     async def react(self, legacy_msg_id: str, emojis: list[str], c: Contact):
+        # only reaction per msg on facebook, but this is handled by slidge core
         if len(emojis) == 0:
             emoji = None
         else:
             emoji = emojis[-1]
-            if len(emojis) > 1:  # only reaction per msg on facebook
-                c.carbon_react(legacy_msg_id, emoji)
         f = self.reaction_futures[legacy_msg_id] = self.xmpp.loop.create_future()
         await self.api.react(legacy_msg_id, emoji)
         await f
 
     async def retract(self, legacy_msg_id: str, c: Contact):
         f = self.unsend_futures[legacy_msg_id] = self.xmpp.loop.create_future()
         await self.api.unsend(legacy_msg_id)
@@ -486,8 +529,63 @@
             raise KeyError(approx_t)
 
 
 def is_group_thread(t: mqtt_t.ThreadKey):
     return t.other_user_id is None and t.thread_fbid is not None
 
 
+# Monkeypatch
+# TODO: remove me when https://github.com/mautrix/facebook/pull/270 is merged
+# and a new maufbapi is released
+
+
+REQUEST_TIMEOUT = 60
+
+
+def publish(
+    self,
+    topic,
+    payload,
+    prefix: bytes = b"",
+    compress: bool = True,
+) -> asyncio.Future:
+    if isinstance(payload, dict):
+        payload = json.dumps(payload)
+    if isinstance(payload, str):
+        payload = payload.encode("utf-8")
+    if isinstance(payload, ThriftObject):
+        payload = payload.to_thrift()
+    if compress:
+        payload = zlib.compress(prefix + payload, level=9)
+    elif prefix:
+        payload = prefix + payload
+    info = self._client.publish(
+        topic.encoded if isinstance(topic, RealtimeTopic) else topic, payload, qos=1
+    )
+    fut = self._loop.create_future()
+    timeout_handle = self._loop.call_later(REQUEST_TIMEOUT, self._cancel_later, fut)
+    fut.add_done_callback(lambda _: timeout_handle.cancel())
+    self._publish_waiters[info.mid] = fut
+    return fut
+
+
+async def request(
+    self,
+    topic: RealtimeTopic,
+    response: RealtimeTopic,
+    payload,
+    prefix: bytes = b"",
+):
+    async with self._response_waiter_locks[response]:
+        fut = self._loop.create_future()
+        self._response_waiters[response] = fut
+        await self.publish(topic, payload, prefix)
+        timeout_handle = self._loop.call_later(REQUEST_TIMEOUT, self._cancel_later, fut)
+        fut.add_done_callback(lambda _: timeout_handle.cancel())
+        return await fut
+
+
+AndroidMQTT.publish = publish
+AndroidMQTT.request = request
+
+
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0b2/slidge/plugins/hackernews.py` & `slidge-0.1.0rc1/slidge/plugins/hackernews.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,25 +47,22 @@
         ) as session:
             async with session.get(LOGIN_URL, allow_redirects=False) as r:
                 log.debug("Login response: %s - %s", r.status, await r.text())
                 if r.status != 302:
                     raise ValueError("Cookie does not seem valid")
 
 
-class Session(BaseSession[LegacyContact, LegacyRoster, Gateway]):
-    http_session: aiohttp.ClientSession
-    highest_handled_submission_id: int
-    hn_username: str
-
-    def post_init(self):
+class Session(BaseSession):
+    def __init__(self, user):
+        super().__init__(user)
         self.http_session = aiohttp.ClientSession(
-            cookies={"user": self.user.registration_form["cookie"]}
+            cookies={"user": self.user.registration_form["cookie"]}  # type: ignore
         )
         self.highest_handled_submission_id = 0
-        self.hn_username = self.user.registration_form["cookie"].split("&")[0]
+        self.hn_username = self.user.registration_form["cookie"].split("&")[0]  # type: ignore
 
     async def login(self):
         kid_ids: list[int] = []
         for submission_id in await self.get_user_submissions():
             user_submission = await self.get_item(submission_id)
             for kid_id in user_submission.get("kids", []):
                 kid_ids.append(kid_id)
@@ -103,33 +100,32 @@
         ) as r:
             if r.status != 200:
                 log.warning("Bad response from API: %s", r)
                 raise RuntimeError
             return (await r.json())["submitted"]
 
     async def send_own_and_reply(self, user_submission, reply_id):
-        contact: LegacyContact = self.contacts.by_legacy_id(reply_id)
+        contact: LegacyContact = await self.contacts.by_legacy_id(reply_id)
         date = datetime.fromtimestamp(user_submission["time"])
-        contact.carbon(
-            parse_comment_text(user_submission["text"]),
-            when=date,
+        contact.send_text(
+            parse_comment_text(user_submission["text"]), when=date, carbon=True
         )
         kid = await self.get_item(reply_id)
         contact.send_text(parse_comment_text(kid["text"]))
 
     async def get_item(self, item_id):
         async with self.http_session.get(f"{API_URL}/item/{item_id}.json") as r:
             return await r.json()
 
     async def logout(self):
         pass
 
-    async def send_text(self, t: str, c: LegacyContact, *, reply_to_msg_id=None):
-        goto = f"threads?id={self.hn_username}#{c.legacy_id}"
-        url = f"{REPLY_URL}?id={c.legacy_id}&goto={goto}"
+    async def send_text(self, text: str, chat: LegacyContact, **k):
+        goto = f"threads?id={self.hn_username}#{chat.legacy_id}"
+        url = f"{REPLY_URL}?id={chat.legacy_id}&goto={goto}"
         async with self.http_session.get(url) as r:
             if r.status != 200:
                 raise XMPPError(text="Couldn't get the post reply web page from HN")
             form_page_content = await r.text()
         match = re.search(HMAC_RE, form_page_content)
 
         if match is None:
@@ -137,16 +133,16 @@
                 text="Couldn't find the HMAC hidden input on the comment reply thread"
             )
 
         await asyncio.sleep(SLEEP_BEFORE_POST)
 
         form_dict = {
             "hmac": match.group(1),
-            "parent": c.legacy_id,
-            "text": t,
+            "parent": chat.legacy_id,
+            "text": text,
             "goto": goto,
         }
 
         form = aiohttp.FormData(form_dict)
         async with self.http_session.post(REPLY_POST_URL, data=form) as r:
             first_attempt_html_content = await r.text()
 
@@ -166,15 +162,15 @@
             async with self.http_session.post(REPLY_POST_URL, data=form) as r:
                 log.debug("Reply response #2: %s", r)
                 if r.status != 200:
                     raise XMPPError(text=f"Problem replying: {r}")
 
     # none of the following make sense in a HN context,
     # this is just to avoid raising NotImplementedErrors
-    async def send_file(self, u: str, c: LegacyContact, *, reply_to_msg_id=None):
+    async def send_file(self, *a, **k):
         pass
 
     async def active(self, c: LegacyContact):
         pass
 
     async def inactive(self, c: LegacyContact):
         pass
```

### Comparing `slidge-0.1.0b2/slidge/plugins/mattermost/api.py` & `slidge-0.1.0rc1/slidge/plugins/mattermost/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 )
 from mattermost_api_reference_client.models.upload_file_multipart_data import (
     UploadFileMultipartData,
 )
 from mattermost_api_reference_client.types import File, Unset
 
 
+class MattermostException(Exception):
+    pass
+
+
+class ContactNotFound(MattermostException):
+    pass
+
+
 class MattermostClient:
     # TODO: this should be autogenerated using a template in mattermost_api_reference_client
 
     def __init__(self, *args, **kwargs):
         self.http = AuthenticatedClient(*args, **kwargs)
         self.mm_id: asyncio.Future[str] = asyncio.get_running_loop().create_future()
         self.me: asyncio.Future[User] = asyncio.get_running_loop().create_future()
@@ -174,15 +182,15 @@
         if r is None or isinstance(r.id, Unset):
             raise RuntimeError(r)
         return r.id
 
     async def get_user_by_username(self, username: str) -> User:
         user = await get_user_by_username.asyncio(username, client=self.http)
         if user is None or isinstance(user.id, Unset):
-            raise RuntimeError("Contact not found")
+            raise ContactNotFound("Contact not found")
         return user
 
     async def get_direct_channel(self, user_id):
         direct_channel = await create_direct_channel.asyncio(
             json_body=[await self.mm_id, user_id], client=self.http
         )
         if direct_channel is None or isinstance(direct_channel.id, Unset):
```

### Comparing `slidge-0.1.0b2/slidge/plugins/mattermost/gateway.py` & `slidge-0.1.0rc1/slidge/plugins/mattermost/gateway.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 import re
 from datetime import datetime
 from typing import Any, Optional
 
 import emoji
 from mattermost_api_reference_client.models import Status
 from mattermost_api_reference_client.types import Unset
+from slixmpp import JID
+from slixmpp.exceptions import XMPPError
 
 from slidge import *
 
-from .api import MattermostClient
+from .api import ContactNotFound, MattermostClient
 from .websocket import EventType, MattermostEvent, Websocket
 
 
 class Gateway(BaseGateway):
     REGISTRATION_INSTRUCTIONS = (
         "Enter mattermost credentials. "
         "Get your MMAUTH_TOKEN on the web interface, using the dev tools of your browser (it's a cookie)."
@@ -42,16 +44,27 @@
     ROSTER_GROUP = "Mattermost"
 
     COMPONENT_NAME = "Mattermost (slidge)"
     COMPONENT_TYPE = "mattermost"
 
     COMPONENT_AVATAR = "https://play-lh.googleusercontent.com/aX7JaAPkmnkeThK4kgb_HHlBnswXF0sPyNI8I8LNmEMMo1vDvMx32tCzgPMsyEXXzZRc"
 
+    async def validate(
+        self, user_jid: JID, registration_form: dict[str, Optional[str]]
+    ):
+        mm_client = get_client_from_registration_form(registration_form)
+        try:
+            await mm_client.login()
+        except Exception as e:
+            raise ValueError("Could not authenticate: %s - %s", e, e.args)
+        if mm_client.me is None:
+            raise ValueError("Could not authenticate")
+
 
-class Contact(LegacyContact["Session"]):
+class Contact(LegacyContact["Session", str]):
     legacy_id: str
 
     MARKS = False
 
     def __init__(self, *a, **kw):
         super().__init__(*a, **kw)
         self._direct_channel_id: Optional[str] = None
@@ -102,15 +115,15 @@
                 for x in await self.session.get_mm_reactions(
                     legacy_msg_id, await self.mm_id()
                 )
             ],
         )
 
 
-class Roster(LegacyRoster[Contact, "Session"]):
+class Roster(LegacyRoster["Session", Contact, str]):
     user_id_to_username: dict[str, str]
     direct_channel_id_to_username: dict[str, str]
 
     def __init__(self, *a, **kw):
         super().__init__(*a, **kw)
         self.user_id_to_username = {}
         self.direct_channel_id_to_username = {}
@@ -119,92 +132,84 @@
         try:
             legacy_id = self.user_id_to_username[user_id]
         except KeyError:
             user = await self.session.mm_client.get_user(user_id)
             if isinstance(user.username, Unset):
                 raise RuntimeError
             legacy_id = self.user_id_to_username[user_id] = user.username
-        return self.by_legacy_id(legacy_id)
+        return await self.by_legacy_id(legacy_id)
 
     async def by_direct_channel_id(self, channel_id: str):
         if (username := self.direct_channel_id_to_username.get(channel_id)) is None:
             for c in self:
                 if (await c.direct_channel_id()) == channel_id:
                     return c
         else:
-            return self.by_legacy_id(username)
-
+            return await self.by_legacy_id(username)
 
-class Session(BaseSession[Contact, Roster, Gateway]):
-    mm_client: MattermostClient
-    ws: Websocket
-    messages_waiting_for_echo: set[str]
-    send_lock: asyncio.Lock
-    view_futures: dict[str, asyncio.Future[None]]
 
-    def post_init(self):
-        self.messages_waiting_for_echo = set()
+class Session(
+    BaseSession[
+        Gateway, str, Roster, Contact, LegacyBookmarks, LegacyMUC, LegacyParticipant
+    ]
+):
+    def __init__(self, user):
+        super().__init__(user)
+        self.messages_waiting_for_echo = set[str]()
         self.send_lock = asyncio.Lock()
         f = self.user.registration_form
-        url = f["url"] + f["basepath"]
-        self.mm_client = MattermostClient(
-            url,
-            verify_ssl=f["strict_ssl"],
-            timeout=5,
-            token=f["token"],
-        )
+        self.mm_client = get_client_from_registration_form(f)
         self.ws = Websocket(
-            re.sub("^http", "ws", f["url"]) + f["basepath"] + f["basepath_ws"],
+            re.sub("^http", "ws", f["url"] or "")
+            + (f["basepath"] or "")
+            + (f["basepath_ws"] or ""),
             f["token"],
         )
-        self.view_futures = {}
+        self.view_futures = dict[str, asyncio.Future[None]]()
 
     async def login(self):
         await self.mm_client.login()
         await self.add_contacts()
         self.xmpp.loop.create_task(self.ws.connect(self.on_mm_event))
-        if self.mm_client.me is None:
-            raise RuntimeError
-
         return f"Connected as '{(await self.mm_client.me).username}'"
 
     async def add_contacts(self):
         user_ids = await self.mm_client.get_contacts()
         contact_mm_users = await self.mm_client.get_users_by_ids(user_ids)
         contact_mm_statuses = await self.mm_client.get_users_statuses_by_ids(user_ids)
 
         statuses = {s.user_id: s for s in contact_mm_statuses}
 
         for user in contact_mm_users:
             status: Status = statuses[user.id]
-            contact = self.contacts.by_legacy_id(user.username)
+            contact = await self.contacts.by_legacy_id(user.username)
             self.contacts.user_id_to_username[user.id] = user.username
             if user.nickname:
                 contact.name = user.nickname
             elif user.first_name and user.last_name:
                 contact.name = user.first_name + " " + user.last_name
             elif user.first_name:
                 contact.name = user.first_name
             elif user.last_name:
                 contact.name = user.last_name
 
             contact.avatar = await self.mm_client.get_profile_image(user.id)
 
             await contact.add_to_roster()
-            contact.update_status(status.status)
+            contact.update_status(str(status.status))
 
     async def on_mm_event(self, event: MattermostEvent):
         self.log.debug("Event: %s", event)
         if event.type == EventType.Hello:
             self.log.debug("Received hello event: %s", event.data)
         elif event.type == EventType.Posted:
             post = event.data["post"]
             self.log.debug("Post: %s", pprint.pformat(post))
 
-            message = post["message"]
+            text = post["message"]
 
             channel_id = post["channel_id"]
             post_id = post["id"]
             user_id = post["user_id"]
 
             if event.data["channel_type"] == "D":  # Direct messages?
                 if user_id == await self.mm_client.mm_id:
@@ -218,70 +223,101 @@
                         for m in members:
                             if m.user_id != await self.mm_client.mm_id:
                                 contact = await self.contacts.by_mm_user_id(m.user_id)
                                 break
                         else:
                             raise RuntimeError("What?")
 
-                        contact.carbon(
-                            message,
-                            post_id,
-                            datetime.fromtimestamp(post["update_at"] / 1000),
+                        contact.send_text(
+                            text,
+                            legacy_msg_id=post_id,
+                            when=datetime.fromtimestamp(post["update_at"] / 1000),
+                            carbon=True,
                         )
                 else:
                     contact = await self.contacts.by_mm_user_id(user_id)
                     if event.data.get("set_online"):
                         contact.online()
-                    contact.send_text(message, legacy_msg_id=post_id)
-                    for file_meta in post.get("metadata", {}).get("files", []):
+                    file_metas = post.get("metadata", {}).get("files", [])
+
+                    if not file_metas:
+                        contact.send_text(text, legacy_msg_id=post_id)
+                        return
+
+                    last_file_i = len(file_metas) - 1
+
+                    for i, file_meta in enumerate(file_metas):
+                        last = i == last_file_i
                         await contact.send_file(
                             filename=file_meta["name"],
                             input_file=io.BytesIO(
                                 await self.mm_client.get_file(file_meta["id"])
                             ),
+                            legacy_msg_id=post_id if last else None,
+                            caption=text if last else None,
                         )
             elif event.data["channel_type"] == "P":
                 # private channel
                 pass
         elif event.type == EventType.ChannelViewed:
             channel_id = event.data["channel_id"]
             try:
                 f = self.view_futures.pop(channel_id)
             except KeyError:
                 pass
             else:
                 f.set_result(None)
                 return
             posts = await self.mm_client.get_posts_for_channel(channel_id)
-            last_msg_id = posts.posts.additional_keys[-1]
+            try:
+                last_msg_id = posts.posts.additional_keys[-1]
+            except IndexError:
+                self.log.debug("ChannelViewed event for a channel with no messages")
+                return
             if (c := await self.contacts.by_direct_channel_id(channel_id)) is None:
                 self.log.debug("Ignoring unknown channel")
             else:
-                c.carbon_read(last_msg_id)
+                c.displayed(last_msg_id, carbon=True)
         elif event.type == EventType.StatusChange:
             user_id = event.data["user_id"]
             if user_id == await self.mm_client.mm_id:
                 self.log.debug("Own status change")
             else:
 
                 contact = await self.contacts.by_mm_user_id(user_id)
                 contact.update_status(event.data["status"])
         elif event.type == EventType.Typing:
             contact = await self.contacts.by_mm_user_id(event.data["user_id"])
             contact.composing()
         elif event.type == EventType.PostEdited:
             post = event.data["post"]
-            contact = await self.contacts.by_mm_user_id(post["user_id"])
-            if post["channel_id"] == await contact.direct_channel_id():
-                contact.correct(post["id"], post["message"])
+            if post["user_id"] == await self.mm_client.mm_id:
+                if (
+                    c := await self.contacts.by_direct_channel_id(post["channel_id"])
+                ) is None:
+                    self.log.debug("Ignoring edit in unknown channel")
+                else:
+                    c.correct(post["id"], post["message"], carbon=True)
+            else:
+                contact = await self.contacts.by_mm_user_id(post["user_id"])
+                if post["channel_id"] == await contact.direct_channel_id():
+                    contact.correct(post["id"], post["message"])
         elif event.type == EventType.PostDeleted:
             post = event.data["post"]
-            contact = await self.contacts.by_mm_user_id(post["user_id"])
-            if post["channel_id"] == await contact.direct_channel_id():
-                contact.retract(post["id"])
+            if post["user_id"] == await self.mm_client.mm_id:
+                if (
+                    c := await self.contacts.by_direct_channel_id(post["channel_id"])
+                ) is None:
+                    self.log.debug("Ignoring edit in unknown channel")
+                else:
+                    c.retract(post["id"], carbon=True)
+            else:
+                contact = await self.contacts.by_mm_user_id(post["user_id"])
+                if post["channel_id"] == await contact.direct_channel_id():
+                    contact.retract(post["id"])
         elif event.type in (EventType.ReactionAdded, EventType.ReactionRemoved):
             reaction = event.data["reaction"]
             legacy_msg_id = reaction["post_id"]
             if (who := reaction["user_id"]) == await self.mm_client.mm_id:
                 user_reactions_name = {
                     f":{x}:" for x in await self.get_mm_reactions(legacy_msg_id, who)
                 }
@@ -292,32 +328,38 @@
                 }
                 self.log.debug(
                     "carbon: %s vs %s", user_reactions_name, user_reactions_char
                 )
                 contact = await self.contacts.by_direct_channel_id(
                     event.broadcast["channel_id"]
                 )
-                contact.carbon_react(legacy_msg_id, user_reactions_char)
+                contact.react(legacy_msg_id, user_reactions_char, carbon=True)
             else:
                 await (await self.contacts.by_mm_user_id(who)).update_reactions(
                     reaction["post_id"]
                 )
 
     async def logout(self):
         pass
 
-    async def send_text(self, t: str, c: Contact, *, reply_to_msg_id=None):
+    async def send_text(self, text: str, chat: Contact, **k):
         async with self.send_lock:
-            msg_id = await self.mm_client.send_message_to_user(c.legacy_id, t)
+            try:
+                msg_id = await self.mm_client.send_message_to_user(chat.legacy_id, text)
+            except ContactNotFound:
+                raise XMPPError(
+                    "recipient-unavailable", text="Cannot find this mattermost user"
+                )
+
             self.messages_waiting_for_echo.add(msg_id)
             return msg_id
 
-    async def send_file(self, u: str, c: Contact, *, reply_to_msg_id=None):
-        channel_id = await c.direct_channel_id()
-        file_id = await self.mm_client.upload_file(channel_id, u)
+    async def send_file(self, url: str, chat: Contact, **k):
+        channel_id = await chat.direct_channel_id()
+        file_id = await self.mm_client.upload_file(channel_id, url)
         return await self.mm_client.send_message_with_file(channel_id, file_id)
 
     async def active(self, c: Contact):
         pass
 
     async def inactive(self, c: Contact):
         pass
@@ -359,7 +401,17 @@
 
     async def get_mm_reactions(self, legacy_msg_id: str, user_id: Optional[str]):
         return {
             x.emoji_name
             for x in await self.mm_client.get_reactions(legacy_msg_id)
             if x.user_id == user_id
         }
+
+
+def get_client_from_registration_form(f: dict[str, Optional[str]]):
+    url = (f.get("url") or "") + (f.get("basepath") or "")
+    return MattermostClient(
+        url,
+        verify_ssl=f["strict_ssl"],
+        timeout=5,
+        token=f["token"],
+    )
```

### Comparing `slidge-0.1.0b2/slidge/plugins/mattermost/websocket.py` & `slidge-0.1.0rc1/slidge/plugins/mattermost/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 class Websocket:
     def __init__(self, url, token):
         self.token = token
         self.url = url
 
         self._alive = False
-        self._last_msg = 0
+        self._last_msg = 0.0
 
         self.ssl_verify = True
         self.keep_alive = True
         self.keep_alive_delay = 30
         self.websocket: asyncio.Future[
             aiohttp.ClientWebSocketResponse
         ] = asyncio.get_event_loop().create_future()
@@ -110,34 +110,29 @@
             context.verify_mode = ssl.CERT_NONE
 
         url = self.url
         self._alive = True
 
         while True:
             try:
-                kw_args = {}
                 async with aiohttp.ClientSession() as session:
-                    async with session.ws_connect(
-                        url,
-                        ssl=context,
-                        **kw_args,
-                    ) as websocket:
+                    async with session.ws_connect(url, ssl=context) as websocket:
                         self.websocket.set_result(websocket)
                         await self._authenticate_websocket(websocket)
                         while self._alive:
                             try:
                                 await self._start_loop(websocket, event_handler)
                             except aiohttp.ClientError:
                                 break
                         if (not self.keep_alive) or (not self._alive):
                             break
             except Exception as e:
-                log.exception(
-                    f"Failed to establish websocket connection: {type(e)} thrown"
-                )
+                log.error("Failed to establish websocket connection")
+                log.exception(e)
+                self.websocket = asyncio.get_event_loop().create_future()
                 await asyncio.sleep(self.keep_alive_delay)
 
     async def _start_loop(self, websocket, event_handler):
         """
         We will listen for websockets events, sending a heartbeats on a timer.
         If we don't the webserver would close the idle connection,
         forcing us to reconnect.
@@ -151,15 +146,16 @@
             self._last_msg = time.time()
             if (seq := d.get("seq_reply")) is None:
                 await handle_event(d, event_handler)
             else:
                 try:
                     self._futures.pop(seq).set_result(d)
                 except KeyError:
-                    log.warning("Ignoring %s", d)
+                    if d["seq_reply"] != 1 and d["status"] != "OK":
+                        log.warning("Ignoring %s", d)
         log.debug("cancelling heartbeat task")
         keep_alive.cancel()
         try:
             await keep_alive
         except asyncio.CancelledError:
             pass
```

### Comparing `slidge-0.1.0b2/slidge/plugins/signal/contact.py` & `slidge-0.1.0rc1/slidge/plugins/signal/contact.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+import asyncio
 import functools
 import logging
-from datetime import datetime
-from mimetypes import guess_extension
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional
 
 import aiosignald.exc as sigexc
 import aiosignald.generated as sigapi
 from slixmpp.exceptions import XMPPError
 
 from slidge import *
 
+from .util import AttachmentSenderMixin
+
 if TYPE_CHECKING:
+    from .group import Participant
     from .session import Session
 
 
-class Contact(LegacyContact["Session"]):
+class Contact(AttachmentSenderMixin, LegacyContact["Session", str]):
     CORRECTION = False
+    REACTIONS_SINGLE_EMOJI = True
 
     def __init__(self, *a, **k):
         super().__init__(*a, **k)
         # keys = msg timestamp; vals = single character emoji
         self.user_reactions = dict[int, str]()
+        self.xmpp.loop.create_task(self._update_info())
 
     @functools.cached_property
     def signal_address(self):
         return sigapi.JsonAddressv1(uuid=self.legacy_id)
 
     async def get_identities(self):
         s = await self.session.signal
@@ -36,71 +40,65 @@
                 address=self.signal_address,
             )
         except sigexc.UnregisteredUserError:
             raise XMPPError("not-found")
         identities = r.identities
         self.session.send_gateway_message(str(identities))
 
-    async def send_attachments(
-        self,
-        attachments: list[sigapi.JsonAttachmentv1],
-        /,
-        legacy_msg_id: int,
-        reply_to_msg_id: int,
-        when: Optional[datetime] = None,
-    ):
-        for attachment in attachments:
-            filename = get_filename(attachment)
-            with open(attachment.storedFilename, "rb") as f:
-                await self.send_file(
-                    filename=filename,
-                    input_file=f,
-                    content_type=attachment.contentType,
-                    legacy_msg_id=legacy_msg_id,
-                    reply_to_msg_id=reply_to_msg_id,
-                    when=when,
+    async def get_profile(self, max_attempts=10, sleep=1, exp=2):
+        attempts = 0
+        while attempts < max_attempts:
+            try:
+                profile = await (await self.session.signal).get_profile(
+                    account=self.session.phone, address=self.signal_address
+                )
+            except sigexc.ProfileUnavailableError as e:
+                log.debug(
+                    "Could not fetch the profile of a contact: %s, retrying later...",
+                    e.message,
                 )
+            else:
+                if profile.profile_name or profile.name or profile.contact_name:
+                    return profile
+            attempts += 1
+            await asyncio.sleep(sleep * attempts**exp)
 
-    async def update_info(self, profile: Optional[sigapi.Profilev1] = None):
+    async def _update_info(self, profile: Optional[sigapi.Profilev1] = None):
         if profile is None:
-            profile = await (await self.session.signal).get_profile(
-                account=self.session.phone, address=self.signal_address
-            )
+            profile = await self.get_profile()
+            if profile is None:
+                log.warning(
+                    "Could not update avatar, nickname, and phone of %s",
+                    self.signal_address,
+                )
+                return
+
         nick = profile.name or profile.profile_name
         if nick is not None:
-            nick = nick.replace("\u0000", "")
+            nick = nick.replace("\u0000", " ")
             self.name = nick
         if profile.avatar is not None:
             self.avatar = Path(profile.avatar)
 
         address = await (await self.session.signal).resolve_address(
             account=self.session.phone,
             partial=sigapi.JsonAddressv1(uuid=self.legacy_id),
         )
 
         self.set_vcard(full_name=nick, phone=address.number, note=profile.about)
-
-    async def update_and_add(self):
-        await self.update_info()
         await self.add_to_roster()
+        self.online()
+
+
+class Roster(LegacyRoster["Session", Contact, str]):
+    async def by_uuid(self, uuid: str):
+        return await self.by_json_address(sigapi.JsonAddressv1(uuid=uuid))
 
+    async def by_json_address(self, address: sigapi.JsonAddressv1):
+        return await self.by_legacy_id(address.uuid)
 
-def get_filename(attachment: sigapi.JsonAttachmentv1):
-    if f := attachment.customFilename:
-        return f
-    else:
-        filename = attachment.id or "unnamed"
-        ext = guess_extension(attachment.contentType)
-        if ext is not None:
-            filename += ext
-        return filename
-
-
-class Roster(LegacyRoster[Contact, "Session"]):
-    def by_json_address(self, address: sigapi.JsonAddressv1):
-        c = self.by_legacy_id(address.uuid)
-        if not c.added_to_roster:
-            self.session.xmpp.loop.create_task(c.update_and_add())
-        return c
+    async def jid_username_to_legacy_id(self, jid_username: str):
+        if jid_username in self.session.bookmarks.known_groups:
+            raise XMPPError("bad-request", "This is a group ID, not a contact ID")
 
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0b2/slidge/plugins/signal/session.py` & `slidge-0.1.0rc1/slidge/plugins/telegram/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,448 +1,325 @@
 import asyncio
 import functools
-import logging
-import os
-import tempfile
 from datetime import datetime
-from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Union
 
-import aiohttp
-import aiosignald.exc as sigexc
-import aiosignald.generated as sigapi
-from slixmpp.exceptions import XMPPError
+import aiotdlib
+from aiotdlib import api as tgapi
 
-from slidge import *
+from . import config
+from .util import get_best_file
 
 if TYPE_CHECKING:
-    from .contact import Contact, Roster
-    from .gateway import Gateway
-
-from . import txt
+    from .contact import Contact
+    from .group import MUC, Participant
+    from .session import Session
+
+
+def get_base_kwargs(user_reg_form: dict):
+    return dict(
+        phone_number=user_reg_form["phone"],
+        api_id=user_reg_form.get("api_id") or config.API_ID,
+        api_hash=user_reg_form.get("api_hash") or config.API_HASH,
+        database_encryption_key=config.TDLIB_KEY,
+        files_directory=config.TDLIB_PATH,
+    )
+
+
+class CredentialsValidation(aiotdlib.Client):
+    def __init__(self, registration_form: dict):
+        super().__init__(**get_base_kwargs(registration_form))
+        self.code_future: asyncio.Future[
+            str
+        ] = asyncio.get_running_loop().create_future()
+        self._auth_get_code = self._get_code
+        self._auth_get_password = self._get_code
+
+    async def _get_code(self):
+        return await self.code_future
+
+
+class TelegramClient(aiotdlib.Client):
+    def __init__(self, session: "Session"):
+        super().__init__(
+            parse_mode=aiotdlib.ClientParseMode.MARKDOWN,
+            **get_base_kwargs(session.user.registration_form),
+        )
+        self.session = session
+        self.contacts = session.contacts
+        self.bookmarks = session.bookmarks
+        self.log = self.session.log
+
+        async def input_(prompt):
+            self.session.send_gateway_status(f"Action required: {prompt}")
+            return await session.input(prompt)
+
+        self.input = input_
+        self._auth_get_code = functools.partial(input_, "Enter code")
+        self._auth_get_password = functools.partial(input_, "Enter 2FA password:")
+        self._auth_get_first_name = functools.partial(input_, "Enter first name:")
+        self._auth_get_last_name = functools.partial(input_, "Enter last name:")
 
+        self.add_event_handler(self.dispatch_update, tgapi.API.Types.ANY)
 
-def handle_unregistered_recipient(func):
-    @functools.wraps(func)
-    async def wrapped(*a, **kw):
+    async def dispatch_update(self, _self, update: tgapi.Update):
         try:
-            return await func(*a, **kw)
-        except (
-            sigexc.UnregisteredUserError,
-            sigexc.IllegalArgumentException,
-            sigexc.InternalError,
-        ) as e:
-            raise XMPPError(
-                "item-not-found",
-                text=e.message,
-            )
+            handler = getattr(self, "handle_" + update.ID[6:])
+        except AttributeError:
+            self.session.log.debug("No handler for %s, ignoring", update.ID)
+        except IndexError:
+            self.session.log.debug("Ignoring weird event: %s", update.ID)
+        else:
+            await handler(update)
 
-    return wrapped
+    async def handle_NewMessage(self, update: tgapi.UpdateNewMessage):
+        if (msg := update.message).is_channel_post:
+            self.log.debug("Ignoring channel post")
+            return
 
+        if not await self.is_private_chat(msg.chat_id):
+            return await self.handle_group_message(msg)
 
-class Session(BaseSession["Contact", "Roster", "Gateway"]):
-    """
-    Represents a signal account
-    """
-
-    def __init__(self, user: GatewayUser):
-        """
-
-        :param user:
-        """
-        super().__init__(user)
-        self.phone = self.user.registration_form["phone"]
-        if self.phone is None:
-            raise RuntimeError
-        self.signal = self.xmpp.signal
-        self.xmpp.sessions_by_phone[self.phone] = self
-        self.reaction_ack_futures: dict[tuple[int, str], asyncio.Future[None]] = {}
-        self.connected = self.xmpp.loop.create_future()
+        session = self.session
+        if msg.is_outgoing:
+            # This means slidge is responsible for this message, so no carbon is needed;
+            # but maybe this does not handle all possible cases gracefully?
+            if msg.sending_state is not None or msg.id in session.sent:
+                return
+            content = msg.content
+            contact = await session.contacts.by_legacy_id(msg.chat_id)
+            if isinstance(content, tgapi.MessageText):
+                contact.send_text(
+                    content.text.text,
+                    legacy_msg_id=msg.id,
+                    when=datetime.fromtimestamp(msg.date),
+                    carbon=True,
+                )
+            elif best_file := get_best_file(content):
+                file = await self.api.download_file(
+                    file_id=best_file.id,
+                    synchronous=True,
+                    priority=1,
+                    offset=0,
+                    limit=0,
+                )
+                has_caption = (caption := content.caption) and (text := caption.text)
+                await contact.send_file(
+                    filename=file.local.path,
+                    legacy_msg_id=None if has_caption else msg.id,
+                    carbon=True,
+                )
+                if has_caption:
+                    contact.send_text(text, legacy_msg_id=msg.id, carbon=True)
+            return
 
-    @staticmethod
-    def xmpp_msg_id_to_legacy_msg_id(i: str) -> int:
-        try:
-            return int(i)
-        except ValueError:
-            raise NotImplementedError
-
-    @handle_unregistered_recipient
-    async def paused(self, c: "Contact"):
-        await (await self.signal).typing(
-            account=self.phone, typing=False, address=c.signal_address
-        )
+        sender = msg.sender_id
+        if not isinstance(sender, tgapi.MessageSenderUser):
+            # Does this happen?
+            self.log.warning("Ignoring chat sender in direct message: %s", msg)
+            return
 
-    async def correct(self, text: str, legacy_msg_id: Any, c: "Contact"):
-        return await self.send_text("Correction: " + text, c)
+        await (await session.contacts.by_legacy_id(sender.user_id)).send_tg_message(msg)
 
-    async def search(self, form_values: dict[str, str]):
-        phone = form_values.get("phone")
-        if phone is None:
-            raise ValueError("Empty phone")
+    async def handle_group_message(self, msg: tgapi.Message):
+        self.log.debug("MUC message: %s", msg)
+        if msg.is_outgoing:
+            if msg.sending_state is not None or msg.id in self.session.sent:
+                return
 
-        try:
-            address = await (await self.signal).resolve_address(
-                account=self.phone,
-                partial=sigapi.JsonAddressv1(number=form_values.get("phone")),
+        muc = await self.bookmarks.by_legacy_id(msg.chat_id)
+        sender = msg.sender_id
+        if isinstance(sender, tgapi.MessageSenderUser):
+            participant = await muc.participant_by_tg_user(
+                await self.api.get_user(sender.user_id)
             )
-        except sigexc.UnregisteredUserError:
-            return
+        else:
+            participant = await muc.participant_system()
+        await participant.send_tg_message(msg)
 
-        contact = self.contacts.by_json_address(address)
+    async def handle_UserStatus(self, update: tgapi.UpdateUserStatus):
+        if update.user_id == await self.get_my_id():
+            return
+        contact = await self.contacts.by_legacy_id(update.user_id)
+        if not contact.added_to_roster:
+            self.log.debug("Ignoring presence of contact not in the roster")
+            return
+        contact.update_status(update.status)
 
-        return SearchResult(
-            fields=[FormField("phone"), FormField("jid", type="jid-single")],
-            items=[{"phone": phone, "jid": contact.jid.bare}],
-        )
+    async def handle_ChatReadOutbox(self, update: tgapi.UpdateChatReadOutbox):
+        if await self.is_private_chat(update.chat_id):
+            contact = await self.contacts.by_legacy_id(update.chat_id)
+            contact.displayed(update.last_read_outbox_message_id)
+        else:
+            muc = await self.bookmarks.by_legacy_id(update.chat_id)
+            async for p in muc.get_participants():
+                p.displayed(update.last_read_outbox_message_id)
+
+    async def handle_ChatAction(self, action: tgapi.UpdateChatAction):
+        sender = action.sender_id
+        if not isinstance(sender, tgapi.MessageSenderUser):
+            self.log.debug("Ignoring action: %s", action)
+            return
 
-    async def login(self):
-        """
-        Attempt to listen to incoming events for this account,
-        or pursue the registration process if needed.
-        """
-        try:
-            await (await self.signal).subscribe(account=self.phone)
-        except sigexc.NoSuchAccountError:
-            device = self.user.registration_form["device"]
-            try:
-                if device == "primary":
-                    await self.register()
-                elif device == "secondary":
-                    await self.link()
-                else:
-                    # This should never happen
-                    self.send_gateway_status("Disconnected", show="dnd")
-                    raise TypeError("Unknown device type", device)
-            except sigexc.SignaldException as e:
-                self.xmpp.send_message(
-                    mto=self.user.jid,
-                    mbody=f"Something went wrong: {e}",
-                    mfrom=self.xmpp.boundjid,
-                )
-                raise
-            await (await self.signal).subscribe(account=self.phone)
-        await self.connected
-        await self.add_contacts_to_roster()
-        return f"Connected as {self.phone}"
+        chat_id = action.chat_id
+        user_id = sender.user_id
+        if chat_id == user_id:
+            composer: Union[
+                "Contact", "Participant"
+            ] = await self.contacts.by_legacy_id(chat_id)
+        else:
+            muc: MUC = await self.bookmarks.by_legacy_id(chat_id)
+            composer = await muc.participant_by_tg_user(
+                await self.api.get_user(user_id)
+            )
 
-    async def on_websocket_connection_state(
-        self, state: sigapi.WebSocketConnectionStatev1
-    ):
-        if (
-            state.state == "CONNECTED"
-            and state.socket == "IDENTIFIED"
-            and not self.connected.done()
-        ):
-            self.connected.set_result(True)
+        composer.composing()
 
-    async def register(self):
-        self.send_gateway_status("Registering…", show="dnd")
-        try:
-            await (await self.signal).register(self.phone)
-        except sigexc.CaptchaRequiredError:
-            self.send_gateway_status("Captcha required", show="dnd")
-            captcha = await self.input(txt.CAPTCHA_REQUIRED)
-            await (await self.signal).register(self.phone, captcha=captcha)
-        sms_code = await self.input(
-            f"Reply to this message with the code you have received by SMS at {self.phone}.",
-        )
-        await (await self.signal).verify(account=self.phone, code=sms_code)
-        await (await self.signal).set_profile(
-            account=self.phone, name=self.user.registration_form["name"]
-        )
-        self.send_gateway_message(txt.REGISTER_SUCCESS)
+    async def handle_ChatReadInbox(self, action: tgapi.UpdateChatReadInbox):
+        if not await self.is_private_chat(action.chat_id):
+            return
 
-    async def send_linking_qrcode(self):
-        self.send_gateway_status("QR scan needed", show="dnd")
-        resp = await (await self.signal).generate_linking_uri()
-        await self.send_qr(resp.uri)
-        self.xmpp.send_message(
-            mto=self.user.jid,
-            mbody=f"Use this URI or QR code on another signal device to "
-            f"finish linking your XMPP account\n{resp.uri}",
-            mfrom=self.xmpp.boundjid,
+        session = self.session
+        msg_id = action.last_read_inbox_message_id
+        self.log.debug(
+            "Self read mark for %s and we sent %s", msg_id, session.sent_read_marks
         )
-        return resp
-
-    async def link(self):
-        resp = await self.send_linking_qrcode()
         try:
-            await (await self.signal).finish_link(
-                device_name=self.user.registration_form["device_name"],
-                session_id=resp.session_id,
-            )
-        except sigexc.ScanTimeoutError:
-            while True:
-                r = await self.input(txt.LINK_TIMEOUT)
-                if r in ("cancel", "link"):
-                    break
+            session.sent_read_marks.remove(msg_id)
+        except KeyError:
+            # slidge didn't send this read mark, so it comes from the official tg client
+            contact = await session.contacts.by_legacy_id(action.chat_id)
+            contact.displayed(msg_id, carbon=True)
+
+    async def handle_MessageContent(self, action: tgapi.UpdateMessageContent):
+        new = action.new_content
+        if isinstance(new, tgapi.MessagePhoto):
+            # Happens when the user send a picture, looks safe to ignore
+            self.log.debug("Ignoring message photo update: %s", new)
+            return
+        if not isinstance(new, tgapi.MessageText):
+            self.log.warning("Ignoring message update: %s", new)
+            return
+        session = self.session
+        corrected_msg_id = action.message_id
+        chat_id = action.chat_id
+        try:
+            fut = session.user_correction_futures.pop(action.message_id)
+        except KeyError:
+            if await self.is_private_chat(chat_id):
+                contact = await session.contacts.by_legacy_id(chat_id)
+                if action.message_id in self.session.sent:
+                    contact.correct(corrected_msg_id, new.text.text, carbon=True)
                 else:
-                    self.send_gateway_message("Please reply either 'link' or 'cancel'")
-            if r == "cancel":
-                raise
-            elif r == "link":
-                await self.link()  # TODO: set a max number of attempts
-        except sigexc.SignaldException as e:
-            self.xmpp.send_message(
-                mto=self.user.jid,
-                mbody=f"Something went wrong during the linking process: {e}.",
-                mfrom=self.xmpp.boundjid,
-            )
-            raise
+                    contact.correct(corrected_msg_id, new.text.text)
+            else:
+                if action.message_id not in self.session.muc_sent_msg_ids:
+                    muc = await session.bookmarks.by_legacy_id(chat_id)
+                    msg = await self.api.get_message(chat_id, corrected_msg_id)
+                    participant = await muc.participant_by_tg_user(
+                        await self.api.get_user(msg.sender_id.user_id)
+                    )
+                    participant.correct(action.message_id, new.text.text)
         else:
-            self.send_gateway_message(txt.LINK_SUCCESS)
-
-    async def logout(self):
-        await (await self.signal).unsubscribe(account=self.phone)
+            self.log.debug("User correction confirmation received")
+            fut.set_result(None)
 
-    async def add_contacts_to_roster(self):
-        """
-        Populate a user's roster
-        """
-        profiles = await (await self.signal).list_contacts(account=self.phone)
-        for profile in profiles.profiles:
-            contact = self.contacts.by_json_address(profile.address)
-            await contact.update_info()
+    async def handle_User(self, action: tgapi.UpdateUser):
+        u = action.user
+        if u.id == await self.get_my_id():
+            return
+        contact = await self.session.contacts.by_legacy_id(u.id)
+        await contact.update_info_from_user(u)
+        if u.is_contact:
             await contact.add_to_roster()
-            contact.online()
-
-    async def on_signal_message(self, msg: sigapi.IncomingMessagev1):
-        """
-        User has received 'something' from signal
-
-        :param msg:
-        """
-        if (sync_msg := msg.sync_message) is not None:
-            if sync_msg.contacts is not None and msg.sync_message.contactsComplete:
-                log.debug("Received a sync contact updates")
-                await self.add_contacts_to_roster()
-
-            if (sent := sync_msg.sent) is None:
-                # Probably a 'message read' marker
-                log.debug("No sent message in this sync message")
-                return
-            sent_msg = sent.message
-            if sent_msg.group or sent_msg.groupV2:
-                return
 
-            contact = self.contacts.by_json_address(sent.destination)
+    async def handle_MessageInteractionInfo(
+        self, update: tgapi.UpdateMessageInteractionInfo
+    ):
+        if not await self.is_private_chat(update.chat_id):
+            return
 
-            if (body := sent_msg.body) is not None:
-                contact.carbon(
-                    body=body,
-                    when=datetime.fromtimestamp(sent_msg.timestamp / 1000),
-                )
-            if (reaction := sent_msg.reaction) is not None:
-                try:
-                    fut = self.reaction_ack_futures.pop(
-                        (reaction.targetSentTimestamp, reaction.emoji)
-                    )
-                except KeyError:
-                    contact.carbon_react(
-                        reaction.targetSentTimestamp,
-                        () if reaction.remove else reaction.emoji,
-                    )
+        contact = await self.session.contacts.by_legacy_id(update.chat_id)
+        me = await self.get_my_id()
+        if update.interaction_info is None:
+            contact.react(update.message_id, [])
+            contact.react(update.message_id, [], carbon=True)
+        else:
+            user_reactions = list[str]()
+            contact_reactions = list[str]()
+            # these sanity checks might not be necessary, but in doubt…
+            for reaction in update.interaction_info.reactions:
+                if reaction.total_count == 1:
+                    if len(reaction.recent_sender_ids) != 1:
+                        self.log.warning(
+                            "Weird reactions (wrong count): %s",
+                            update.interaction_info.reactions,
+                        )
+                        continue
+                    sender = reaction.recent_sender_ids[0]
+                    if isinstance(sender, tgapi.MessageSenderUser):
+                        if sender.user_id == me:
+                            user_reactions.append(reaction.reaction)
+                        elif sender.user_id == contact.legacy_id:
+                            contact_reactions.append(reaction.reaction)
+                    else:
+                        self.log.warning(
+                            "Weird reactions (neither me nor them): %s",
+                            update.interaction_info.reactions,
+                        )
+                elif reaction.total_count == 2:
+                    user_reactions.append(reaction.reaction)
+                    contact_reactions.append(reaction.reaction)
                 else:
-                    fut.set_result(None)
-            if (delete := sent_msg.remoteDelete) is not None:
-                contact.carbon_retract(delete.target_sent_timestamp)
+                    self.log.warning(
+                        "Weird reactions (empty): %s", update.interaction_info.reactions
+                    )
 
-        contact = self.contacts.by_json_address(msg.source)
+            contact.react(update.message_id, contact_reactions)
+            contact.react(update.message_id, user_reactions, carbon=True)
 
-        if (data := msg.data_message) is not None:
-            if data.group or data.groupV2:
-                return
-            if (quote := data.quote) is None:
-                reply_to_msg_id = None
-            else:
-                reply_to_msg_id = quote.id
-            await contact.send_attachments(
-                data.attachments,
-                legacy_msg_id=msg.data_message.timestamp,
-                reply_to_msg_id=reply_to_msg_id,
-            )
-            if (body := data.body) is not None:
-                contact.send_text(
-                    body=body,
-                    legacy_msg_id=msg.data_message.timestamp,
-                    reply_to_msg_id=reply_to_msg_id,
-                    when=datetime.fromtimestamp(msg.data_message.timestamp / 1000),
-                )
-            if (reaction := data.reaction) is not None:
-                self.log.debug("Reaction: %s", reaction)
-                if reaction.remove:
-                    contact.react(reaction.targetSentTimestamp)
+    async def handle_DeleteMessages(self, update: tgapi.UpdateDeleteMessages):
+        if not update.is_permanent:  # tdlib send 'delete from cache' updates apparently
+            self.log.debug("Ignoring non permanent delete")
+            return
+        for legacy_msg_id in update.message_ids:
+            try:
+                future = self.session.delete_futures.pop(legacy_msg_id)
+            except KeyError:
+                if await self.is_private_chat(update.chat_id):
+                    contact = await self.session.contacts.by_legacy_id(update.chat_id)
+                    if legacy_msg_id in self.session.sent:
+                        contact.retract(legacy_msg_id, carbon=True)
+                    else:
+                        contact.retract(legacy_msg_id)
                 else:
-                    contact.react(reaction.targetSentTimestamp, reaction.emoji)
-            if (delete := data.remoteDelete) is not None:
-                contact.retract(delete.target_sent_timestamp)
-
-        if (typing_message := msg.typing_message) is not None:
-            if typing_message.group_id:
-                return
-            action = typing_message.action
-            if action == "STARTED":
-                contact.active()
-                contact.composing()
-            elif action == "STOPPED":
-                contact.paused()
-
-        if (receipt_message := msg.receipt_message) is not None:
-            type_ = receipt_message.type
-            if type_ == "DELIVERY":
-                for t in msg.receipt_message.timestamps:
-                    contact.received(t)
-            elif type_ == "READ":
-                for t in msg.receipt_message.timestamps:
-                    contact.displayed(t)
-
-    @handle_unregistered_recipient
-    async def send_text(self, t: str, c: "Contact", *, reply_to_msg_id=None) -> int:
-        if reply_to_msg_id is None:
-            quote = None
-        else:
-            quote = sigapi.JsonQuotev1(
-                id=reply_to_msg_id,
-                author=c.signal_address,
-                text=""  # not sure what this accomplishes? does not seem to have any effect,
-                # but must not be None or NullPointerException
-            )
-        response = await (await self.signal).send(
-            account=self.phone,
-            recipientAddress=c.signal_address,
-            messageBody=t,
-            quote=quote,
-        )
-        result = response.results[0]
-        log.debug("Result: %s", result)
-        if result.networkFailure or result.proof_required_failure:
-            raise XMPPError(str(result))
-        elif result.identityFailure:
-            s = await self.signal
-            identities = (
-                await s.get_identities(
-                    account=self.phone,
-                    address=c.signal_address,
-                )
-            ).identities
-            ans = await self.input(
-                f"The identity of {c.legacy_id} has changed. "
-                f"Do you want to trust all their identities and resend the message?"
-            )
-            if ans.lower().startswith("y"):
-                for i in identities:
-                    await (await self.signal).trust(
-                        account=self.phone,
-                        address=c.signal_address,
-                        safety_number=i.safety_number,
-                    )
-                await self.send_text(t, c, reply_to_msg_id=reply_to_msg_id)
+                    return
+                    # FIXME: does not work because we need to fetch the participant,
+                    #        the DeleteMessage payload has not author info,
+                    #        and we cannot get_message() anymore
+                    # We should probably use MUC moderation tools here
+                    # muc = await self.session.bookmarks.by_legacy_id(update.chat_id)
+                    # msg = await self.api.get_message(update.chat_id, legacy_msg_id)
+                    # participant = await muc.participant_by_tg_user_id(
+                    #     msg.sender_id.user_id
+                    # )
+                    # participant.retract(legacy_msg_id)
             else:
-                raise XMPPError(str(result))
-        return response.timestamp
-
-    @handle_unregistered_recipient
-    async def send_file(self, u: str, c: "Contact", *, reply_to_msg_id=None):
-        s = await self.signal
-        async with aiohttp.ClientSession() as client:
-            async with client.get(url=u) as r:
-                with tempfile.TemporaryDirectory(
-                    dir=Path(self.xmpp.signal_socket).parent,
-                ) as d:
-                    os.chmod(d, 0o777)
-                    with open(Path(d) / r.url.name, "wb") as f:
-                        f.write(await r.content.read())
-                        os.chmod(
-                            f.name, 0o666
-                        )  # temp file is 0600 https://stackoverflow.com/a/10541972/5902284
-                        signal_r = await s.send(
-                            account=self.phone,
-                            recipientAddress=c.signal_address,
-                            attachments=[sigapi.JsonAttachmentv1(filename=f.name)],
-                        )
-                        return signal_r.timestamp
-
-    async def active(self, c: "Contact"):
-        pass
+                future.set_result(update)
 
-    async def inactive(self, c: "Contact"):
-        pass
-
-    @handle_unregistered_recipient
-    async def composing(self, c: "Contact"):
-        self.log.debug("COMPOSING %s", c)
-        await (await self.signal).typing(
-            account=self.phone,
-            address=c.signal_address,
-            typing=True,
-        )
-
-    @handle_unregistered_recipient
-    async def displayed(self, legacy_msg_id: int, c: "Contact"):
-        await (await self.signal).mark_read(
-            account=self.phone,
-            to=c.signal_address,
-            timestamps=[legacy_msg_id],
-        )
-
-    @handle_unregistered_recipient
-    async def react(self, legacy_msg_id: int, emojis: list[str], c: "Contact"):
-        remove = len(emojis) == 0
-        if remove:
+    async def handle_MessageSendSucceeded(
+        self, update: tgapi.UpdateMessageSendSucceeded
+    ):
+        self.session.sent_read_marks.add(update.message.id)
+        for _ in range(10):
             try:
-                emoji = c.user_reactions.pop(legacy_msg_id)
+                future = self.session.ack_futures.pop(update.message.id)
             except KeyError:
-                self.send_gateway_message(
-                    f"Slidge failed to remove your reactions on message '{legacy_msg_id}'"
-                )
-                self.log.warning("Could not find the emoji to remove reaction")
+                await asyncio.sleep(0.5)
+            else:
+                future.set_result(update.message.id)
                 return
-        else:
-            emoji = emojis[-1]
-            if len(emojis) > 1:
-                self.send_gateway_message("Only one reaction per message on signal")
-                c.carbon_react(legacy_msg_id, emoji)
-            c.user_reactions[legacy_msg_id] = emoji
-
-        response = await (await self.signal).react(
-            username=self.phone,
-            recipientAddress=c.signal_address,
-            reaction=sigapi.JsonReactionv1(
-                emoji=emoji,
-                remove=remove,
-                targetAuthor=sigapi.JsonAddressv1(number=self.phone)
-                if legacy_msg_id in self.sent
-                else c.signal_address,
-                targetSentTimestamp=legacy_msg_id,
-            ),
-        )
-        result = response.results[0]
-        if (
-            result.networkFailure
-            or result.identityFailure
-            or result.proof_required_failure
-        ):
-            raise XMPPError(str(result))
-        f = self.reaction_ack_futures[
-            (legacy_msg_id, emoji)
-        ] = self.xmpp.loop.create_future()
-        await f
-
-    @handle_unregistered_recipient
-    async def retract(self, legacy_msg_id: int, c: "Contact"):
-        try:
-            await (await self.signal).remote_delete(
-                account=self.phone, address=c.signal_address, timestamp=legacy_msg_id
-            )
-        except sigexc.SignaldException as e:
-            raise XMPPError(text=f"Something went wrong during remote delete: {e}")
-
-    async def add_device(self, uri: str):
-        try:
-            await (await self.signal).add_device(account=self.phone, uri=uri)
-        except sigexc.SignaldException as e:
-            self.send_gateway_message(f"Problem: {e}")
-        else:
-            self.send_gateway_message("Linking OK")
-
+        self.log.warning("Ignoring Send success for %s", update.message.id)
 
-log = logging.getLogger(__name__)
+    async def is_private_chat(self, chat_id: int):
+        chat = await self.get_chat(chat_id)
+        return isinstance(chat.type_, tgapi.ChatTypePrivate)
```

### Comparing `slidge-0.1.0b2/slidge/plugins/skype.py` & `slidge-0.1.0rc1/slidge/plugins/skype.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
-import concurrent.futures
 import io
 import logging
 import pprint
 import threading
 from pathlib import Path
 from threading import Lock, Thread
 from typing import Any, Optional
 
 import aiohttp
 import skpy
+from requests.exceptions import ConnectionError
 from slixmpp import JID
 from slixmpp.exceptions import XMPPError
 
 from slidge import *
 
 
 class Gateway(BaseGateway["Session"]):
@@ -29,50 +29,28 @@
     COMPONENT_TYPE = "skype"
 
     COMPONENT_AVATAR = "https://logodownload.org/wp-content/uploads/2017/05/skype-logo-1-1-2048x2048.png"
 
     async def validate(
         self, user_jid: JID, registration_form: dict[str, Optional[str]]
     ):
-        pass
-
-    def __init__(self, args):
-        super().__init__(args)
-        self.executor = concurrent.futures.ThreadPoolExecutor()
-
-    def shutdown(self):
-        super().shutdown()
-        log.debug("Shutting down thread pool")
-        self.executor.shutdown(wait=False, cancel_futures=True)
-        log.debug("Shutting down user threads")
-        for user in user_store.get_all():
-            session = self._session_cls.from_jid(user.jid)
-            if thread := session.thread:
-                thread.stop()
-
-
-class Roster(LegacyRoster):
-    # ':' is forbidden in the username part of a JID
-
-    @staticmethod
-    def legacy_id_to_jid_username(legacy_id: str) -> str:
-        if legacy_id.startswith("live:"):
-            return legacy_id.replace("live:", "__live__")
-        else:
-            return legacy_id
-
-    @staticmethod
-    def jid_username_to_legacy_id(jid_username: str) -> str:
-        if jid_username.startswith("__live__"):
-            return jid_username.replace("__live__", "live:")
-        else:
-            return jid_username
+        try:
+            await asyncio.to_thread(
+                skpy.Skype,
+                registration_form["username"],
+                registration_form["password"],
+                str(global_config.HOME_DIR / user_jid.bare),
+            )
+        except skpy.SkypeApiException:
+            raise XMPPError("bad-request")
+        except skpy.SkypeAuthException:
+            raise XMPPError("forbidden", etype="auth")
 
 
-class Contact(LegacyContact):
+class Contact(LegacyContact["Session", str]):
     def update_presence(self, status: skpy.SkypeUtils.Status):
         if status == skpy.SkypeUtils.Status.Offline:
             self.offline()
         elif status == skpy.SkypeUtils.Status.Busy:
             self.busy()
         elif status == skpy.SkypeUtils.Status.Away:
             self.away("Away")
@@ -103,44 +81,54 @@
                 # no need to sleep since getEvents blocks for 30 seconds already
                 asyncio.run_coroutine_threadsafe(session.on_skype_event(event), loop)
 
     def stop(self):
         self.stop_event.set()
 
 
-class Session(BaseSession[Contact, Roster, Gateway]):
+class Session(
+    BaseSession[
+        Gateway,
+        int,
+        LegacyRoster,
+        Contact,
+        LegacyBookmarks,
+        LegacyMUC,
+        LegacyParticipant,
+    ]
+):
     skype_token_path: Path
     sk: skpy.Skype
-    thread: Optional[ListenThread]
-    sent_by_user_to_ack: dict[int, asyncio.Future]
-    unread_by_user: dict[int, skpy.SkypeMsg]
-    send_lock: Lock
-
-    def post_init(self):
-        self.skype_token_path = self.xmpp.home_dir / self.user.bare_jid
-        self.thread = None
-        self.sent_by_user_to_ack = {}
-        self.unread_by_user = {}
+
+    def __init__(self, user):
+        super().__init__(user)
+        self.skype_token_path = global_config.HOME_DIR / self.user.bare_jid
+        self.thread: Optional[ListenThread] = None
+        self.sent_by_user_to_ack = dict[int, asyncio.Future]()
+        self.unread_by_user = dict[int, skpy.SkypeMsg]()
         self.send_lock = Lock()
 
-    async def async_wrap(self, func, *args):
-        return await self.xmpp.loop.run_in_executor(self.xmpp.executor, func, *args)
+    def shutdown(self):
+        super().shutdown()
+        log.debug("Shutting down user threads")
+        if thread := self.thread:
+            thread.stop()
 
     async def login(self):
         f = self.user.registration_form
-        self.sk = await self.async_wrap(
+        self.sk = await asyncio.to_thread(
             skpy.Skype,
             f["username"],
             f["password"],
             str(self.skype_token_path),
         )
 
         self.sk.subscribePresence()
         for contact in self.sk.contacts:
-            c = self.contacts.by_legacy_id(contact.id)
+            c = await self.contacts.by_legacy_id(contact.id)
             first = contact.name.first
             last = contact.name.last
             if first is not None and last is not None:
                 c.name = f"{first} {last}"
             elif first is not None:
                 c.name = first
             elif last is not None:
@@ -159,50 +147,50 @@
         if isinstance(event, skpy.SkypeNewMessageEvent):
             while self.send_lock.locked():
                 await asyncio.sleep(0.1)
             msg = event.msg
             chat = event.msg.chat
             if isinstance(chat, skpy.SkypeSingleChat):
                 log.debug("this is a single chat with user: %s", chat.userIds[0])
-                contact = self.contacts.by_legacy_id(chat.userIds[0])
+                contact = await self.contacts.by_legacy_id(chat.userIds[0])
                 if msg.userId == self.sk.userId:
                     try:
                         fut = self.sent_by_user_to_ack.pop(msg.clientId)
                     except KeyError:
                         if log.isEnabledFor(logging.DEBUG):
                             log.debug(
                                 "Slidge did not send this message: %s",
                                 pprint.pformat(vars(event)),
                             )
-                        contact.carbon(msg.plain)
+                        contact.send_text(msg.plain, carbon=True)
                     else:
                         fut.set_result(msg)
                 else:
                     if isinstance(msg, skpy.SkypeTextMsg):
                         contact.send_text(msg.plain, legacy_msg_id=msg.clientId)
                         self.unread_by_user[msg.clientId] = msg
                     elif isinstance(msg, skpy.SkypeFileMsg):
                         file = io.BytesIO(
-                            await self.async_wrap(lambda: msg.fileContent)
+                            await asyncio.to_thread(lambda: msg.fileContent)
                         )  # non-blocking download / lambda because fileContent = property
                         await contact.send_file(filename=msg.file.name, input_file=file)
         elif isinstance(event, skpy.SkypeTypingEvent):
-            contact = self.contacts.by_legacy_id(event.userId)
+            contact = await self.contacts.by_legacy_id(event.userId)
             if event.active:
                 contact.composing()
             else:
                 contact.paused()
         elif isinstance(event, skpy.SkypeEditMessageEvent):
             msg = event.msg
             chat = event.msg.chat
             if isinstance(chat, skpy.SkypeSingleChat):
                 if (user_id := msg.userId) != self.sk.userId:
                     if log.isEnabledFor(logging.DEBUG):
                         log.debug("edit msg event: %s", pprint.pformat(vars(event)))
-                    contact = self.contacts.by_legacy_id(user_id)
+                    contact = await self.contacts.by_legacy_id(user_id)
                     msg_id = msg.clientId
                     log.debug("edited msg id: %s", msg_id)
                     if text := msg.plain:
                         contact.correct(msg_id, text)
                     else:
                         if msg_id:
                             contact.retract(msg_id)
@@ -211,115 +199,112 @@
                                 "/me tried to remove a message, but slidge got in trouble"
                             )
         elif isinstance(event, skpy.SkypeChatUpdateEvent):
             if log.isEnabledFor(logging.DEBUG):
                 log.debug("chat update: %s", pprint.pformat(vars(event)))
         elif isinstance(event, skpy.SkypePresenceEvent):
             if event.userId != self.sk.userId:
-                self.contacts.by_legacy_id(event.userId).update_presence(event.status)
+                (await self.contacts.by_legacy_id(event.userId)).update_presence(
+                    event.status
+                )
 
         # No 'contact has read' event :( https://github.com/Terrance/SkPy/issues/206
-        await self.async_wrap(event.ack)
+        await asyncio.to_thread(event.ack)
 
-    async def send_text(self, t: str, c: LegacyContact, *, reply_to_msg_id=None):
-        chat = self.sk.contacts[c.legacy_id].chat
+    async def send_text(self, text: str, chat: LegacyContact, **k):
+        skype_chat = self.sk.contacts[chat.legacy_id].chat
         self.send_lock.acquire()
-        msg = await self.async_wrap(chat.sendMsg, t)
+        msg = await asyncio.to_thread(skype_chat.sendMsg, text)
         if log.isEnabledFor(logging.DEBUG):
             log.debug("Sent msg: %s", pprint.pformat(vars(msg)))
         future = asyncio.Future[skpy.SkypeMsg]()
         self.sent_by_user_to_ack[msg.clientId] = future
         self.send_lock.release()
         skype_msg = await future
         return skype_msg.clientId
 
     async def logout(self):
         if self.thread is not None:
             self.thread.stop()
             self.thread.join()
 
-    async def send_file(self, u: str, c: LegacyContact, *, reply_to_msg_id=None):
+    async def send_file(self, url: str, chat: LegacyContact, **kwargs):
         async with aiohttp.ClientSession() as session:
-            async with session.get(u) as response:
+            async with session.get(url) as response:
                 file_bytes = await response.read()
-        fname = u.split("/")[-1]
+        fname = url.split("/")[-1]
         fname_lower = fname.lower()
-        await self.async_wrap(
-            self.sk.contacts[c.legacy_id].chat.sendFile,
+        await asyncio.to_thread(
+            self.sk.contacts[chat.legacy_id].chat.sendFile,
             io.BytesIO(file_bytes),
             fname,
             any(fname_lower.endswith(x) for x in (".png", ".jpg", ".gif", ".jpeg")),
         )
 
     async def active(self, c: LegacyContact):
         pass
 
     async def inactive(self, c: LegacyContact):
         pass
 
     async def composing(self, c: LegacyContact):
-        self.xmpp.executor.submit(self.sk.contacts[c.legacy_id].chat.setTyping, True)
+        await asyncio.to_thread(self.sk.contacts[c.legacy_id].chat.setTyping, True)
 
     async def paused(self, c: LegacyContact):
-        self.xmpp.executor.submit(self.sk.contacts[c.legacy_id].chat.setTyping, False)
+        await asyncio.to_thread(self.sk.contacts[c.legacy_id].chat.setTyping, False)
 
     async def displayed(self, legacy_msg_id: int, c: LegacyContact):
         try:
             skype_msg = self.unread_by_user.pop(legacy_msg_id)
         except KeyError:
             log.debug(
                 "We did not transmit: %s (%s)", legacy_msg_id, self.unread_by_user
             )
         else:
             log.debug("Calling read on %s", skype_msg)
             try:
-                await self.async_wrap(skype_msg.read)
+                await asyncio.to_thread(skype_msg.read)
             except skpy.SkypeApiException as e:
                 # FIXME: this raises HTTP 400 and does not mark the message as read
                 # https://github.com/Terrance/SkPy/issues/207
                 self.log.debug("Skype read marker failed: %r", e)
 
     async def correct(self, text: str, legacy_msg_id: Any, c: Contact):
-        try:
-            m = self.get_msg(legacy_msg_id, c)
-        except RuntimeError:
-            raise XMPPError("not-found")
-        else:
-            self.xmpp.executor.submit(m.edit, text)
+        m = self.get_msg(legacy_msg_id, c)
+        await asyncio.to_thread(m.edit, text)
 
     async def retract(self, legacy_msg_id: Any, c: Contact):
-        try:
-            m = self.get_msg(legacy_msg_id, c)
-        except RuntimeError:
-            raise XMPPError("not-found")
-        else:
-            log.debug("Deleting %s", m)
-            self.xmpp.executor.submit(m.delete)
+        m = self.get_msg(legacy_msg_id, c)
+        log.debug("Deleting %s", m)
+        await asyncio.to_thread(m.delete)
 
     async def search(self, form_values: dict[str, str]):
         pass
 
     def get_msg(self, legacy_msg_id: int, contact: Contact) -> skpy.SkypeTextMsg:
         for m in self.sk.contacts[contact.legacy_id].chat.getMsgs():
             log.debug("Message %r vs %r : %s", legacy_msg_id, m.clientId, m)
             if m.clientId == legacy_msg_id:
                 return m
         else:
-            raise RuntimeError("Could not find message ID")
+            raise XMPPError(
+                "item-not-found", text=f"Could not find message '{legacy_msg_id}'"
+            )
 
 
-def handle_thread_exception(args):
-    # TODO: establish what exceptions are OK (eg temporary network failures)
-    #       and which one should trigger killing the session and/or exiting slidge
-    #       and/or relogging in
-    log.error("Exception in thread: %s", args)
-    if (thread := getattr(args, "thread")) is not None:
-        if isinstance(thread, ListenThread):
-            session = thread.session
-            log.warning("Attempting re-login for %s", session.user)
-            thread.stop()
-            session.re_login()
+def handle_thread_exception(args: threading.ExceptHookArgs):
+    if (
+        (thread := getattr(args, "thread"))
+        and isinstance(thread, ListenThread)
+        and args.exc_type is ConnectionError
+    ):
+        session = thread.session
+        log.info("Connection error, attempting re-login for %s", session.user)
+        thread.stop()
+        session.re_login()
+    else:
+        log.error("Exception in thread: %s", args)
 
 
 threading.excepthook = handle_thread_exception
 
 log = logging.getLogger(__name__)
```

### Comparing `slidge-0.1.0b2/slidge/plugins/steam.py` & `slidge-0.1.0rc1/slidge/plugins/steam.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,47 +8,104 @@
 
 Asyncsteampy https://github.com/somespecialone/asyncsteampy
 might be interesting as it uses python's asyncio BUT the
 login process seem a little too exotic for my taste.
 """
 import asyncio
 from collections import defaultdict
-from typing import Any
+from functools import partial
+from typing import Any, Callable, Optional
 
 import steam.enums
+from slixmpp import JID
+from slixmpp.exceptions import XMPPError
 from steam.client import SteamClient
 from steam.client.user import SteamUser
 from steam.core.msg import MsgProto
 from steam.enums.common import EPersonaState, EResult
 from steam.enums.emsg import EMsg
 from steam.protobufs.steammessages_friendmessages_pb2 import (
     k_EMessageReactionType_Emoticon,
 )
 from steam.steamid import SteamID
 
 from slidge import *
+from slidge.core.adhoc import RegistrationType, TwoFactorNotRequired
 from slidge.util import BiDict
 
 
 class Gateway(BaseGateway["Session"]):
     REGISTRATION_INSTRUCTIONS = "Enter steam credentials"
     REGISTRATION_FIELDS = [
         FormField(var="username", label="Steam username", required=True),
         FormField(var="password", label="Password", private=True, required=True),
     ]
+    REGISTRATION_TYPE = RegistrationType.TWO_FACTOR_CODE
 
     ROSTER_GROUP = "Steam"
 
     COMPONENT_NAME = "Steam (slidge)"
     COMPONENT_TYPE = "steam"
 
     COMPONENT_AVATAR = "https://logos-download.com/wp-content/uploads/2016/05/Steam_icon_logo_logotype.png"
 
+    def __init__(self):
+        super().__init__()
+        self._pending_registrations = dict[str, tuple[SteamClient, EResult]]()
+        # we store logged clients on registration to get it
+        self.steam_clients = dict[str, SteamClient]()
+
+    async def validate(
+        self, user_jid: JID, registration_form: dict[str, Optional[str]]
+    ):
+        username = registration_form["username"]
+        password = registration_form["password"]
 
-class Contact(LegacyContact["Session"]):
+        store_dir = global_config.HOME_DIR / user_jid.bare
+        store_dir.mkdir(exist_ok=True)
+
+        client = SteamClient()
+        client.set_credential_location(store_dir)
+
+        login_result = client.login(username, password)
+        if login_result == EResult.InvalidPassword:
+            raise ValueError("Invalid password")
+        elif login_result == EResult.OK:
+            self.steam_clients[user_jid.bare] = client
+            raise TwoFactorNotRequired
+        elif login_result in (
+            EResult.AccountLogonDenied,
+            EResult.AccountLoginDeniedNeedTwoFactor,
+        ):
+            self._pending_registrations[user_jid.bare] = client, login_result
+        else:
+            raise ValueError(f"Login problem: {login_result}")
+
+    async def validate_two_factor_code(self, user: GatewayUser, code: str):
+        username = user.registration_form["username"]
+        password = user.registration_form["password"]
+
+        client, login_result = self._pending_registrations.pop(user.bare_jid)
+        if login_result == EResult.AccountLogonDenied:
+            # 2FA by mail (?)
+            login_result = client.login(username, password, auth_code=code)
+        elif login_result == EResult.AccountLoginDeniedNeedTwoFactor:
+            # steam guard (?)
+            login_result = client.login(username, password, two_factor_code=code)
+
+        if login_result != EResult.OK:
+            raise XMPPError(
+                "forbidden", etype="auth", text=f"Could not login: {login_result}"
+            )
+
+        # store the client, so it's picked up on Sessions.login(), without re-auth
+        self.steam_clients[user.bare_jid] = client
+
+
+class Contact(LegacyContact["Session", int]):
     MARKS = False
     CORRECTION = False
     RETRACTION = False
 
     def __init__(self, *a, **k):
         super().__init__(*a, **k)
         # keys = msg timestamp; vals = list of single character emoji
@@ -64,72 +121,89 @@
             self.busy()
         elif persona_state == EPersonaState.Away:
             self.away()
 
     def update_reactions(self, timestamp: int):
         self.react(timestamp, self.contact_reactions[timestamp])
 
+    async def available_emojis(self, legacy_msg_id):
+        return set(emoji_translate.values())
 
-class Roster(LegacyRoster[Contact, "Session"]):
-    @staticmethod
-    def jid_username_to_legacy_id(jid_username: str) -> int:
-        return int(jid_username)
 
+class Roster(LegacyRoster["Session", Contact, int]):
+    async def jid_username_to_legacy_id(self, jid_username: str) -> int:
+        try:
+            return int(jid_username)
+        except ValueError:
+            raise XMPPError("bad-request")
+
+    def by_steam_user(self, steam_user: SteamUser) -> asyncio.Task[Contact]:
+        return self.by_steam_id(steam_user.steam_id)
+
+    def by_steam_id(self, steam_id: SteamID) -> asyncio.Task[Contact]:
+        return self.session.xmpp.loop.create_task(self.by_legacy_id(steam_id.id))
+
+    def by_steam_user_apply(self, steam_user: SteamUser, method: Callable):
+        task = self.by_steam_user(steam_user)
+        task.add_done_callback(lambda f: method(f.result()))
+
+    def by_steam_id_apply(self, steam_id: SteamID, method: Callable):
+        task = self.by_steam_id(steam_id)
+        task.add_done_callback(lambda f: method(f.result()))
 
-class Session(BaseSession[Contact, Roster, Gateway]):
-    steam: SteamClient
-    job_futures: dict[str, asyncio.Future[Any]]
 
-    def post_init(self):
-        store_dir = self.xmpp.home_dir / self.user.bare_jid
+class Session(
+    BaseSession[
+        Gateway, int, Roster, Contact, LegacyBookmarks, LegacyMUC, LegacyParticipant
+    ]
+):
+    def __init__(self, user):
+        super().__init__(user)
+        store_dir = global_config.HOME_DIR / self.user.bare_jid
         store_dir.mkdir(exist_ok=True)
 
-        self.job_futures = {}
+        self.job_futures = dict[str, asyncio.Future[Any]]()
 
-        self.steam = SteamClient()
-        self.steam.set_credential_location(store_dir)
-        self.steam.username = self.user.registration_form["username"]
+        client = self.xmpp.steam_clients.pop(user.bare_jid, None)
+        if client is None:
+            self.steam = SteamClient()
+            self.log.debug("Creating steam client, %s", store_dir)
+            self.steam.set_credential_location(store_dir)
+        else:
+            # in case the session is created just after successful registration
+            self.log.debug("Using found client: %s - %s", client, client.logged_on)
+            self.steam = client
 
     @staticmethod
-    def xmpp_msg_id_to_legacy_msg_id(legacy_msg_id: Any) -> int:
-        return int(legacy_msg_id)
+    def xmpp_msg_id_to_legacy_msg_id(xmpp_msg_id: str):
+        return int(xmpp_msg_id)
 
     async def login(self):
-        username = self.user.registration_form["username"]
-        password = self.user.registration_form["password"]
-
-        # self.steam.on(SteamClient.EVENT_CHAT_MESSAGE, self.on_steam_msg)
         self.steam.on(EMsg.ClientPersonaState, self.on_persona_state)
         self.steam.on("FriendMessagesClient.IncomingMessage#1", self.on_friend_message)
         self.steam.on("FriendMessagesClient.MessageReaction#1", self.on_friend_reaction)
         self.steam.on(EMsg.ServiceMethodResponse, self.on_service_method_response)
 
-        login_result = self.steam.relogin()
-
-        if login_result != EResult.OK:
-            login_result = self.steam.login(username, password)
-
-            if login_result == EResult.AccountLogonDenied:  # 2FA
-                code = await self.input("Enter the code you received by email")
-                login_result = self.steam.login(
-                    self.user.registration_form["username"],
-                    self.user.registration_form["password"],
-                    auth_code=code,
-                )
+        if not self.steam.logged_on:
+            # if just after registration, we're already logged on
+            self.log.debug("Client is not logged on")
+            login_result = self.steam.login(
+                self.user.registration_form["username"],
+                self.user.registration_form["password"],
+            )
+            self.log.debug("Re-login result: %s", login_result)
 
-        self.log.debug("Login result: %s", login_result)
-        if login_result == EResult.OK:
-            self.log.debug("Login success")
-        else:
-            raise RuntimeError("Could not connect to steam")
+            if login_result == EResult.OK:
+                self.log.debug("Login success")
+            else:
+                raise RuntimeError("Could not connect to steam")
 
         for f in self.steam.friends:
-            f: SteamUser
             self.log.debug("Friend: %s - %s - %s", f, f.name, f.steam_id.id)
-            c = self.contacts.by_legacy_id(f.steam_id.id)
+            c = await self.contacts.by_legacy_id(f.steam_id.id)
             c.name = f.name
             c.avatar = f.get_avatar_url()
             await c.add_to_roster()
             c.update_status(f.state)
 
         asyncio.create_task(self.idle())
 
@@ -147,88 +221,103 @@
                 "Ignoring: %s vs %s", msg.header.jobid_target, self.job_futures
             )
         else:
             fut.set_result(msg.body)
 
     def on_friend_message(self, msg):
         self.log.debug("New friend message : %s", msg)
+        steam_user = self.steam.get_user(msg.body.steamid_friend)
         if (type_ := msg.body.chat_entry_type) == steam.enums.EChatEntryType.Typing:
-            user = self.steam.get_user(msg.body.steamid_friend)
-            self.contacts.by_legacy_id(user.steam_id.id).composing()
+            self.contacts.by_steam_user_apply(steam_user, Contact.composing)
         elif type_ == steam.enums.EChatEntryType.ChatMsg:
-            user = self.steam.get_user(msg.body.steamid_friend)
-            self.contacts.by_legacy_id(user.steam_id.id).send_text(
-                msg.body.message, legacy_msg_id=msg.body.rtime32_server_timestamp
+            self.contacts.by_steam_user_apply(
+                steam_user,
+                partial(
+                    Contact.send_text,
+                    body=msg.body.message,
+                    legacy_msg_id=msg.body.rtime32_server_timestamp,
+                ),
             )
 
     def on_friend_reaction(self, msg):
         self.log.debug("New friend reaction : %s", msg)
         body = msg.body
         timestamp = body.server_timestamp
+        emoji = emoji_translate.get(body.reaction) or "❓"
+
         if body.reactor == self.steam.steam_id:
             if body.reaction_type == k_EMessageReactionType_Emoticon:
-                contact = self.contacts.by_legacy_id(
-                    SteamID(msg.body.steamid_friend).id
+                contact_task = self.contacts.by_steam_id(
+                    SteamID(msg.body.steamid_friend)
                 )
-                emoji = emoji_translate.get(body.reaction)
-                if emoji is None:
-                    return
-                if body.is_add:
-                    contact.user_reactions[timestamp].add(emoji)
-                else:
-                    try:
-                        contact.user_reactions[timestamp].remove(emoji)
-                    except KeyError:
-                        self.log.warning("User removed a reaction we didn't know about")
-                contact.carbon_react(timestamp, contact.user_reactions[timestamp])
+
+                def callback(task: asyncio.Task[Contact]):
+                    c = task.result()
+                    if body.is_add:
+                        c.user_reactions[timestamp].add(emoji)
+                    else:
+                        try:
+                            c.user_reactions[timestamp].remove(emoji)
+                        except KeyError:
+                            self.log.warning(
+                                "User removed a reaction we didn't know about"
+                            )
+                    c.react(timestamp, c.user_reactions[timestamp], carbon=True)
+
+                contact_task.add_done_callback(callback)
         else:
             if body.reaction_type == k_EMessageReactionType_Emoticon:
-                contact = self.contacts.by_legacy_id(SteamID(msg.body.reactor).id)
-                emoji = emoji_translate.get(body.reaction, "❓")
-                if body.is_add:
-                    contact.contact_reactions[timestamp].add(emoji)
-                else:
-                    try:
-                        contact.contact_reactions[timestamp].remove(emoji)
-                    except KeyError:
-                        self.log.warning(
-                            "Contact removed a reaction we didn't know about"
-                        )
-                contact.update_reactions(timestamp)
+                contact_task = self.contacts.by_steam_id(SteamID(msg.body.reactor))
+
+                def callback(task: asyncio.Task[Contact]):
+                    c = task.result()
+                    if body.is_add:
+                        c.contact_reactions[timestamp].add(emoji)
+                    else:
+                        try:
+                            c.contact_reactions[timestamp].remove(emoji)
+                        except KeyError:
+                            self.log.warning(
+                                "Contact removed a reaction we didn't know about"
+                            )
+                    c.update_reactions(timestamp)
+
+                contact_task.add_done_callback(callback)
 
     def on_persona_state(self, msg: MsgProto):
         persona_state = msg.body
         self.log.debug("New state event: %s", persona_state)
         for f in persona_state.friends:
             if f.friendid == self.steam.steam_id:
                 self.log.debug("This is me %s", self.steam.steam_id)
                 return
-            self.contacts.by_legacy_id(SteamID(f.friendid).id).update_status(
-                f.persona_state
+            self.contacts.by_steam_id_apply(
+                SteamID(f.friendid),
+                partial(Contact.update_status, persona_state=f.persona_state),
             )
 
     async def logout(self):
         pass
 
-    async def send_text(self, t: str, c: Contact, *, reply_to_msg_id=None):
-        if not t:
+    async def send_text(self, text: str, chat: Contact, **k):
+        if not text:
             return
         job_id = self.steam.send_um(
             "FriendMessages.SendMessage#1",
             {
-                "steamid": SteamID(c.legacy_id),
+                "steamid": SteamID(chat.legacy_id),
                 "chat_entry_type": steam.enums.EChatEntryType.ChatMsg,
-                "message": t,
+                "message": text,
             },
         )
         f = self.job_futures[job_id] = self.xmpp.loop.create_future()
         return (await f).server_timestamp
 
-    async def send_file(self, u: str, c: Contact, *, reply_to_msg_id=None):
-        return await self.send_text(u, c)
+    async def send_file(self, url: str, chat: Contact, **k):
+        return await self.send_text(url, chat)
 
     async def active(self, c: Contact):
         pass
 
     async def inactive(self, c: Contact):
         pass
 
@@ -254,14 +343,15 @@
         pass
 
     async def react(self, legacy_msg_id: Any, emojis: list[str], c: Contact):
         old = c.user_reactions[legacy_msg_id]
         new = set[str]()
         for emoji in emojis:
             if emoji_translate.inverse.get(emoji) is None:
+                # should not happen anymore, slidge core should  take care of that never happening
                 self.send_gateway_message(
                     f"On steam, you can only react with {' '.join(emoji_translate.values())}"
                 )
             else:
                 new.add(emoji)
 
         for emoji_char in old - new:
@@ -285,15 +375,15 @@
                     "reaction_type": k_EMessageReactionType_Emoticon,
                     "reaction": emoji_translate.inverse.get(emoji_char),
                     "is_add": True,
                 },
             )
 
         c.user_reactions[legacy_msg_id] = new
-        c.carbon_react(legacy_msg_id, new)
+        c.react(legacy_msg_id, new, carbon=True)
 
     async def retract(self, legacy_msg_id: Any, c: Contact):
         pass
 
 
 emoji_translate = BiDict[str, str](
     [
```

### Comparing `slidge-0.1.0b2/slidge/plugins/telegram/contact.py` & `slidge-0.1.0rc1/slidge/plugins/telegram/group.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,184 @@
-import asyncio
-import logging
-import time
-from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Union
+from datetime import datetime, timezone
+from typing import TYPE_CHECKING, Optional
 
 import aiotdlib.api as tgapi
+from slixmpp import JID
+from slixmpp.exceptions import XMPPError
 
 from slidge import *
 
+from .util import AvailableEmojisMixin, TelegramToXMPPMixin
+
 if TYPE_CHECKING:
+    from .contact import Contact
     from .session import Session
 
 
-async def noop():
-    return
-
-
-class Contact(LegacyContact["Session"]):
-    legacy_id: int
-    # Telegram official clients have no XMPP presence equivalent, but a 'last seen' indication.
-    CLIENT_TYPE = "phone"
-
-    def __init__(self, *a, **k):
-        super(Contact, self).__init__(*a, **k)
-        self._online_expire_task = self.xmpp.loop.create_task(noop())
+class Bookmarks(LegacyBookmarks):
+    @staticmethod
+    async def legacy_id_to_jid_local_part(legacy_id: int):
+        return "group" + str(legacy_id)
 
     @staticmethod
-    def _format_last_seen(timestamp: Union[int, float]):
-        return f"Last seen {datetime.fromtimestamp(timestamp):%A %H:%M GMT}"
+    async def jid_local_part_to_legacy_id(local_part: str):
+        return int(local_part.replace("group", ""))
 
-    async def _expire_online(self, timestamp: Union[int, float]):
-        now = time.time()
-        how_long = timestamp - now
-        log.debug("Online status expires in %s seconds", how_long)
-        await asyncio.sleep(how_long)
-        self.away(self._format_last_seen(now))
-
-    def update_status(self, status: tgapi.UserStatus):
-        if isinstance(status, tgapi.UserStatusEmpty):
-            self.inactive()
-            self.offline()
-        elif isinstance(status, tgapi.UserStatusLastMonth):
-            self.inactive()
-            self.extended_away("Offline since last month")
-        elif isinstance(status, tgapi.UserStatusLastWeek):
-            self.inactive()
-            self.extended_away("Offline since last week")
-        elif isinstance(status, tgapi.UserStatusOffline):
-            self.inactive()
-            if self._online_expire_task.done():
-                # we've never seen the contact online, so we use the was_online timestamp
-                self.away(self._format_last_seen(status.was_online))
-        elif isinstance(status, tgapi.UserStatusOnline):
-            self.online()
-            self.active()
-            self._online_expire_task.cancel()
-            self._online_expire_task = self.xmpp.loop.create_task(
-                self._expire_online(status.expires)
-            )
-        elif isinstance(status, tgapi.UserStatusRecently):
-            self.inactive()
-            self.away("Last seen recently")
 
-    async def send_tg_message(self, msg: tgapi.Message):
+class MUC(LegacyMUC["Session", int, "Participant", int], AvailableEmojisMixin):
+    MAX_SUPER_GROUP_PARTICIPANTS = 200
+    session: "Session"
+    name = "unnamed"
+
+    async def join(self, join_presence):
+        self.user_nick = await self.session.my_name
+        await self.update_subject_from_msg()
+        await super().join(join_presence)
+
+    async def update_subject_from_msg(self, msg: Optional[tgapi.Message] = None):
+        if msg is None:
+            try:
+                msg = await self.session.tg.api.get_chat_pinned_message(self.legacy_id)
+                self.log.debug("Pinned message: %s", type(msg.content))
+            except tgapi.NotFound:
+                self.log.debug("Pinned message not found?")
+                return
         content = msg.content
-        if isinstance(content, tgapi.MessageText):
-            # TODO: parse formatted text to markdown
-            formatted_text = content.text
-            self.send_text(
-                body=formatted_text.text,
-                legacy_msg_id=msg.id,
-                reply_to_msg_id=msg.reply_to_message_id,
-            )
-        elif isinstance(content, tgapi.MessageAnimatedEmoji):
-            emoji = content.animated_emoji.sticker.emoji
-            self.send_text(
-                body=emoji,
-                legacy_msg_id=msg.id,
-                reply_to_msg_id=msg.reply_to_message_id,
-            )
-        elif isinstance(content, tgapi.MessagePhoto):
-            photo = content.photo
-            best_file = max(photo.sizes, key=lambda x: x.width).photo
-            await self.send_tg_file(best_file, content.caption, msg.id)
-        elif isinstance(content, tgapi.MessageVideo):
-            best_file = content.video.video
-            await self.send_tg_file(best_file, content.caption, msg.id)
-        elif isinstance(content, tgapi.MessageAnimation):
-            best_file = content.animation.animation
-            await self.send_tg_file(best_file, content.caption, msg.id)
-        else:
-            self.session.log.debug("Ignoring content: %s", type(content))
+        if not isinstance(content, (tgapi.MessagePhoto, tgapi.MessageText)):
+            return
 
-    async def send_tg_file(self, best_file, caption, msg_id):
-        query = tgapi.DownloadFile.construct(
-            file_id=best_file.id, synchronous=True, priority=1
-        )
-        best_file_downloaded: tgapi.File = await self.session.tg.request(query)
-        await self.send_file(best_file_downloaded.local.path)
-        if caption.text:
-            self.send_text(caption.text, legacy_msg_id=msg_id)
-
-    async def update_info_from_user(self, user: Optional[tgapi.User] = None):
-        if user is None:
-            user = await self.session.tg.api.get_user(self.legacy_id)
-        if username := user.username:
-            name = username
-        else:
-            name = user.first_name
-            if last := user.last_name:
-                name += " " + last
-        self.name = name
-
-        if photo := user.profile_photo:
-            if (local := photo.small.local) and (path := local.path):
-                with open(path, "rb") as f:
-                    self.avatar = f.read()
+        sender_id = msg.sender_id
+        self.subject_date = datetime.fromtimestamp(msg.date, tz=timezone.utc)
+        if isinstance(sender_id, tgapi.MessageSenderUser):
+            if sender_id.user_id == await self.session.tg.get_my_id():
+                self.subject_setter = self.user_nick
             else:
-                response = await self.session.tg.api.download_file(
-                    file_id=photo.small.id,
-                    synchronous=True,
-                    priority=1,
-                    offset=0,
-                    limit=0,
-                )
-                with open(response.local.path, "rb") as f:
-                    self.avatar = f.read()
-
-        if isinstance(user.type_, tgapi.UserTypeBot) or user.id == 777000:
-            # 777000 is not marked as bot, it's the "Telegram" contact, which gives
-            # confirmation codes and announces telegram-related stuff
-            self.CLIENT_TYPE = "bot"
-
+                contact = await self.session.contacts.by_legacy_id(sender_id.user_id)
+                self.subject_setter = contact.name
         else:
-            if user.is_contact:
-                self._subscribe_to = True
-                self._subscribe_from = user.is_mutual_contact
-            else:
-                self._subscribe_to = self._subscribe_from = False
+            self.subject_setter = self.name
 
-        self.update_status(user.status)
+        if isinstance(content, tgapi.MessagePhoto):
+            self.subject = content.caption.text
+        if isinstance(content, tgapi.MessageText):
+            self.subject = content.text.text
 
-        if p := user.phone_number:
-            phone = "+" + p
+    async def get_participants(self):
+        self.log.debug("Getting participants")
+        chat = await self.session.tg.get_chat(chat_id=self.legacy_id)
+        if not isinstance(
+            chat.type_, (tgapi.ChatTypeBasicGroup, tgapi.ChatTypeSupergroup)
+        ):
+            raise XMPPError("item-not-found", text="This is not a valid group ID")
+
+        info = await self.session.tg.get_chat_info(chat, full=True)
+        if isinstance(info, tgapi.BasicGroupFullInfo):
+            members = info.members
+        elif isinstance(info, tgapi.SupergroupFullInfo):
+            if info.can_get_members:
+                members = (
+                    await self.session.tg.api.get_supergroup_members(
+                        supergroup_id=chat.type_.supergroup_id,
+                        filter_=None,
+                        offset=0,
+                        limit=self.MAX_SUPER_GROUP_PARTICIPANTS,
+                        skip_validation=True,
+                    )
+                ).members
+            else:
+                members = []
         else:
-            phone = None
-        self.set_vcard(
-            given=user.first_name, surname=user.last_name, phone=phone, full_name=name
+            raise RuntimeError
+        self.log.debug("%s participants", len(members))
+        for member in members:
+            sender = member.member_id
+            if not isinstance(sender, tgapi.MessageSenderUser):
+                self.log.debug("Ignoring non-user sender")  # Does this happen?
+                continue
+            if sender.user_id == await self.session.tg.get_my_id():
+                continue
+            yield await self.participant_by_tg_user(
+                await self.session.tg.get_user(sender.user_id)
+            )
+
+    async def send_text(self, text: str) -> int:
+        result = await self.session.tg.send_text(self.legacy_id, text)
+        self.log.debug("MUC SEND RESULT: %s", result)
+        msg_id = await self.session.wait_for_tdlib_success(result.id)
+        self.log.debug("MUC SEND MSG: %s", msg_id)
+        return msg_id
+
+    async def participant_by_tg_user(self, user: tgapi.User) -> "Participant":
+        return await Participant.by_tg_user(self, user)
+
+    async def participant_system(self) -> "Participant":
+        return await self.get_participant("")
+
+    async def participant_by_tg_user_id(self, user_id: int) -> "Participant":
+        return await Participant.by_tg_user(
+            self, await self.session.tg.api.get_user(user_id)
         )
 
-    async def update_info_from_chat(self, chat: tgapi.Chat):
-        self.name = chat.title
-        if isinstance(chat.photo, tgapi.ChatPhotoInfo):
-            if (local := chat.photo.small.local) and (path := local.path):
-                with open(path, "rb") as f:
-                    self.avatar = f.read()
-            else:
-                response = await self.session.tg.api.download_file(
-                    file_id=chat.photo.small.id,
-                    synchronous=True,
-                    priority=1,
+    async def get_tg_chat(self):
+        return await self.session.tg.get_chat(self.legacy_id)
+
+    async def fill_history(
+        self,
+        full_jid: JID,
+        maxchars: Optional[int] = None,
+        maxstanzas: Optional[int] = None,
+        seconds: Optional[int] = None,
+        since: Optional[int] = None,
+    ):
+        for m in await self.fetch_history(50):
+            part = await self.participant_by_tg_user(
+                await self.session.tg.get_user(m.sender_id.user_id)
+            )
+            await part.send_tg_message(m, full_jid=full_jid)
+
+    async def fetch_history(self, n: int):
+        tg = self.session.tg
+        chat = await self.get_tg_chat()
+        m = chat.last_message
+        if m is None:
+            return []
+
+        messages = [chat.last_message]
+        i = 0
+        last_message_id = m.id
+        while True:
+            fetched = (
+                await tg.api.get_chat_history(
+                    chat_id=self.legacy_id,
+                    from_message_id=last_message_id,
                     offset=0,
-                    limit=0,
+                    limit=10,
+                    only_local=False,
                 )
-                with open(response.local.path, "rb") as f:
-                    self.avatar = f.read()
+            ).messages
+            if len(fetched) == 0:
+                break
+            messages.extend(fetched)
+            i += len(fetched)
+            if i > n:
+                break
+
+            last_message_id = fetched[-1].id
+
+        return reversed(messages)
+
+
+class Participant(LegacyParticipant[MUC], TelegramToXMPPMixin):
+    contact: "Contact"
+    session: "Session"  # type:ignore
 
+    def __init__(self, *a, **k):
+        super().__init__(*a, **k)
+        self.chat_id = self.muc.legacy_id
+        self.session.log.debug("PARTICIPANT-N: %s", self.muc.n_participants)
 
-class Roster(LegacyRoster["Contact", "Session"]):
     @staticmethod
-    def jid_username_to_legacy_id(jid_username: str) -> int:
-        return int(jid_username)
-
-
-log = logging.getLogger(__name__)
+    async def by_tg_user(muc: MUC, user: tgapi.User):
+        nick = " ".join((user.first_name, user.last_name)).strip()
+        p = Participant(muc, nick)
+        p.contact = await muc.session.contacts.by_legacy_id(user.id)
+        return p
```

### Comparing `slidge-0.1.0b2/slidge/plugins/telegram/gateway.py` & `slidge-0.1.0rc1/slidge/plugins/telegram/gateway.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,116 @@
+import asyncio
 import logging
 import typing
-from argparse import Namespace
 from datetime import datetime
 
 import aiotdlib.api as tgapi
 from slixmpp import JID, Iq
 from slixmpp.exceptions import XMPPError
 
 from slidge import *
+from slidge.core.adhoc import RegistrationType
 
 from ...util import is_valid_phone_number
-from .config import get_parser
+from . import config
+from .client import CredentialsValidation
 
 if typing.TYPE_CHECKING:
     from .session import Session
 
-REGISTRATION_INSTRUCTIONS = """You can visit https://my.telegram.org/apps to get an API ID and an API HASH
-
-This is the only tested login method, but other methods (password, bot token, 2FA...)
-should work too, in theory at least.
-"""
+REGISTRATION_INSTRUCTIONS = (
+    "You need to create a telegram account in an official telegram client.\n\n"
+    "Then you can enter your phone number here, and you will receive a confirmation code "
+    "in the official telegram client. "
+    "You can uninstall the telegram client after this if you want."
+)
 
 
 class Gateway(BaseGateway["Session"]):
     REGISTRATION_INSTRUCTIONS = REGISTRATION_INSTRUCTIONS
-    REGISTRATION_FIELDS = [
-        FormField(var="phone", label="Phone number", required=True),
-        FormField(var="api_id", label="API ID", required=False),
-        FormField(var="api_hash", label="API hash", required=False),
-        FormField(var="", value="The fields below have not been tested", type="fixed"),
-        FormField(var="bot_token", label="Bot token", required=False),
-        FormField(var="first", label="First name", required=False),
-        FormField(var="last", label="Last name", required=False),
-    ]
+    REGISTRATION_FIELDS = [FormField(var="phone", label="Phone number", required=True)]
+    REGISTRATION_TYPE = RegistrationType.TWO_FACTOR_CODE
     ROSTER_GROUP = "Telegram"
     COMPONENT_NAME = "Telegram (slidge)"
     COMPONENT_TYPE = "telegram"
     COMPONENT_AVATAR = "https://web.telegram.org/img/logo_share.png"
 
     SEARCH_FIELDS = [
         FormField(var="phone", label="Phone number", required=True),
         FormField(var="first", label="First name", required=True),
         FormField(var="last", label="Last name", required=False),
     ]
 
-    args: Namespace
+    GROUPS = True
 
-    def config(self, argv: list[str]):
-        Gateway.args = args = get_parser().parse_args(argv)
-        if args.tdlib_path is None:
-            args.tdlib_path = self.home_dir / "tdlib"
+    def __init__(self):
+        super().__init__()
+        if config.TDLIB_PATH is None:
+            config.TDLIB_PATH = global_config.HOME_DIR / "tdlib"
+        self._pending_registrations = dict[
+            str, tuple[asyncio.Task[CredentialsValidation], CredentialsValidation]
+        ]()
+        if not config.API_ID:
+            self.REGISTRATION_FIELDS.extend(
+                [
+                    FormField(
+                        var="info",
+                        type="fixed",
+                        label="Get API id and hash on https://my.telegram.org/apps",
+                    ),
+                    FormField(var="api_id", label="API ID", required=True),
+                    FormField(var="api_hash", label="API Hash", required=True),
+                ]
+            )
+        log.debug("CONFIG %s", vars(config))
 
     async def validate(
         self, user_jid: JID, registration_form: dict[str, typing.Optional[str]]
     ):
         phone = registration_form.get("phone")
         if not is_valid_phone_number(phone):
             raise ValueError("Not a valid phone number")
-
-    async def unregister(self, user):
-        pass
+        tg_client = CredentialsValidation(registration_form)  # type: ignore
+        auth_task = self.loop.create_task(tg_client.start())
+        self._pending_registrations[user_jid.bare] = auth_task, tg_client
+
+    async def validate_two_factor_code(self, user: GatewayUser, code: str):
+        auth_task, tg_client = self._pending_registrations.pop(user.bare_jid)
+        tg_client.code_future.set_result(code)
+        try:
+            await asyncio.wait_for(auth_task, config.REGISTRATION_AUTH_CODE_TIMEOUT)
+        except asyncio.TimeoutError:
+            raise XMPPError(
+                "not-authorized",
+                text="Something went wrong when trying to authenticate you on the "
+                "telegram network. Please retry and/or contact your slidge admin.",
+            )
+        await tg_client.stop()
+
+    async def unregister(self, user: GatewayUser):
+        session = self.session_cls.from_user(user)
+        # FIXME: this effectively removes user data from disk, but crashes slidge.
+        await session.tg.start()
+        await session.tg.api.log_out()
 
     def add_adhoc_commands(self):
-        self["xep_0050"].add_command(
+        self.adhoc.add_command(
             node="get_sessions",
             name="List active sessions",
             handler=self.adhoc_active_sessions1,
+            only_users=True,
         )
 
     async def adhoc_active_sessions1(
         self, iq: Iq, adhoc_session: dict[str, typing.Any]
     ):
         user = user_store.get_by_stanza(iq)
         if user is None:
             raise XMPPError("subscription-required")
-        session = self._session_cls.from_stanza(iq)
+        session = self.session_cls.from_stanza(iq)
 
         form = self["xep_0004"].make_form("form", "Active telegram sessions")
         tg_sessions = (await session.tg.api.get_active_sessions()).sessions
         form.add_field(
             "tg_session_id",
             ftype="list-single",
             label="Sessions",
```

### Comparing `slidge-0.1.0b2/slidge/plugins/telegram/session.py` & `slidge-0.1.0rc1/slidge/plugins/telegram/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,169 +1,203 @@
 import asyncio
+import functools
 import logging
 import re
 import tempfile
 from mimetypes import guess_type
-from pathlib import Path
-from typing import Optional
+from typing import Union
 
 import aiohttp
 import aiotdlib.api as tgapi
 from aiotdlib.api.errors import BadRequest
 from slixmpp.exceptions import XMPPError
 
 from slidge import *
 
+from ...util.types import Chat
+from . import config
 from .client import TelegramClient
 from .contact import Contact, Roster
 from .gateway import Gateway
+from .group import MUC
 
 
-class Session(BaseSession[Contact, Roster, Gateway]):
-    tdlib_path: Optional[Path] = None
-    tg: TelegramClient
-    sent_read_marks: set[int]
-    ack_futures: dict[int, asyncio.Future]
-    user_correction_futures: dict[int, asyncio.Future]
-    delete_futures: dict[int, asyncio.Future]
-
-    def post_init(self):
-        registration_form = {
-            k: v if v != "" else None for k, v in self.user.registration_form.items()
-        }
-        self.sent_read_marks = set()
-        self.ack_futures = {}
-        self.user_correction_futures = {}
-        self.delete_futures = {}
-
-        i = registration_form.get("api_id")
-        if i is not None:
-            i = int(i)  # makes testing easier to make api_id optional...
-
-        self.tg = TelegramClient(
-            self,
-            api_id=i,
-            api_hash=registration_form.get("api_hash"),
-            phone_number=registration_form["phone"],
-            bot_token=registration_form.get("bot_token"),
-            first_name=registration_form.get("first"),
-            last_name=registration_form.get("last"),
-            database_encryption_key=Gateway.args.tdlib_key,
-            files_directory=Gateway.args.tdlib_path,
-        )
+def catch_chat_not_found(coroutine):
+    @functools.wraps(coroutine)
+    async def wrapped(*a, **k):
+        try:
+            return await coroutine(*a, **k)
+        except tgapi.BadRequest as e:
+            if e.code == 400:
+                raise XMPPError(condition="item-not-found", text="Recipient not found")
+            else:
+                raise
+
+    return wrapped
+
+
+class Session(
+    BaseSession[Gateway, int, Roster, Contact, LegacyBookmarks, MUC, LegacyParticipant]
+):
+    def __init__(self, user):
+        super().__init__(user)
+        self.sent_read_marks = set[int]()
+        self.ack_futures = dict[int, asyncio.Future]()
+        self.user_correction_futures = dict[int, asyncio.Future]()
+        self.delete_futures = dict[int, asyncio.Future]()
+
+        self.my_name: asyncio.Future[str] = self.xmpp.loop.create_future()
+
+        self.tg = TelegramClient(self)
 
     @staticmethod
     def xmpp_msg_id_to_legacy_msg_id(i: str) -> int:
-        try:
-            return int(i)
-        except ValueError:
-            raise NotImplementedError("This is not a valid telegram msg ID")
+        return int(i)
 
     async def login(self):
         await self.tg.start()
         await self.add_contacts_to_roster()
-        return f"Connected as {await self.tg.get_my_id()}"
+        await self.add_groups()
+        me = await self.tg.get_user(await self.tg.get_my_id())
+        my_name = (me.first_name + " " + me.last_name).strip()
+        self.my_name.set_result(my_name)
+        return f"Connected as {my_name}"
 
     async def logout(self):
         await self.tg.stop()
 
     async def wait_for_tdlib_success(self, result_id: int):
         fut = self.xmpp.loop.create_future()
         self.ack_futures[result_id] = fut
         return await fut
 
-    async def send_text(self, t: str, c: "Contact", *, reply_to_msg_id=None) -> int:
-        t = escape(t)
-        try:
-            result = await self.tg.send_text(
-                chat_id=c.legacy_id, text=t, reply_to_message_id=reply_to_msg_id
-            )
-        except tgapi.BadRequest as e:
-            if e.code == 400:
-                raise XMPPError(condition="item-not-found", text="No such contact")
-            else:
-                raise
+    @catch_chat_not_found
+    async def send_text(
+        self,
+        text: str,
+        chat: Union[Contact, MUC],
+        *,
+        reply_to_msg_id=None,
+        reply_to_fallback_text=None,
+        reply_to=None,
+        **kwargs,
+    ) -> int:
+        text = escape(text)
+        result = await self.tg.send_text(
+            chat_id=chat.legacy_id, text=text, reply_to_message_id=reply_to_msg_id
+        )
         new_message_id = await self.wait_for_tdlib_success(result.id)
         self.log.debug("Result: %s / %s", result, new_message_id)
         return new_message_id
 
-    async def send_file(self, u: str, c: "Contact", *, reply_to_msg_id=None) -> int:
-        type_, _ = guess_type(u)
+    @catch_chat_not_found
+    async def send_file(
+        self,
+        url: str,
+        chat: Chat,
+        reply_to_msg_id=None,
+        **kwargs,
+    ) -> int:
+        type_, _ = guess_type(url)
         if type_ is not None:
             type_, subtype = type_.split("/")
 
         async with aiohttp.ClientSession() as session:
-            async with session.get(u) as response:
+            async with session.get(url) as response:
                 response.raise_for_status()
+                kwargs = dict(
+                    chat_id=chat.legacy_id, reply_to_message_id=reply_to_msg_id
+                )
                 with tempfile.NamedTemporaryFile() as file:
                     bytes_ = await response.read()
                     file.write(bytes_)
                     if type_ == "image":
-                        result = await self.tg.send_photo(
-                            chat_id=c.legacy_id, photo=file.name
-                        )
+                        result = await self.tg.send_photo(photo=file.name, **kwargs)
                     elif type_ == "video":
-                        result = await self.tg.send_video(
-                            chat_id=c.legacy_id, video=file.name
-                        )
+                        result = await self.tg.send_video(video=file.name, **kwargs)
+                    elif type_ == "audio":
+                        result = await self.tg.send_audio(audio=file.name, **kwargs)
                     else:
                         result = await self.tg.send_document(
-                            c.legacy_id, document=file.name
+                            document=file.name, **kwargs
                         )
 
         return result.id
 
+    @catch_chat_not_found
     async def active(self, c: "Contact"):
         res = await self.tg.api.open_chat(chat_id=c.legacy_id)
         self.log.debug("Open chat res: %s", res)
 
+    @catch_chat_not_found
     async def inactive(self, c: "Contact"):
         res = await self.tg.api.close_chat(chat_id=c.legacy_id)
         self.log.debug("Close chat res: %s", res)
 
+    @catch_chat_not_found
     async def composing(self, c: "Contact"):
         res = await self.tg.api.send_chat_action(
             chat_id=c.legacy_id,
             action=tgapi.ChatActionTyping(),
             message_thread_id=0,  # TODO: check what telegram's threads really are
         )
         self.log.debug("Send composing res: %s", res)
 
     async def paused(self, c: "Contact"):
         pass
 
+    @catch_chat_not_found
     async def displayed(self, tg_id: int, c: "Contact"):
         res = await self.tg.api.view_messages(
             chat_id=c.legacy_id,
             message_thread_id=0,
             message_ids=[tg_id],
             force_read=True,
         )
         self.log.debug("Send chat action res: %s", res)
 
+    @catch_chat_not_found
     async def add_contacts_to_roster(self):
         users = await self.tg.api.get_contacts()
         for id_ in users.user_ids:
-            contact = self.contacts.by_legacy_id(id_)
+            contact = await self.contacts.by_legacy_id(id_)
             await contact.add_to_roster()
             await contact.update_info_from_user()
 
+    async def add_groups(self):
+        for chat in await self.tg.get_main_list_chats_all():
+            if isinstance(chat.type_, tgapi.ChatTypeBasicGroup):
+                muc = await self.bookmarks.by_legacy_id(chat.id)
+                group = await self.tg.get_basic_group(chat.type_.basic_group_id)
+                muc.type = MucType.GROUP
+            elif isinstance(chat.type_, tgapi.ChatTypeSupergroup):
+                muc = await self.bookmarks.by_legacy_id(chat.id)
+                group = await self.tg.get_supergroup(chat.type_.supergroup_id)
+                muc.type = MucType.CHANNEL
+            else:
+                continue
+
+            muc.n_participants = group.member_count
+            muc.DISCO_NAME = chat.title
+
+    @catch_chat_not_found
     async def correct(self, text: str, legacy_msg_id: int, c: "Contact"):
         f = self.user_correction_futures[legacy_msg_id] = self.xmpp.loop.create_future()
         await self.tg.api.edit_message_text(
             chat_id=c.legacy_id,
             message_id=legacy_msg_id,
             reply_markup=None,
             input_message_content=tgapi.InputMessageText.construct(
                 text=tgapi.FormattedText.construct(text=text)
             ),
             skip_validation=True,
         )
         await f
 
+    @catch_chat_not_found
     async def search(self, form_values: dict[str, str]):
         phone = form_values["phone"]
         first = form_values.get("first", phone)
         last = form_values.get("last", "")
         response = await self.tg.api.import_contacts(
             contacts=[
                 tgapi.Contact(
@@ -176,72 +210,57 @@
             ]
         )
         user_id = response.user_ids[0]
         if user_id == 0:
             return
 
         await self.add_contacts_to_roster()
-        contact = self.contacts.by_legacy_id(user_id)
+        contact = await self.contacts.by_legacy_id(user_id)
         await contact.update_info_from_user()
         await contact.add_to_roster()
 
         return SearchResult(
             fields=[FormField("phone"), FormField("jid", type="jid-single")],
             items=[{"phone": form_values["phone"], "jid": contact.jid.bare}],
         )
 
+    @catch_chat_not_found
     async def remove_reactions(self, legacy_msg_id, c: "Contact"):
         try:
             r = await self.tg.api.set_message_reaction(
                 chat_id=c.legacy_id,
                 message_id=legacy_msg_id,
                 reaction="",
                 is_big=False,
             )
         except BadRequest as e:
             self.log.debug("Remove reaction error: %s", e)
         else:
             self.log.debug("Remove reaction response: %s", r)
 
-    async def react(self, legacy_msg_id, emojis, c: "Contact"):
+    @catch_chat_not_found
+    async def react(self, legacy_msg_id: int, emojis: list[str], c: "Contact"):
         if len(emojis) == 0:
             await self.remove_reactions(legacy_msg_id, c)
             return
 
-        if len(emojis) > 1:
-            c.carbon_react(legacy_msg_id)
-            await self.remove_reactions(legacy_msg_id, c)
-            self.send_gateway_message(
-                "Warning: unlike XMPP, telegram only accepts one reaction per message. "
-                f"Your reactions have been removed."
-            )
-            return
-
-        emoji = emojis[-1]
-
+        # we never have more than 1 emoji, slidge core makes sure of that
         try:
             r = await self.tg.api.set_message_reaction(
                 chat_id=c.legacy_id,
                 message_id=legacy_msg_id,
-                reaction=emoji,
+                reaction=emojis[0],
                 is_big=False,
             )
         except BadRequest as e:
-            available = await self.tg.api.get_message_available_reactions(
-                chat_id=c.legacy_id, message_id=legacy_msg_id
-            )
-            available_emojis = [a.reaction for a in available.reactions]
-            self.send_gateway_message(
-                "Error: unlike XMPP, telegram does not allow arbitrary emojis to be used as reactions: "
-                f"{e.message}. Please pick your reaction in this list: {' '.join(available_emojis)}"
-            )
-            c.carbon_react(legacy_msg_id)
+            raise XMPPError("bad-request", text=e.message)
         else:
             self.log.debug("Message reaction response: %s", r)
 
+    @catch_chat_not_found
     async def retract(self, legacy_msg_id, c):
         f = self.delete_futures[legacy_msg_id] = self.xmpp.loop.create_future()
         r = await self.tg.api.delete_messages(c.legacy_id, [legacy_msg_id], revoke=True)
         self.log.debug("Delete message response: %s", r)
         confirmation = await f
         self.log.debug("Message delete confirmation: %s", confirmation)
```

### Comparing `slidge-0.1.0b2/slidge/util/db.py` & `slidge-0.1.0rc1/slidge/util/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """
 This module covers a backend for storing user data persistently and managing a
 pseudo-roster for the gateway component.
 """
 
 import dataclasses
+import datetime
 import logging
 import os.path
 import shelve
 from io import BytesIO
 from os import PathLike
 from typing import Iterable, Optional, Union
 
 from pickle_secure import Pickler, Unpickler
 from slixmpp import JID, Iq, Message, Presence
 
 
 # noinspection PyUnresolvedReferences
 class EncryptedShelf(shelve.DbfilenameShelf):
+    cache: dict
+    dict: dict
+    writeback: bool
+    keyencoding: str
+    _protocol: int
+
     def __init__(
         self, filename: PathLike, key: str, flag="c", protocol=None, writeback=False
     ):
         super().__init__(str(filename), flag, protocol, writeback)
         self.secret_key = key
 
     def __getitem__(self, key):
@@ -48,21 +55,27 @@
     A dataclass representing a gateway user
     """
 
     bare_jid: str
     """Bare JID of the user"""
     registration_form: dict[str, Optional[str]]
     """Content of the registration form, as a dict"""
+    plugin_data: Optional[dict] = None
+    registration_date: Optional[datetime.datetime] = None
 
     def __hash__(self):
         return hash(self.bare_jid)
 
     def __repr__(self):
         return f"<User {self.bare_jid}>"
 
+    def __post_init__(self):
+        if self.registration_date is None:
+            self.registration_date = datetime.datetime.now()
+
     @property
     def jid(self) -> JID:
         """
         The user's (bare) JID
 
         :return:
         """
@@ -75,14 +88,17 @@
         :param field: Name of the field
         :param default: Default value to return if the field is not present
 
         :return: Value of the field
         """
         return self.registration_form.get(field, default)
 
+    def commit(self):
+        user_store.commit(self)
+
 
 class UserStore:
     """
     Basic user store implementation using shelve from the python standard library
 
     Set_file must be called before it is usable
     """
@@ -127,23 +143,28 @@
         :param jid: JID of the gateway user
         :param registration_form: Content of the registration form (:xep:`0077`)
         """
         log.debug("Adding user %s", jid)
         self._users[jid.bare] = GatewayUser(
             bare_jid=jid.bare,
             registration_form=registration_form,
+            registration_date=datetime.datetime.now(),
         )
         self._users.sync()
         log.debug("Store: %s", self._users)
 
+    def commit(self, user: GatewayUser):
+        self._users[user.bare_jid] = user
+        self._users.sync()
+
     def get(self, _gateway_jid, _node, ifrom: JID, iq) -> Optional[GatewayUser]:
         """
         Get a user from the store
 
-        NB: there is no reason to call this, it is used by SliXMPP plugins
+        NB: there is no reason to call this, it is used by SliXMPP internal API
 
         :param _gateway_jid:
         :param _node:
         :param ifrom:
         :param iq:
         :return:
         """
@@ -152,23 +173,25 @@
         log.debug("Getting user %s", ifrom.bare)
         return self._users.get(ifrom.bare)
 
     def remove(self, _gateway_jid, _node, ifrom: JID, _iq):
         """
         Remove a user from the store
 
-        NB: there is no reason to call this, it is used by SliXMPP plugins
+        NB: there is no reason to call this, it is used by SliXMPP internal API
+        """
+        self.remove_by_jid(ifrom)
 
-        :param _gateway_jid:
-        :param _node:
-        :param ifrom:
-        :param _iq:
+    def remove_by_jid(self, jid: JID):
         """
-        log.debug("Removing user %s", ifrom.bare)
-        del self._users[ifrom.bare]
+        Remove a user from the store, by JID
+        """
+        j = jid.bare
+        log.debug("Removing user %s", j)
+        del self._users[j]
         self._users.sync()
 
     def get_by_jid(self, jid: JID) -> Optional[GatewayUser]:
         """
         Convenience function to get a user from their JID.
 
         :param jid: JID of the gateway user
@@ -181,14 +204,18 @@
         Convenience function to get a user from a stanza they sent.
 
         :param s: A stanza sent by the gateway user
         :return:
         """
         return self.get_by_jid(s.get_from())
 
+    def close(self):
+        self._users.sync()
+        self._users.close()
+
 
 class YesSet(set):
     """
     A pseudo-set which always test True for membership
     """
 
     def __contains__(self, item):
```

### Comparing `slidge-0.1.0b2/slidge/util/util.py` & `slidge-0.1.0rc1/slidge/util/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 import dataclasses
 import logging
 import re
 from abc import ABCMeta
-from typing import Generic, Iterable, Literal, Optional, TypeVar
+from typing import Collection, Generic, Optional, TypeVar
 
-field_type = Literal[
-    "boolean",
-    "fixed",
-    "text-single",
-    "jid-single",
-    "list-single",
-    "list-multi",
-    "text-private",
-]
+from .types import FieldType
 
 
 @dataclasses.dataclass
 class FormField:
     """
     Represents a field of the form that a user will see when registering to the gateway
     via their XMPP client.
@@ -31,33 +23,33 @@
     required: bool = False
     """Whether this field is mandatory or not"""
     private: bool = False
     """
     For sensitive info that should not be displayed on screen while the user types.
     Forces field_type to "text-private"
     """
-    type: field_type = "text-single"
+    type: FieldType = "text-single"
     """Type of the field, see `XEP-0004 <https://xmpp.org/extensions/xep-0004.html#protocol-fieldtypes>`_"""
     value: str = ""
     """Pre-filled value. Will be automatically pre-filled if a registered user modifies their subscription"""
     options: Optional[list[dict[str, str]]] = None
 
     def dict(self):
         return dataclasses.asdict(self)
 
     def __post_init__(self):
         if self.private:
             self.type = "text-private"
 
 
-KeyType = TypeVar("KeyType")  # FIXME: mypy does not correctly infer types with this...
+KeyType = TypeVar("KeyType")
 ValueType = TypeVar("ValueType")
 
 
-class BiDict(Generic[KeyType, ValueType], dict):
+class BiDict(Generic[KeyType, ValueType], dict[KeyType, ValueType]):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.inverse: dict[ValueType, KeyType] = {}
         for key, value in self.items():
             self.inverse[value] = key
 
     def __setitem__(self, key: KeyType, value: ValueType):
@@ -65,16 +57,16 @@
             del self.inverse[self[key]]
         super().__setitem__(key, value)
         self.inverse[value] = key
 
 
 @dataclasses.dataclass
 class SearchResult:
-    fields: Iterable[FormField]
-    items: Iterable[dict[str, str]]
+    fields: Collection[FormField]
+    items: Collection[dict[str, str]]
 
 
 class SubclassableOnce(type):
     TEST_MODE = False  # To allow importing everything, including plugins, during tests
 
     def __init__(cls, name, bases, dct):
         for b in bases:
```

### Comparing `slidge-0.1.0b2/slidge/util/xep_0030/disco.py` & `slidge-0.1.0rc1/slidge/util/xep_0030/disco.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,29 +295,29 @@
                 'itype': itype,
                 'lang': lang,
                 'local': local,
                 'cached': cached}
         return self.api['has_identity'](jid, node, ifrom, data)
 
     async def get_info_from_domain(self, domain=None, timeout=None,
-                                   cached=True, callback=None):
+                                   cached=True, callback=None, **iqkwargs):
         """Fetch disco#info of specified domain and one disco#items level below
         """
 
         if domain is None:
             domain = self.xmpp.boundjid.domain
 
         if not cached or domain not in self.domain_infos:
             infos = [self.get_info(
-                domain, timeout=timeout)]
+                domain, timeout=timeout, **iqkwargs)]
             iq_items = await self.get_items(
                 domain, timeout=timeout)
             items = iq_items['disco_items']['items']
             infos += [
-                self.get_info(item[0], timeout=timeout)
+                self.get_info(item[0], timeout=timeout, **iqkwargs)
                 for item in items]
             info_futures, _ = await asyncio.wait(
                 infos,
                 timeout=timeout,
             )
 
             self.domain_infos[domain] = [
```

### Comparing `slidge-0.1.0b2/slidge/util/xep_0030/stanza/info.py` & `slidge-0.1.0rc1/slidge/util/xep_0030/stanza/info.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0030/stanza/items.py` & `slidge-0.1.0rc1/slidge/util/xep_0030/stanza/items.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0030/static.py` & `slidge-0.1.0rc1/slidge/util/xep_0030/static.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0077/register.py` & `slidge-0.1.0rc1/slidge/util/xep_0077/register.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Slixmpp: The Slick XMPP Library
 # Copyright (C) 2012 Nathanael C. Fritz, Lance J.T. Stout
 # This file is part of Slixmpp.
 # See the file LICENSE for copying permission.
 import logging
 import ssl
 
+from slixmpp.exceptions import XMPPError
 from slixmpp.plugins import BasePlugin
 from slixmpp.stanza import Iq, StreamFeatures
 from slixmpp.xmlstream import JID, StanzaBase, register_stanza_plugin
 from slixmpp.xmlstream.handler import CoroutineCallback
 from slixmpp.xmlstream.matcher import StanzaPath
 
 from . import stanza
@@ -63,14 +64,15 @@
     stanza = stanza
     default_config = {
         "create_account": True,
         "force_registration": False,
         "order": 50,
         "form_fields": {"username", "password"},
         "form_instructions": "Enter your credentials",
+        "enable_subscription": True,
     }
     _user_store: dict[str, dict[str, str]]
 
     def plugin_init(self):
         register_stanza_plugin(StreamFeatures, RegisterFeature)
         register_stanza_plugin(Iq, Register)
 
@@ -143,14 +145,19 @@
     def _user_modify(self, _jid, _node, ifrom, registration):
         self._user_store[ifrom.bare] = {
             key: registration[key] for key in self.form_fields
         }
 
     async def _handle_registration(self, iq: StanzaBase):
         if iq["type"] == "get":
+            if not self.enable_subscription:
+                raise XMPPError(
+                    "bad-request",
+                    text="You must use adhoc commands to register to this gateway.",
+                )
             await self._send_form(iq)
         elif iq["type"] == "set":
             form_dict = iq["register"]["form"].get_values() or iq["register"]
 
             if form_dict.get("remove"):
                 try:
                     await self.api["user_remove"](None, None, iq["from"], iq)
@@ -164,14 +171,20 @@
                     )
                 else:
                     reply = iq.reply()
                     reply.send()
                     self.xmpp.event("user_unregister", iq)
                 return
 
+            if not self.enable_subscription:
+                raise XMPPError(
+                    "bad-request",
+                    text="You must use adhoc commands to register to this gateway.",
+                )
+
             if self.form_fields is not None:
                 for field in self.form_fields:
                     if not iq["register"][field]:
                         # Incomplete Registration
                         _send_error(
                             iq,
                             "406",
```

### Comparing `slidge-0.1.0b2/slidge/util/xep_0077/stanza.py` & `slidge-0.1.0rc1/slidge/util/xep_0077/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0100/gateway.py` & `slidge-0.1.0rc1/slidge/util/xep_0100/gateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import logging
 
-from slixmpp import JID, Iq, Message, Presence
+from slixmpp import JID, Iq, Message, Presence, register_stanza_plugin
 from slixmpp.plugins.base import BasePlugin
 
+from slidge.core import config
+
+from . import stanza
+
 log = logging.getLogger(__name__)
 
 
 class XEP_0100(BasePlugin):
     name = "xep_0100"
     description = "XEP-0100: Gateway interaction (slidge)"
     dependencies = {
@@ -38,14 +42,16 @@
         self.xmpp.add_event_handler("user_unregister", self.on_user_unregister)
         self.xmpp.add_event_handler(
             "presence_unsubscribe", self.on_presence_unsubscribe
         )
 
         self.xmpp.add_event_handler("message", self.on_message)
 
+        register_stanza_plugin(Iq, stanza.Gateway)
+
     def plugin_end(self):
         if not self.xmpp.is_component:
             self.xmpp.remove_event_handler("user_register", self.on_user_register)
             self.xmpp.remove_event_handler("user_unregister", self.on_user_unregister)
             self.xmpp.remove_event_handler(
                 "presence_unsubscribe", self.on_presence_unsubscribe
             )
@@ -61,18 +67,15 @@
         self.xmpp.send_presence(pto=iq.get_from().bare, ptype="unsubscribed")
 
     async def on_user_register(self, iq: Iq):
         self.xmpp.client_roster[iq.get_from()].load()
         await self.add_component_to_roster(jid=iq.get_from())
 
     async def add_component_to_roster(self, jid: JID):
-        try:
-            if self.xmpp.no_roster_push:
-                return
-        except AttributeError:
+        if config.NO_ROSTER_PUSH:
             return
         items = {
             self.xmpp.boundjid.bare: {
                 "name": self.component_name,
                 "subscription": "both",
                 "groups": ["Slidge"],
             }
@@ -85,14 +88,16 @@
                     jid=jid.bare, roster_items=items
                 )
             except PermissionError:
                 log.warning(
                     "Slidge does not have the privilege to manage users' rosters. "
                     "Users should add the slidge component to their rosters manually."
                 )
+                if config.ROSTER_PUSH_PRESENCE_SUBSCRIPTION_REQUEST_FALLBACK:
+                    self.xmpp.send_presence(ptype="subscribe", pto=jid.bare)
 
     def on_presence_unsubscribe(self, p: Presence):
         if p.get_to() == self.xmpp.boundjid.bare:
             log.debug("REMOVE: Our roster: %s", self.xmpp.client_roster)
             self.xmpp["xep_0077"].api["user_remove"](None, None, p["from"], p)
             self.xmpp.event("user_unregister", p)
```

### Comparing `slidge-0.1.0b2/slidge/util/xep_0292/stanza.py` & `slidge-0.1.0rc1/slidge/util/xep_0292/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0292/vcard4.py` & `slidge-0.1.0rc1/slidge/util/xep_0292/vcard4.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             )
         )
 
         self.xmpp.plugin["xep_0030"].add_feature(NS)
 
     def get_vcard(self, jid: JidStr, requested_by: JidStr) -> Optional[VCard4]:
         vcard = self._vcards.get(JID(jid).bare)
-        log.debug("VCARDS: %s", self._vcards)
         if vcard:
             if auth := vcard.authorized_jids:
                 if JID(requested_by).bare in auth:
                     return vcard.content
             else:
                 return vcard.content
         return None
```

### Comparing `slidge-0.1.0b2/slidge/util/xep_0356/permissions.py` & `slidge-0.1.0rc1/slidge/util/xep_0356/permissions.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0356/privilege.py` & `slidge-0.1.0rc1/slidge/util/xep_0356/privilege.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0356/stanza.py` & `slidge-0.1.0rc1/slidge/util/xep_0356/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0356_old/privilege.py` & `slidge-0.1.0rc1/slidge/util/xep_0356_old/privilege.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0356_old/stanza.py` & `slidge-0.1.0rc1/slidge/util/xep_0356_old/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0461/reply.py` & `slidge-0.1.0rc1/slidge/util/xep_0461/reply.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.0b2/slidge/util/xep_0461/stanza.py` & `slidge-0.1.0rc1/slidge/util/xep_0461/stanza.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,39 +9,72 @@
     name = "reply"
     plugin_attrib = "reply"
     interfaces = {"id", "to"}
 
 
 class FeatureFallBack(ElementBase):
     # should also be a multi attrib
-    namespace = "urn:xmpp:feature-fallback:0"
+    namespace = "urn:xmpp:fallback:0"
     name = "fallback"
     plugin_attrib = "feature_fallback"
     interfaces = {"for"}
 
     def get_stripped_body(self):
         # only works for a single fallback_body attrib
         start = self["fallback_body"]["start"]
         end = self["fallback_body"]["end"]
         body = self.parent()["body"]
-        try:
-            start = int(start)
-            end = int(end)
-        except ValueError:
+        if start <= end < len(body):
+            return body[:start] + body[end:]
+        else:
             return body
+
+    def get_fallback_body(self):
+        # only works for a single fallback_body attrib
+        start = self["fallback_body"]["start"]
+        end = self["fallback_body"]["end"]
+        body = self.parent()["body"]
+        if start <= end:
+            return body[start:end]
         else:
-            return body[:start] + body[end:]
+            return ""
+
+    def add_quoted_fallback(self, fallback: str):
+        msg = self.parent()
+        quoted = "\n".join("> " + x.strip() for x in fallback.split("\n")) + "\n"
+        msg["body"] = quoted + msg["body"]
+        msg["feature_fallback"]["for"] = NS
+        msg["feature_fallback"]["fallback_body"]["start"] = 0
+        msg["feature_fallback"]["fallback_body"]["end"] = len(quoted)
 
 
 class FallBackBody(ElementBase):
     # According to https://xmpp.org/extensions/inbox/compatibility-fallback.html
     # this should be a multi_attrib *but* since it's a protoXEP, we'll see...
     namespace = FeatureFallBack.namespace
     name = "body"
     plugin_attrib = "fallback_body"
     interfaces = {"start", "end"}
 
+    def set_start(self, v: int):
+        self._set_attr("start", str(v))
+
+    def get_start(self):
+        try:
+            return int(self._get_attr("start"))
+        except ValueError:
+            return 0
+
+    def set_end(self, v: int):
+        self._set_attr("end", str(v))
+
+    def get_end(self):
+        try:
+            return int(self._get_attr("end"))
+        except ValueError:
+            return 0
+
 
 def register_plugins():
     register_stanza_plugin(Message, Reply)
     register_stanza_plugin(Message, FeatureFallBack)
     register_stanza_plugin(FeatureFallBack, FallBackBody)
```

### Comparing `slidge-0.1.0b2/setup.py` & `slidge-0.1.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['slidge',
  'slidge.core',
+ 'slidge.core.mixins',
+ 'slidge.core.muc',
  'slidge.plugins',
  'slidge.plugins.discord',
  'slidge.plugins.mattermost',
  'slidge.plugins.signal',
  'slidge.plugins.telegram',
+ 'slidge.plugins.whatsapp',
  'slidge.util',
  'slidge.util.xep_0030',
  'slidge.util.xep_0030.stanza',
- 'slidge.util.xep_0055',
+ 'slidge.util.xep_0050',
  'slidge.util.xep_0077',
- 'slidge.util.xep_0084',
  'slidge.util.xep_0100',
- 'slidge.util.xep_0115',
  'slidge.util.xep_0292',
- 'slidge.util.xep_0333',
  'slidge.util.xep_0356',
  'slidge.util.xep_0356_old',
- 'slidge.util.xep_0363',
  'slidge.util.xep_0461']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ConfigArgParse>=1.5.3,<2.0.0',
  'Pillow>=8.1.0',
  'aiohttp>=3.6.0',
  'pickle-secure>=0.9.99,<0.10.0',
  'qrcode>=7.3',
- 'slixmpp>=1.8.2,<2.0.0']
+ 'slixmpp>=1.8.3,<2.0.0']
 
 extras_require = \
 {'discord': ['discord.py-self>=1.9.2,<2.0.0'],
- 'facebook': ['mautrix-facebook>=0.4.0,<0.5.0'],
+ 'facebook': ['mautrix-facebook>=0.4.1,<0.5.0'],
  'mattermost': ['mattermost-api-reference-client>=4.0.0,<5.0.0',
                 'emoji>=2.0.0,<3.0.0'],
  'signal': ['aiosignald>=0.3.4,<0.4.0'],
  'skype': ['SkPy>=0.10.4,<0.11.0'],
  'steam': ['steam[client]>=1.3.0,<2.0.0'],
  'telegram': ['aiotdlib>=0.19.2,<0.20.0', 'pydantic']}
 
 entry_points = \
 {'console_scripts': ['slidge = slidge.__main__:main']}
 
 setup_kwargs = {
     'name': 'slidge',
-    'version': '0.1.0b2',
+    'version': '0.1.0rc1',
     'description': 'XMPP bridging framework',
-    'long_description': 'Slidge 🛷\n========\n\n[Home](https://sr.ht/~nicoco/slidge) |\n[Source](https://sr.ht/~nicoco/slidge/sources) |\n[Issues](https://sr.ht/~nicoco/slidge/trackers) |\n[Patches](https://lists.sr.ht/~nicoco/public-inbox) |\n[Chat](xmpp:slidge@conference.nicoco.fr?join)\n\nTurn any XMPP client into that fancy multiprotocol chat app that every cool kid want.\n\n[![Documentation status](https://readthedocs.org/projects/slidge/badge/?version=latest)](https://slidge.readthedocs.io/)\n[![builds.sr.ht status](https://builds.sr.ht/~nicoco/slidge/commits/master/ci.yml.svg)](https://builds.sr.ht/~nicoco/slidge/commits/master/ci.yml?)\n[![Debian package](https://builds.sr.ht/~nicoco/slidge/commits/master/debian.yml.svg)](https://builds.sr.ht/~nicoco/slidge/commits/master/debian.yml?)\n[![pypi](https://badge.fury.io/py/slidge.svg)](https://pypi.org/project/slidge/)\n\nSlidge is a general purpose XMPP (puppeteer) gateway framework in python.\nIt\'s a work in progress, but it should make\n[writing gateways to other chat networks](https://slidge.readthedocs.io/en/latest/dev/tutorial.html)\n(*plugins*) as frictionless as possible.\n\nIt comes with a few plugins included, implementing at least basic direct messaging and often more "advanced"\ninstant messaging features:\n\n|            | Presences[¹] | Typing[²] | Marks[³] | Upload[⁴] | Edit[⁵] | React[⁶] | Retract[⁷] | Reply[⁸] | \n|------------|--------------|-----------|----------|-----------|---------|----------|------------|----------|\n| Signal     | N/A          | ✅         | ✅        | ✅         | N/A     | ✅        | ✅          | ✅        |\n| Telegram   | ✅            | ✅         | ✅        | ✅         | ✅       | ✅        | ✅          | ✅        |\n| Discord    | ❌            | ✅         | N/A      | ✅         | ✅       | ~        | ✅          | ✅        |\n| Steam      | ✅            | ✅         | N/A      | ❌         | N/A     | ~        | N/A        | N/A      |\n| Mattermost | ✅            | ✅         | ~        | ✅         | ✅       | ✅        | ✅          | ❌        |\n| Facebook   | ❌            | ✅         | ✅        | ✅         | ✅       | ✅        | ✅          | ✅        |\n| Skype      | ✅            | ✅         | ❌        | ✅         | ✅       | ❌        | ✅          | ❌        |\n\n\n[¹]: https://xmpp.org/rfcs/rfc6121.html#presence\n[²]: https://xmpp.org/extensions/xep-0085.html\n[³]: https://xmpp.org/extensions/xep-0333.html\n[⁴]: https://xmpp.org/extensions/xep-0363.html\n[⁵]: https://xmpp.org/extensions/xep-0308.html\n[⁶]: https://xmpp.org/extensions/xep-0444.html\n[⁷]: https://xmpp.org/extensions/xep-0424.html\n[⁸]: https://xmpp.org/extensions/xep-0461.html\n\n\nThis table may not be entirely accurate, but **in theory**, stuff marked ✅ works.\nN/A means that the legacy network does not have an equivalent of this XMPP feature\n(because XMPP is better, what did you think?).\n\n**WARNING**: you may break the terms of use of a legacy network and end up getting your account locked\nby using slidge. Refer to the\n[keeping a low profile](https://slidge.readthedocs.io/en/latest/user/low_profile.html)\ndocumentation page for more info.\n\nStatus\n------\n\nSlidge is beta-grade software.\nRight now, only direct messages are implemented, no group chat stuff at all.\nDirect messaging does (more or less) work though.\nAny contribution whatsoever (testing, patches, suggestions, beer, …) is more than welcome.\n\nTry slidge and give us some\nfeedback, through the [MUC](xmpp:slidge@conference.nicoco.fr?join), the\n[issue tracker](https://todo.sr.ht/~nicoco/slidge) or in the\n[public inbox](https://lists.sr.ht/~nicoco/public-inbox).\nDon\'t be shy!\n\nInstallation\n------------\n\n### containers\n\nContainers for arm64 and amd64 are available on\n[docker hub](https://hub.docker.com/u/nicocool84).\n\n### debian\n\nDebian packages for *bullseye* (amd64 only for now, help welcome\nto support other architectures)\nare built on each push to master as artifacts of\n[this build job](https://builds.sr.ht/~nicoco/slidge/commits/master/debian.yml?).\n\nA repo is maintained by IGImonster. To use it do this (as root):\n\n```sh\n# trust the repo\'s key\nwget -O- http://deb.slidge.im/repo/slidge.gpg.key \\\n  |gpg --dearmor \\\n  |tee /usr/share/keyrings/slidge.gpg > /dev/null\n# add the repo, replace \'release\' with \'nightly\' if you\'re feeling adventurous \necho "deb [signed-by=/usr/share/keyrings/slidge.gpg] http://deb.slidge.im/repo/debian release main" \\\n  > /etc/apt/sources.list.d/slidge.list\n# install\napt update && apt install slidge -y\n```\n\nRefer to [the docs](https://slidge.readthedocs.io/en/latest/admin/launch.html#debian-packages)\nfor information about how to use the provided systemd service files.\n\n### pip\n\nTagged releases are uploaded to [pypi](https://pypi.org/project/slidge/).\n\n```sh\npip install slidge[signal]  # you can replace signal with any network listed in the table above\npython -m slidge --legacy-module=slidge.plugins.signal\n```\n\nIf you\'re looking for the bleeding edge, download an artifact\n[here](https://builds.sr.ht/~nicoco/slidge/commits/master/ci.yml?).\n\nAbout privacy\n-------------\n\nSlidge (and most if not all XMPP gateway that I know of) will break\nend-to-end encryption, or more precisely one of the \'ends\' become the\ngateway itself. If privacy is a major concern for you, my advice would\nbe to:\n\n-   use XMPP + OMEMO\n-   self-host your gateways\n-   have your gateways hosted by someone you know AFK and trust\n\nRelated projects\n----------------\n\n-   [Spectrum](https://www.spectrum.im/)\n-   [Bitfrost](https://github.com/matrix-org/matrix-bifrost)\n-   [Mautrix](https://github.com/mautrix)\n-   [matterbridge](https://github.com/42wim/matterbridge)\n-   [XMPP-discord-bridge](https://git.polynom.me/PapaTutuWawa/xmpp-discord-bridge)\n',
+    'long_description': 'Slidge 🛷\n========\n\n[Home](https://sr.ht/~nicoco/slidge) |\n[Source](https://sr.ht/~nicoco/slidge/sources) |\n[Issues](https://sr.ht/~nicoco/slidge/trackers) |\n[Patches](https://lists.sr.ht/~nicoco/public-inbox) |\n[Chat](xmpp:slidge@conference.nicoco.fr?join)\n\nTurn any XMPP client into that fancy multiprotocol chat app that every cool kid want.\n\n[![Documentation status](https://readthedocs.org/projects/slidge/badge/?version=latest)](https://slidge.readthedocs.io/)\n[![builds.sr.ht status](https://builds.sr.ht/~nicoco/slidge/commits/master/ci.yml.svg)](https://builds.sr.ht/~nicoco/slidge/commits/master/ci.yml?)\n[![Debian package](https://builds.sr.ht/~nicoco/slidge/commits/master/debian.yml.svg)](https://builds.sr.ht/~nicoco/slidge/commits/master/debian.yml?)\n[![pypi](https://badge.fury.io/py/slidge.svg)](https://pypi.org/project/slidge/)\n\nSlidge is a general purpose XMPP (puppeteer) gateway framework in python.\nIt\'s a work in progress, but it should make\n[writing gateways to other chat networks](https://slidge.readthedocs.io/en/latest/dev/tutorial.html)\n(*plugins*) as frictionless as possible.\n\nIt comes with a few plugins included, implementing at least basic direct messaging and often more "advanced"\ninstant messaging features:\n\n|            | Presences[¹] | Typing[²] | Marks[³] | Upload[⁴] | Edit[⁵] | React[⁶] | Retract[⁷] | Reply[⁸] | Groups[⁹] |\n|------------|--------------|-----------|----------|-----------|---------|----------|------------|----------|-----------|\n| Signal     | N/A          | ✅        | ✅       | ✅        | N/A     | ✅       | ✅         | ✅       | ~         |\n| Telegram   | ✅           | ✅        | ✅       | ✅        | ✅      | ✅       | ✅         | ✅       | ~         |\n| Discord    | ❌           | ✅        | N/A      | ✅        | ✅      | ~        | ✅         | ✅       | ❌         |\n| Steam      | ✅           | ✅        | N/A      | ❌        | N/A     | ~        | N/A        | N/A      | ❌         |\n| Mattermost | ✅           | ✅        | ~        | ✅        | ✅      | ✅       | ✅         | ❌       | ❌         |\n| Facebook   | ❌           | ✅        | ✅       | ✅        | ✅      | ✅       | ✅         | ✅       | ❌         |\n| Skype      | ✅           | ✅        | ❌       | ✅        | ✅      | ❌       | ✅         | ❌       | ❌         |\n| WhatsApp   | ✅           | ✅        | ✅       | ✅        | N/A     | ✅       | ✅         | ✅       | ❌         |\n\n\n[¹]: https://xmpp.org/rfcs/rfc6121.html#presence\n[²]: https://xmpp.org/extensions/xep-0085.html\n[³]: https://xmpp.org/extensions/xep-0333.html\n[⁴]: https://xmpp.org/extensions/xep-0363.html\n[⁵]: https://xmpp.org/extensions/xep-0308.html\n[⁶]: https://xmpp.org/extensions/xep-0444.html\n[⁷]: https://xmpp.org/extensions/xep-0424.html\n[⁸]: https://xmpp.org/extensions/xep-0461.html\n[⁹]: https://xmpp.org/extensions/xep-0045.html\n\n\nThis table may not be entirely accurate, but **in theory**, stuff marked ✅ works.\nN/A means that the legacy network does not have an equivalent of this XMPP feature\n(because XMPP is better, what did you think?).\n\n**WARNING**: you may break the terms of use of a legacy network and end up getting your account locked\nby using slidge. Refer to the\n[keeping a low profile](https://slidge.readthedocs.io/en/latest/user/low_profile.html)\ndocumentation page for more info.\n\nStatus\n------\n\nSlidge is **beta**-grade software for 1:1 chats.\nGroup chat support is **experimental**.\n\nTry slidge and give us some\nfeedback, through the [MUC](xmpp:slidge@conference.nicoco.fr?join), the\n[issue tracker](https://todo.sr.ht/~nicoco/slidge) or in the\n[public inbox](https://lists.sr.ht/~nicoco/public-inbox).\nDon\'t be shy!\n\nInstallation\n------------\n\n### containers\n\nContainers for arm64 and amd64 are available on\n[docker hub](https://hub.docker.com/u/nicocool84).\n\n### debian\n\nDebian packages for *bullseye* (amd64 only for now, help welcome\nto support other architectures)\nare built on each push to master as artifacts of\n[this build job](https://builds.sr.ht/~nicoco/slidge/commits/master/debian.yml?).\n\nA repo is maintained by IGImonster. To use it do this (as root):\n\n```sh\n# trust the repo\'s key\nwget -O- http://deb.slidge.im/repo/slidge.gpg.key \\\n  |gpg --dearmor \\\n  |tee /usr/share/keyrings/slidge.gpg > /dev/null\n# add the repo, replace \'release\' with \'nightly\' if you\'re feeling adventurous \necho "deb [signed-by=/usr/share/keyrings/slidge.gpg] http://deb.slidge.im/repo/debian release main" \\\n  > /etc/apt/sources.list.d/slidge.list\n# install\napt update && apt install slidge -y\n```\n\nRefer to [the docs](https://slidge.readthedocs.io/en/latest/admin/launch.html#debian-packages)\nfor information about how to use the provided systemd service files.\n\n### pip\n\nTagged releases are uploaded to [pypi](https://pypi.org/project/slidge/).\n\n```sh\npip install slidge[signal]  # you can replace signal with any network listed in the table above\npython -m slidge --legacy-module=slidge.plugins.signal\n```\n\nIf you\'re looking for the bleeding edge, download an artifact\n[here](https://builds.sr.ht/~nicoco/slidge/commits/master/ci.yml?).\n\nAbout privacy\n-------------\n\nSlidge (and most if not all XMPP gateway that I know of) will break\nend-to-end encryption, or more precisely one of the \'ends\' become the\ngateway itself. If privacy is a major concern for you, my advice would\nbe to:\n\n-   use XMPP + OMEMO\n-   self-host your gateways\n-   have your gateways hosted by someone you know AFK and trust\n\nRelated projects\n----------------\n\n-   [Spectrum](https://www.spectrum.im/)\n-   [Bitfrost](https://github.com/matrix-org/matrix-bifrost)\n-   [Mautrix](https://github.com/mautrix)\n-   [matterbridge](https://github.com/42wim/matterbridge)\n-   [XMPP-discord-bridge](https://git.polynom.me/PapaTutuWawa/xmpp-discord-bridge)\n',
     'author': 'Nicolas Cedilnik',
     'author_email': 'nicoco@nicoco.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://sr.ht/~nicoco/slidge/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `slidge-0.1.0b2/PKG-INFO` & `slidge-0.1.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slidge
-Version: 0.1.0b2
+Version: 0.1.0rc1
 Summary: XMPP bridging framework
 Home-page: https://sr.ht/~nicoco/slidge/
 License: AGPL-3.0-or-later
 Author: Nicolas Cedilnik
 Author-email: nicoco@nicoco.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -17,27 +17,27 @@
 Provides-Extra: mattermost
 Provides-Extra: signal
 Provides-Extra: skype
 Provides-Extra: steam
 Provides-Extra: telegram
 Requires-Dist: ConfigArgParse (>=1.5.3,<2.0.0)
 Requires-Dist: Pillow (>=8.1.0)
-Requires-Dist: SkPy (>=0.10.4,<0.11.0); extra == "skype"
+Requires-Dist: SkPy (>=0.10.4,<0.11.0) ; extra == "skype"
 Requires-Dist: aiohttp (>=3.6.0)
-Requires-Dist: aiosignald (>=0.3.4,<0.4.0); extra == "signal"
-Requires-Dist: aiotdlib (>=0.19.2,<0.20.0); extra == "telegram"
-Requires-Dist: discord.py-self (>=1.9.2,<2.0.0); extra == "discord"
-Requires-Dist: emoji (>=2.0.0,<3.0.0); extra == "mattermost"
-Requires-Dist: mattermost-api-reference-client (>=4.0.0,<5.0.0); extra == "mattermost"
-Requires-Dist: mautrix-facebook (>=0.4.0,<0.5.0); extra == "facebook"
+Requires-Dist: aiosignald (>=0.3.4,<0.4.0) ; extra == "signal"
+Requires-Dist: aiotdlib (>=0.19.2,<0.20.0) ; extra == "telegram"
+Requires-Dist: discord.py-self (>=1.9.2,<2.0.0) ; extra == "discord"
+Requires-Dist: emoji (>=2.0.0,<3.0.0) ; extra == "mattermost"
+Requires-Dist: mattermost-api-reference-client (>=4.0.0,<5.0.0) ; extra == "mattermost"
+Requires-Dist: mautrix-facebook (>=0.4.1,<0.5.0) ; extra == "facebook"
 Requires-Dist: pickle-secure (>=0.9.99,<0.10.0)
-Requires-Dist: pydantic; extra == "telegram"
+Requires-Dist: pydantic ; extra == "telegram"
 Requires-Dist: qrcode (>=7.3)
-Requires-Dist: slixmpp (>=1.8.2,<2.0.0)
-Requires-Dist: steam[client] (>=1.3.0,<2.0.0); extra == "steam"
+Requires-Dist: slixmpp (>=1.8.3,<2.0.0)
+Requires-Dist: steam[client] (>=1.3.0,<2.0.0) ; extra == "steam"
 Description-Content-Type: text/markdown
 
 Slidge 🛷
 ========
 
 [Home](https://sr.ht/~nicoco/slidge) |
 [Source](https://sr.ht/~nicoco/slidge/sources) |
@@ -56,51 +56,51 @@
 It's a work in progress, but it should make
 [writing gateways to other chat networks](https://slidge.readthedocs.io/en/latest/dev/tutorial.html)
 (*plugins*) as frictionless as possible.
 
 It comes with a few plugins included, implementing at least basic direct messaging and often more "advanced"
 instant messaging features:
 
-|            | Presences[¹] | Typing[²] | Marks[³] | Upload[⁴] | Edit[⁵] | React[⁶] | Retract[⁷] | Reply[⁸] | 
-|------------|--------------|-----------|----------|-----------|---------|----------|------------|----------|
-| Signal     | N/A          | ✅         | ✅        | ✅         | N/A     | ✅        | ✅          | ✅        |
-| Telegram   | ✅            | ✅         | ✅        | ✅         | ✅       | ✅        | ✅          | ✅        |
-| Discord    | ❌            | ✅         | N/A      | ✅         | ✅       | ~        | ✅          | ✅        |
-| Steam      | ✅            | ✅         | N/A      | ❌         | N/A     | ~        | N/A        | N/A      |
-| Mattermost | ✅            | ✅         | ~        | ✅         | ✅       | ✅        | ✅          | ❌        |
-| Facebook   | ❌            | ✅         | ✅        | ✅         | ✅       | ✅        | ✅          | ✅        |
-| Skype      | ✅            | ✅         | ❌        | ✅         | ✅       | ❌        | ✅          | ❌        |
+|            | Presences[¹] | Typing[²] | Marks[³] | Upload[⁴] | Edit[⁵] | React[⁶] | Retract[⁷] | Reply[⁸] | Groups[⁹] |
+|------------|--------------|-----------|----------|-----------|---------|----------|------------|----------|-----------|
+| Signal     | N/A          | ✅        | ✅       | ✅        | N/A     | ✅       | ✅         | ✅       | ~         |
+| Telegram   | ✅           | ✅        | ✅       | ✅        | ✅      | ✅       | ✅         | ✅       | ~         |
+| Discord    | ❌           | ✅        | N/A      | ✅        | ✅      | ~        | ✅         | ✅       | ❌         |
+| Steam      | ✅           | ✅        | N/A      | ❌        | N/A     | ~        | N/A        | N/A      | ❌         |
+| Mattermost | ✅           | ✅        | ~        | ✅        | ✅      | ✅       | ✅         | ❌       | ❌         |
+| Facebook   | ❌           | ✅        | ✅       | ✅        | ✅      | ✅       | ✅         | ✅       | ❌         |
+| Skype      | ✅           | ✅        | ❌       | ✅        | ✅      | ❌       | ✅         | ❌       | ❌         |
+| WhatsApp   | ✅           | ✅        | ✅       | ✅        | N/A     | ✅       | ✅         | ✅       | ❌         |
 
 
 [¹]: https://xmpp.org/rfcs/rfc6121.html#presence
 [²]: https://xmpp.org/extensions/xep-0085.html
 [³]: https://xmpp.org/extensions/xep-0333.html
 [⁴]: https://xmpp.org/extensions/xep-0363.html
 [⁵]: https://xmpp.org/extensions/xep-0308.html
 [⁶]: https://xmpp.org/extensions/xep-0444.html
 [⁷]: https://xmpp.org/extensions/xep-0424.html
 [⁸]: https://xmpp.org/extensions/xep-0461.html
+[⁹]: https://xmpp.org/extensions/xep-0045.html
 
 
 This table may not be entirely accurate, but **in theory**, stuff marked ✅ works.
 N/A means that the legacy network does not have an equivalent of this XMPP feature
 (because XMPP is better, what did you think?).
 
 **WARNING**: you may break the terms of use of a legacy network and end up getting your account locked
 by using slidge. Refer to the
 [keeping a low profile](https://slidge.readthedocs.io/en/latest/user/low_profile.html)
 documentation page for more info.
 
 Status
 ------
 
-Slidge is beta-grade software.
-Right now, only direct messages are implemented, no group chat stuff at all.
-Direct messaging does (more or less) work though.
-Any contribution whatsoever (testing, patches, suggestions, beer, …) is more than welcome.
+Slidge is **beta**-grade software for 1:1 chats.
+Group chat support is **experimental**.
 
 Try slidge and give us some
 feedback, through the [MUC](xmpp:slidge@conference.nicoco.fr?join), the
 [issue tracker](https://todo.sr.ht/~nicoco/slidge) or in the
 [public inbox](https://lists.sr.ht/~nicoco/public-inbox).
 Don't be shy!
```

