# Comparing `tmp/maplestory_openapi-2.4.1.tar.gz` & `tmp/maplestory_openapi-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maplestory_openapi-2.4.1.tar", last modified: Wed Feb 21 13:09:31 2024, max compression
+gzip compressed data, was "maplestory_openapi-2.5.0.tar", last modified: Tue Apr  9 15:09:33 2024, max compression
```

## Comparing `maplestory_openapi-2.4.1.tar` & `maplestory_openapi-2.5.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.878129 maplestory_openapi-2.4.1/maplestory_openapi/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.882129 maplestory_openapi-2.4.1/maplestory_openapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.882129 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.882129 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_ability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_android_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_beauty_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_cashitem_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_dojang.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_hexamatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_hexamatrix_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_hyper_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_item_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_link_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_pet_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_popularity.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_propensity.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_set_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_symbol_equipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_vmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.882129 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/guild/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/guild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/guild/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/guild/guild_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/cube_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/potential_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/starforce_history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/achievement_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/dojang_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/guild_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/overall_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/theseed_ranking.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/union_ranking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/union.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/union_artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/union_raider.py
--rw-r--r--   0 runner    (1001) docker     (127)    45983 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/maplestory_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/maplestory_api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/maplestory_openapi/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/maplestory_openapi/api/utils/date.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 13:09:31.878129 maplestory_openapi-2.4.1/maplestory_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-21 13:09:31.000000 maplestory_openapi-2.4.1/maplestory_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-21 13:09:31.000000 maplestory_openapi-2.4.1/maplestory_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 13:09:31.000000 maplestory_openapi-2.4.1/maplestory_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-21 13:09:31.000000 maplestory_openapi-2.4.1/maplestory_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-21 13:09:31.000000 maplestory_openapi-2.4.1/maplestory_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 13:09:31.886129 maplestory_openapi-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-21 13:09:25.000000 maplestory_openapi-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.340494 maplestory_openapi-2.5.0/maplestory_openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.340494 maplestory_openapi-2.5.0/maplestory_openapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.340494 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.344494 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_ability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_android_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_beauty_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_cashitem_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_dojang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_hexamatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_hexamatrix_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_hyper_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_item_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_link_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_pet_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_popularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_propensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_set_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_symbol_equipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_vmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.344494 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/guild/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/guild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/guild/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/guild/guild_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/cube_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/potential_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/starforce_history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/achievement_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/dojang_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/guild_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/overall_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/theseed_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/union_ranking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/union_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/union_raider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47126 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/maplestory_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/maplestory_api_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/maplestory_openapi/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/maplestory_openapi/api/utils/date.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:09:33.340494 maplestory_openapi-2.5.0/maplestory_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 15:09:33.000000 maplestory_openapi-2.5.0/maplestory_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-09 15:09:33.000000 maplestory_openapi-2.5.0/maplestory_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:09:33.000000 maplestory_openapi-2.5.0/maplestory_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 15:09:33.000000 maplestory_openapi-2.5.0/maplestory_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 15:09:33.000000 maplestory_openapi-2.5.0/maplestory_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:09:33.348494 maplestory_openapi-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-09 15:09:24.000000 maplestory_openapi-2.5.0/setup.py
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_ability.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_ability.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     ability_info(list[CharacterAbilityInfo]): 어빌리티 정보
     remain_fame(int): 보유 명성치
     preset_no(int): 적용 중인 어빌리티 프리셋 번호
     ability_preset_1(CharacterAbilityPreset): 어빌리티 1번 프리셋 전체 정보
     ability_preset_2(CharacterAbilityPreset): 어빌리티 2번 프리셋 전체 정보
     ability_preset_3(CharacterAbilityPreset): 어빌리티 3번 프리셋 전체 정보
     """
-    date: datetime
+    date: datetime | None | None
     ability_grade: str
     ability_info: list[CharacterAbilityInfo]
     remain_fame: int
     preset_no: int | None
     ability_preset_1: CharacterAbilityPreset | None
     ability_preset_2: CharacterAbilityPreset | None
     ability_preset_3: CharacterAbilityPreset | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_android_equipment.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_android_equipment.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     android_non_humanoid_flag(str): 비인간형 안드로이드 여부
     android_shop_usable_flag(str): 잡화상점 기능 이용 가능 여부
     preset_no(int): 적용 중인 장비 프리셋 번호
     android_preset_1(CharacterAndroidEquipmentPreset): 1번 프리셋 안드로이드 정보
     android_preset_2(CharacterAndroidEquipmentPreset): 2번 프리셋 안드로이드 정보
     android_preset_3(CharacterAndroidEquipmentPreset): 3번 프리셋 안드로이드 정보
     """
-    date: datetime
+    date: datetime | None
     android_name: str | None
     android_nickname: str | None
     android_icon: str | None
     android_description: str | None
     android_hair: CharacterAndroidEquipmentHair
     android_face: CharacterAndroidEquipmentFace
     android_skin_name: str | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_basic.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_basic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from datetime import datetime
 from pydantic import BaseModel
 
 
 class CharacterBasic(BaseModel):
     """캐릭터 기본 정보
 
+    date(datetime): 조회 기준일 (KST)
     character_name(str): 캐릭터 명
     world_name(str): 월드 명
     character_gender(str): 캐릭터 성별
     character_class(str): 캐릭터 직업
     character_class_level(str): 캐릭터 직업 차수
     character_level(int): 캐릭터 레벨
     character_exp(int): 현재 레벨에서 보유한 경험치
     character_exp_rate(str): 현재 레벨에서 경험치 퍼센트
     character_guild_name(str): 캐릭터 소속 길드 명
     character_image(str): 캐릭터 외형 이미지
     """
+    date: datetime | None
     character_name: str
     world_name: str
     character_gender: str
     character_class: str
     character_class_level: str
     character_level: int
     character_exp: int
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_beauty_equipment.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_beauty_equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     character_hair: 캐릭터 헤어 정보 (제로인 경우 알파, 엔젤릭버스터인 경우 일반 모드)
     character_face: 캐릭터 성형 정보 (제로인 경우 알파, 엔젤릭버스터인 경우 일반 모드)
     character_skin_name: 캐릭터 피부 명 (제로인 경우 알파, 엔젤릭버스터인 경우 일반 모드)
     additional_character_hair: 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드에 적용 중인 헤어 정보
     additional_character_face: 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드에 적용 중인 성형 정보
     additional_character_skin_name: 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드에 적용 중인 피부 명
     """
-    date: datetime
+    date: datetime | None
     character_gender: str
     character_class: str
     character_hair: CharacterBeautyEquipmentHair
     character_face: CharacterBeautyEquipmentFace
     character_skin_name: str
     additional_character_hair: CharacterBeautyEquipmentHair | None
     additional_character_face: CharacterBeautyEquipmentFace | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_cashitem_equipment.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_cashitem_equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     cash_item_equipment_preset_2(list[CharacterCashitemEquipmentPreset]): 2번 코디 프리셋
     cash_item_equipment_preset_3(list[CharacterCashitemEquipmentPreset]): 3번 코디 프리셋
     additional_cash_item_equipment_base(list[CharacterCashitemEquipmentPreset]): 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드에서 장착 중인 캐시 장비
     additional_cash_item_equipment_preset_1(list[CharacterCashitemEquipmentPreset]): 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드의 1번 코디 프리셋
     additional_cash_item_equipment_preset_2(list[CharacterCashitemEquipmentPreset]): 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드의 2번 코디 프리셋
     additional_cash_item_equipment_preset_3(list[CharacterCashitemEquipmentPreset]): 제로인 경우 베타, 엔젤릭버스터인 경우 드레스 업 모드의 3번 코디 프리셋
     """
-    date: datetime
+    date: datetime | None
     character_gender: str
     character_class: str
     preset_no: int
     cash_item_equipment_base: list[CharacterCashitemEquipmentPreset]
     cash_item_equipment_preset_1: list[CharacterCashitemEquipmentPreset]
     cash_item_equipment_preset_2: list[CharacterCashitemEquipmentPreset]
     cash_item_equipment_preset_3: list[CharacterCashitemEquipmentPreset]
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_dojang.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_dojang.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     character_class(str): 캐릭터 직업
     world_name(str): 월드 명
     dojang_best_floor(int): 무릉도장 최고 기록 층수
     date_dojang_record(datetime): 무릉도장 최고 기록 달성 일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     dojang_best_time(int): 무릉도장 최고 층수 클리어에 걸린 시간 (초)
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     world_name: str
     dojang_best_floor: int
     date_dojang_record: datetime
     dojang_best_time: int
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_hexamatrix.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_hexamatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 
 class CharacterHexaMatrix(BaseModel):
     """HEXA 코어 정보
 
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     character_hexa_core_equipment(list[CharacterHexaMatrixCoreEquipment]): HEXA 코어 정보
     """
-    date: datetime
+    date: datetime | None
     character_hexa_core_equipment: list[CharacterHexaMatrixCoreEquipment]
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_hexamatrix_stat.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_hexamatrix_stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,11 +28,11 @@
 class CharacterHexaMatrixStat(BaseModel):
     """HEXA 코어 스탯
 
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     character_class(str): 캐릭터 직업
     character_hexa_stat_core(list[CharacterHexaMatrixStatCore]): HEXA 코어 스탯 정보
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     character_hexa_stat_core: list[CharacterHexaMatrixStatCore]
     preset_hexa_stat_core: list[CharacterHexaMatrixStatCore]
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_hyper_stat.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_hyper_stat.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     hyper_stat_preset_1(list[CharacterHyperStatPreset]): 프리셋 1번 하이퍼 스탯 정보
     hyper_stat_preset_1_remain_point(int): 프리셋 1번 하이퍼 스탯 잔여 포인트
     hyper_stat_preset_2(list[CharacterHyperStatPreset]): 프리셋 2번 하이퍼 스탯 정보
     hyper_stat_preset_2_remain_point(int): 프리셋 2번 하이퍼 스탯 잔여 포인트
     hyper_stat_preset_3(list[CharacterHyperStatPreset]): 프리셋 3번 하이퍼 스탯 정보
     hyper_stat_preset_3_remain_point(int): 프리셋 3번 하이퍼 스탯 잔여 포인트
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     use_preset_no: str
     use_available_hyper_stat: int
     hyper_stat_preset_1: list[CharacterHyperStatPreset]
     hyper_stat_preset_1_remain_point: int
     hyper_stat_preset_2: list[CharacterHyperStatPreset]
     hyper_stat_preset_2_remain_point: int
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_item_equipment.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_item_equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
     item_equipment_preset_1(list[CharacterItemEquipmentInfo]): 1번 프리셋 장비 정보
     item_equipment_preset_2(list[CharacterItemEquipmentInfo]): 2번 프리셋 장비 정보
     item_equipment_preset_3(list[CharacterItemEquipmentInfo]): 3번 프리셋 장비 정보
     title(CharacterItemEquipmentTitle): 칭호 정보
     dragon_equipment(list[CharacterItemEquipmentInfo]): 에반 드래곤 장비 정보 (에반인 경우 응답)
     mechanic_equipment(list[CharacterItemEquipmentInfo]): 메카닉 장비 정보 (메카닉인 경우 응답)
     """
-    date: datetime
+    date: datetime | None
     character_gender: str
     character_class: str
     preset_no: int | None
     item_equipment: list[CharacterItemEquipmentInfo]
     item_equipment_preset_1: list[CharacterItemEquipmentInfo] | None
     item_equipment_preset_2: list[CharacterItemEquipmentInfo] | None
     item_equipment_preset_3: list[CharacterItemEquipmentInfo] | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_link_skill.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_link_skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     character_link_skill_preset_2(list[CharacterLinkSkillInfo]): 링크 스킬 2번 프리셋 정보
     character_link_skill_preset_3(list[CharacterLinkSkillInfo]): 링크 스킬 3번 프리셋 정보
     character_owned_link_skill(CharacterLinkSkillInfo): 내 링크 스킬 정보
     character_owned_link_skill_preset_1(CharacterLinkSkillInfo): 내 링크 스킬 1번 프리셋 정보
     character_owned_link_skill_preset_2(CharacterLinkSkillInfo): 내 링크 스킬 1번 프리셋 정보
     character_owned_link_skill_preset_3(CharacterLinkSkillInfo): 내 링크 스킬 1번 프리셋 정보
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     character_link_skill: list[CharacterLinkSkillInfo]
     character_link_skill_preset_1: list[CharacterLinkSkillInfo]
     character_link_skill_preset_2: list[CharacterLinkSkillInfo]
     character_link_skill_preset_3: list[CharacterLinkSkillInfo]
     character_owned_link_skill: CharacterLinkSkillInfo
     character_owned_link_skill_preset_1: CharacterLinkSkillInfo | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_pet_equipment.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_pet_equipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     pet_3_auto_skill(CharacterPetEquipmentAutoSkill): 펫3 펫 버프 자동스킬 정보
     pet_3_pet_type(str): 펫3 원더 펫 종류
     pet_3_skill(list[str]): 펫3 펫 보유 스킬
     pet_3_date_expire(datetime): 펫3 마법의 시간 (KST)
     pet_3_appearance(str): 펫3 외형
     pet_3_appearance_icon(str): 펫3 외형 아이콘
     """
-    date: datetime
+    date: datetime | None
     pet_1_name: str | None
     pet_1_nickname: str | None
     pet_1_icon: str | None
     pet_1_description: str | None
     pet_1_equipment: CharacterPetEquipmentItem | None
     pet_1_auto_skill: CharacterPetEquipmentAutoSkill | None
     pet_1_pet_type: str | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_propensity.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_propensity.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     charisma_level(int): 카리스마 레벨
     sensibility_level(int): 감성 레벨
     insight_level(int): 통찰력 레벨
     willingness_level(int): 의지 레벨
     handicraft_level(int): 손재주 레벨
     charm_level(int): 매력 레벨
     """
-    date: datetime
+    date: datetime | None
     charisma_level: int
     sensibility_level: int
     insight_level: int
     willingness_level: int
     handicraft_level: int
     charm_level: int
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_set_effect.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_set_effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 
 class CharacterSetEffect(BaseModel):
     """캐릭터 세트효과 정보
 
     date(datetime): 조회 기준일
     set_effect(list[CharacterSetEffectInfoDto]): 세트 효과 정보
     """
-    date: datetime
+    date: datetime | None
     set_effect: list[CharacterSetEffectInfo]
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_skill.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_skill.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     """캐릭터 스킬 정보
 
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     character_class(str): 캐릭터 직업
     character_skill_grade(str): 스킬 전직 차수
     character_skill(list[CharacterSkillInfo]): 스킬 정보
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     character_skill_grade: str
     character_skill: list[CharacterSkillInfo]
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_stat.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_stat.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     """캐릭터 스탯 정보
 
     date(datetime): 조회 기준일
     character_class(str): 직업
     final_stat(list[CharacterStatInfo]): 현재 스탯 정보
     remain_ap(int): 잔여 AP
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     final_stat: list[CharacterStatInfo]
     remain_ap: int
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_symbol_equipment.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_symbol_equipment.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,10 +35,10 @@
 class CharacterSymbolEquipment(BaseModel):
     """캐릭터 심볼 장비 정보
 
     date(datetime): 조회 기준일
     character_class(str): 직업
     symbol(list[CharacterSymbolEquipmentInfo]): 심볼 장비 정보
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     symbol: list[CharacterSymbolEquipmentInfo]
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/character/character_vmatrix.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/character/character_vmatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     """V매트릭스 정보
 
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     character_class(str): 캐릭터 직업
     character_v_core_equipment(list[CharacterVMatrixCoreEquipment]): V코어 정보
     character_v_matrix_remain_slot_upgrade_point(int): 캐릭터 잔여 매트릭스 강화 포인트
     """
-    date: datetime
+    date: datetime | None
     character_class: str
     character_v_core_equipment: list[CharacterVMatrixCoreEquipment]
     character_v_matrix_remain_slot_upgrade_point: int
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/guild/guild_basic.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/guild/guild_basic.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/cube_history.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/cube_history.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/potential_history.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/potential_history.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/history/starforce_history.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/history/starforce_history.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/achievement_ranking.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/achievement_ranking.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/dojang_ranking.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/dojang_ranking.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/guild_ranking.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/guild_ranking.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/overall_ranking.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/overall_ranking.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/theseed_ranking.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/theseed_ranking.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/ranking/union_ranking.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/ranking/union_ranking.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/union.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/union.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
     union_level(int): 유니온 레벨
     union_grade(str): 유니온 등급
     union_artifact_level(int): 아티팩트 레벨
     union_artifact_exp(int): 보유 아티팩트 경험치
     union_artifact_point(int): 보유 아티팩트 포인트
     """
-    date: datetime
+    date: datetime | None
     union_level: int
     union_grade: str
     union_artifact_level: int | None
     union_artifact_exp: int | None
     union_artifact_point: int | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/union_artifact.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/union_artifact.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,11 +35,11 @@
     """유니온 아티팩트 정보
 
     date(datetime): 조회 기준일
     union_artifact_effect(list[UnionArtifactEffect]): 아티팩트 효과 정보
     union_artifact_crystal(list[UnionArtifactCrystal]): 아티팩트 크리스탈 정보
     union_artifact_remain_ap(int): 잔여 아티팩트 AP
     """
-    date: datetime
+    date: datetime | None
     union_artifact_effect: list[UnionArtifactEffect]
     union_artifact_crystal: list[UnionArtifactCrystal]
-    union_artifact_remain_ap: int | None
+    union_artifact_remain_ap: int | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/dto/union/union_raider.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/dto/union/union_raider.py`

 * *Files 24% similar despite different names*

```diff
@@ -50,21 +50,47 @@
     stat_field_id(str): 공격대 배치 위치 (11시 방향부터 시계 방향 순서대로 0~7)
     stat_field_effect(str): 해당 지역 점령 효과
     """
     stat_field_id: str
     stat_field_effect: str
 
 
+class UnionRaiderPreset(BaseModel):
+    """유니온 프리셋 정보
+
+    union_Raider_stat(list[str]): 유니온 공격대원 효과
+    union_occupied_stat(list[str]): 유니온 공격대 점령 효과
+    union_inner_stat(list[UnionRaiderInnerStat]): 유니온 공격대 배치
+    union_block(list[UnionRaiderBlock]): 유니온 블록 정보
+    """
+    union_raider_stat: list[str]
+    union_occupied_stat: list[str]
+    union_inner_stat: list[UnionRaiderInnerStat]
+    union_block: list[UnionRaiderBlock]
+
+
 class UnionRaider(BaseModel):
     """유니온 공격대 정보
 
     date(datetime): 조회 기준일 (KST, 일 단위 데이터로 시, 분은 일괄 0으로 표기)
-    union_Raider_stat(str): 유니온 공격대원 효과
-    union_occupied_stat(str): 유니온 공격대 점령 효과
+    union_Raider_stat(list[str]): 유니온 공격대원 효과
+    union_occupied_stat(list[str]): 유니온 공격대 점령 효과
     union_inner_stat(list[UnionRaiderInnerStat]): 유니온 공격대 배치
     union_block(list[UnionRaiderBlock]): 유니온 블록 정보
+    use_preset_not(int): 적용 중인 프리셋 번호
+    union_raider_preset_1(UnionRaiderPreset): 유니온 프리셋 1번 정보
+    union_raider_preset_2(UnionRaiderPreset): 유니온 프리셋 2번 정보
+    union_raider_preset_3(UnionRaiderPreset): 유니온 프리셋 3번 정보
+    union_raider_preset_4(UnionRaiderPreset): 유니온 프리셋 4번 정보
+    union_raider_preset_5(UnionRaiderPreset): 유니온 프리셋 5번 정보
     """
-    date: datetime
+    date: datetime | None
     union_raider_stat: list[str]
     union_occupied_stat: list[str]
     union_inner_stat: list[UnionRaiderInnerStat]
     union_block: list[UnionRaiderBlock]
+    use_preset_not: int
+    union_raider_preset_1: UnionRaiderPreset | None
+    union_raider_preset_2: UnionRaiderPreset | None
+    union_raider_preset_3: UnionRaiderPreset | None
+    union_raider_preset_4: UnionRaiderPreset | None
+    union_raider_preset_5: UnionRaiderPreset | None
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/maplestory_api.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/maplestory_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,274 +60,284 @@
         )
 
     #region 캐릭터 정보 조회
 
     def get_character_id(self, character_name: str) -> Character:
         """캐릭터 식별자(ocid)를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param character_name (str): 캐릭터 이름
         """
 
         path = 'maplestory/v1/id'
         query = {
             'character_name': character_name,
         }
         r = self.fetch(path, query)
         return Character(**r)
 
-    def get_character_basic(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterBasic:
+    def get_character_basic(self, ocid: str, date: datetime | None = None) -> CharacterBasic:
         """기본 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/basic'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterBasic(**r)
 
-    def get_character_popularity(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterPopularity:
+    def get_character_popularity(self, ocid: str, date: datetime | None = None) -> CharacterPopularity:
         """인기도 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/popularity'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterPopularity(
             date=r.get('date'),
             popularity=r.get('popularity'),
         )
 
-    def get_character_stat(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterStat:
+    def get_character_stat(self, ocid: str, date: datetime | None = None) -> CharacterStat:
         """종합능력치 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/stat'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterStat(**r)
 
-    def get_character_hyper_stat(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterHyperStat:
+    def get_character_hyper_stat(self, ocid: str, date: datetime | None = None) -> CharacterHyperStat:
         """하이퍼스탯 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/hyper-stat'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterHyperStat(**r)
 
-    def get_character_propensity(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterPropensity:
+    def get_character_propensity(self, ocid: str, date: datetime | None = None) -> CharacterPropensity:
         """성향 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/propensity'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterPropensity(**r)
 
-    def get_character_ability(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterAbility:
+    def get_character_ability(self, ocid: str, date: datetime | None = None) -> CharacterAbility:
         """어빌리티 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/ability'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterAbility(**r)
 
-    def get_character_item_equipment(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterItemEquipment:
+    def get_character_item_equipment(self, ocid: str, date: datetime | None = None) -> CharacterItemEquipment:
         """장착한 장비 중 캐시 장비를 제외한 나머지 장비 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/item-equipment'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterItemEquipment(**r)
 
-    def get_character_cashitem_equipment(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterCashitemEquipment:
+    def get_character_cashitem_equipment(self, ocid: str, date: datetime | None = None) -> CharacterCashitemEquipment:
         """장착한 캐시 장비 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/cashitem-equipment'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
 
         return CharacterCashitemEquipment(**r)
 
-    def get_character_symbol_equipment(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterSymbolEquipment:
+    def get_character_symbol_equipment(self, ocid: str, date: datetime | None = None) -> CharacterSymbolEquipment:
         """장착한 심볼 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일 (KST)
         """
         path = 'maplestory/v1/character/symbol-equipment'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
         return CharacterSymbolEquipment(**r)
 
-    def get_character_set_effect(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterSetEffect:
+    def get_character_set_effect(self, ocid: str, date: datetime | None = None) -> CharacterSetEffect:
         """적용받고 있는 세트 효과 정보를 조회합니다
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.).
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/set-effect'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
         return CharacterSetEffect(**r)
 
-    def get_character_beauty_equipment(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterBeautyEquipment:
+    def get_character_beauty_equipment(self, ocid: str, date: datetime | None = None) -> CharacterBeautyEquipment:
         """캐릭터 헤어, 성형, 피부 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.).
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/beauty-equipment'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date)
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None
         }
         r = self.fetch(path, query)
         return CharacterBeautyEquipment(**r)
 
-    def get_character_android_equipment(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterAndroidEquipment:
+    def get_character_android_equipment(self, ocid: str, date: datetime | None = None) -> CharacterAndroidEquipment:
         """장착한 안드로이드 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.).
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/android-equipment'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterAndroidEquipment(**r)
 
-    def get_character_pet_equipment(self, ocid: str, date: datetime = get_proper_default_datetime(update_hour=1, day_offset=1)) -> CharacterPetEquipment:
+    def get_character_pet_equipment(self, ocid: str, date: datetime | None = None) -> CharacterPetEquipment:
         """장착한 펫 및 펫 스킬, 장비 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 캐릭터 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.).
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/pet-equipment'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterPetEquipment(**r)
 
-    def get_character_skill(self, ocid: str, character_skill_grade: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> CharacterSkill:
+    def get_character_skill(self, ocid: str, character_skill_grade: str, date: datetime | None = None) -> CharacterSkill:
         """캐릭터 스킬과 하이퍼 스킬 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 오전 0시부터 전일 데이터 조회가 가능합니다.
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
@@ -344,164 +354,167 @@
         - hyperactive: 하이퍼 액티브 스킬
         - 5: 5차 스킬
         - 6: 6차 스킬
         """
         path = 'maplestory/v1/character/skill'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
             'character_skill_grade': character_skill_grade,
         }
         r = self.fetch(path, query)
         return CharacterSkill(**r)
 
-    def get_character_link_skill(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> CharacterLinkSkill:
+    def get_character_link_skill(self, ocid: str, date: datetime | None = None) -> CharacterLinkSkill:
         """장착 링크 스킬 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 오전 0시부터 전일 데이터 조회가 가능합니다.
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/link-skill'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterLinkSkill(**r)
 
-    def get_character_vmatrix(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> CharacterVMatrix:
+    def get_character_vmatrix(self, ocid: str, date: datetime | None = None) -> CharacterVMatrix:
         """V매트릭스 슬롯 정보와 장착한 V코어 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 오전 0시부터 전일 데이터 조회가 가능합니다.
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/vmatrix'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterVMatrix(**r)
 
-    def get_character_hexamatrix(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> CharacterHexaMatrix:
+    def get_character_hexamatrix(self, ocid: str, date: datetime | None = None) -> CharacterHexaMatrix:
         """HEXA 매트릭스에 장착한 HEXA 코어 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 오전 0시부터 전일 데이터 조회가 가능합니다.
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/hexamatrix'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterHexaMatrix(**r)
 
-    def get_character_hexamatrix_stat(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> CharacterHexaMatrixStat:
+    def get_character_hexamatrix_stat(self, ocid: str, date: datetime | None = None) -> CharacterHexaMatrixStat:
         """HEXA 매트릭스에 설정한 HEXA 스탯 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 오전 0시부터 전일 데이터 조회가 가능합니다.
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/hexamatrix-stat'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterHexaMatrixStat(**r)
 
-    def get_character_dojang(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> CharacterDojang:
+    def get_character_dojang(self, ocid: str, date: datetime | None = None) -> CharacterDojang:
         """캐릭터 무릉도장 최고 기록 정보를 조회합니다.
 
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
         - 오전 0시부터 전일 데이터 조회가 가능합니다.
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신시 유의해 주시기 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/character/dojang'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return CharacterDojang(**r)
 
     #endregion
 
     #region 유니온 정보 조회
 
-    def get_union(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> Union:
+    def get_union(self, ocid: str, date: datetime | None = None) -> Union:
         """유니온 레벨 및 유니온 등급 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 유니온 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/user/union'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return Union(**r)
 
-    def get_union_raider(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> UnionRaider:
+    def get_union_raider(self, ocid: str, date: datetime | None = None) -> UnionRaider:
         """유니온에 배치된 공격대원 효과 및 공격대 점령 효과 등 상세 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 유니온 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/user/union-raider'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return UnionRaider(**r)
 
-    def get_union_artifact(self, ocid: str, date: datetime = get_proper_default_datetime(day_offset=1)) -> UnionArtifact:
+    def get_union_artifact(self, ocid: str, date: datetime | None = None) -> UnionArtifact:
         """유니온 아티팩트 정보를 조회합니다.
 
+        - 메이플스토리 게임 데이터는 평균 15분 후 확인 가능합니다.
         - 2023년 12월 21일 데이터부터 조회할 수 있습니다.
-        - 유니온 정보 조회 API는 일자별 데이터로 매일 오전 1시부터 전일 데이터 조회가 가능합니다. (예를 들어, 12월 22일 데이터를 조회하면 22일 00시부터 23일의 00시 사이의 데이터가 조회됩니다.)
+        - 과거 데이터는 원하는 일자를 입력해 조회할 수 있으며, 전일 데이터는 다음날 오전 1시부터 확인할 수 있습니다. (12월 22일 데이터 조회 시, 22일 00시부터 23일 00시 사이 데이터가 조회 됩니다.)
         - 게임 콘텐츠 변경으로 ocid가 변경될 수 있습니다. ocid 기반 서비스 갱신 시 유의해 주시길 바랍니다.
 
         @param ocid(str): 캐릭터 식별자(ocid)
         @param date(datetime): 조회 기준일(KST)
         """
         path = 'maplestory/v1/user/union-artifact'
         query = {
             'ocid': ocid,
-            'date': self.to_date_string(datetime(2023, 12, 21), date),
+            'date': self.to_date_string(datetime(2023, 12, 21), date) if date is not None else None,
         }
         r = self.fetch(path, query)
         return UnionArtifact(**r)
 
     #endregion
 
     #region 길드 정보 조회
@@ -760,17 +773,20 @@
         }
         r = self.fetch(path, query)
         return AchievementRanking(**r)
 
     #endregion
 
     def fetch(self, path: str, query: dict) -> Any:
+
+        params = {key: value for key, value in query.items() if value is not None}
+
         r = requests.get(
             f'{self.BASE_URL}{path}',
-            params=query,
+            params=params,
             headers={
                 'x-nxopen-api-key': self.api_key,
             },
             timeout=self.timeout,
         ).json()
 
         if (r.get('error')):
```

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi/api/utils/date.py` & `maplestory_openapi-2.5.0/maplestory_openapi/api/utils/date.py`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/maplestory_openapi.egg-info/SOURCES.txt` & `maplestory_openapi-2.5.0/maplestory_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maplestory_openapi-2.4.1/setup.py` & `maplestory_openapi-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='maplestory_openapi',
-    version='2.4.1',
+    version='2.5.0',
     description='This Python library enables the use of the MapleStory OpenAPI of Nexon.',
     author='so99ynoodles',
     url='https://github.com/SpiralMoon/maplestory.openapi',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'requests',
```

