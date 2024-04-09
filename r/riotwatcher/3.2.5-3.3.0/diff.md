# Comparing `tmp/riotwatcher-3.2.5.tar.gz` & `tmp/riotwatcher-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotwatcher-3.2.5.tar", last modified: Sat May 20 22:41:01 2023, max compression
+gzip compressed data, was "riotwatcher-3.3.0.tar", last modified: Tue Apr  9 08:22:10 2024, max compression
```

## Comparing `riotwatcher-3.2.5.tar` & `riotwatcher-3.3.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.326981 riotwatcher-3.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.330981 riotwatcher-3.2.5/src/riotwatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Deserializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.334981 riotwatcher-3.2.5/src/riotwatcher/Handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/DeprecationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/DeserializerAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/DictionaryDeserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/IllegalArgumentError.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.334981 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/ApplicationRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/InternalLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/Limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/MethodRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimiterAdapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/RequestHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/SanitationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/ThrowOnErrorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/TypeCorrectorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/Handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/LolWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/LorWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/RateLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/TftWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/ValWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.338981 riotwatcher-3.2.5/src/riotwatcher/_apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/BaseApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/Endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/NamedEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/UrlConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.338981 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChampionApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LeagueEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiV4Urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/MatchApiV5Urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/SpectatorApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/SummonerApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ThirdPartyCodeApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/LorEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/MatchApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/RankedApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/AccountApi.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.342981 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/AccountApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/RiotEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/riot/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/MatchApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/SummonerApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/TftEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/ContentApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/MatchApi.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/ContentApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/MatchApiUrls.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/ValEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/src/riotwatcher/riotwatcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.330981 riotwatcher-3.2.5/src/riotwatcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 22:41:01.000000 riotwatcher-3.2.5/src/riotwatcher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 22:41:01.346981 riotwatcher-3.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_LolWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_LorWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_RiotWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_TftWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-20 22:40:53.000000 riotwatcher-3.2.5/tests/test_ValWatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.443936 riotwatcher-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-09 08:22:10.443936 riotwatcher-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 08:22:10.443936 riotwatcher-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.419936 riotwatcher-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.423936 riotwatcher-3.3.0/src/riotwatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Deserializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.427936 riotwatcher-3.3.0/src/riotwatcher/Handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/DeprecationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/DeserializerAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/DictionaryDeserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/IllegalArgumentError.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.427936 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/ApplicationRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/InternalLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/Limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/MethodRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimiterAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/RequestHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/SanitationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/ThrowOnErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/TypeCorrectorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/Handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/LolWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/LorWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/RateLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/TftWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/ValWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.431936 riotwatcher-3.3.0/src/riotwatcher/_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/BaseApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/Endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/NamedEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/UrlConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.431936 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/SpectatorApiV5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.435936 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ChampionApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/LeagueEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/LolStatusApiV4Urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/MatchApiV5Urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/SpectatorApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/SummonerApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ThirdPartyCodeApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.435936 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.435936 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/urls/LorEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/urls/MatchApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/urls/RankedApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.435936 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/AccountApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.439936 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/urls/AccountApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/urls/RiotEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/riot/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.439936 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.439936 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/MatchApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/SummonerApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/TftEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.439936 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/ContentApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/MatchApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.439936 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/urls/ContentApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/urls/MatchApiUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/urls/ValEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/src/riotwatcher/riotwatcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.443936 riotwatcher-3.3.0/src/riotwatcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-09 08:22:10.000000 riotwatcher-3.3.0/src/riotwatcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-09 08:22:10.000000 riotwatcher-3.3.0/src/riotwatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 08:22:10.000000 riotwatcher-3.3.0/src/riotwatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 08:22:10.000000 riotwatcher-3.3.0/src/riotwatcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 08:22:10.000000 riotwatcher-3.3.0/src/riotwatcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 08:22:10.443936 riotwatcher-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/tests/test_LolWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/tests/test_LorWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/tests/test_RiotWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/tests/test_TftWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-09 08:22:06.000000 riotwatcher-3.3.0/tests/test_ValWatcher.py
```

### Comparing `riotwatcher-3.2.5/LICENSE` & `riotwatcher-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/PKG-INFO` & `riotwatcher-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: riotwatcher
-Version: 3.2.5
+Version: 3.3.0
 Summary: RiotWatcher is a thin wrapper on top of the Riot Games API for League of Legends.
 Home-page: https://github.com/pseudonym117/Riot-Watcher
 Author: AG Stephan
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Classifier: Topic :: Games/Entertainment :: Role-Playing
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: requests
+Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 RiotWatcher
 ===========
 
 |pypi| |docs| |coverage| |black|
 
 Check for full (read: slightly better) documentation `here <http://riot-watcher.readthedocs.io/en/latest/>`__!
 
 RiotWatcher is a thin wrapper on top of the `Riot Games API for League
 of Legends <https://developer.riotgames.com/>`__. All public methods as
-of 5/20/2023 are supported in full.
+of 4/9/2024 are supported in full.
 
 RiotWatcher by default supports a naive rate limiter. This rate limiter will
 try to stop you from making too many requests, and in a single threaded test
 environment does this rather well. In a multithreaded environment, you may
 still get some 429 errors. 429 errors are currently NOT retried for you.
 
 
@@ -176,14 +182,22 @@
 Known Issues
 ------------
 
 Rate limiter has some race conditions when used concurrently.
 
 Changelog
 ---------
+v3.3.0 - 4/9/2024
+~~~~~~~~~~~~~~~~~
+LoL Champion mastery endpoints updated to use puuid
+
+LoL spectator v4 replaced with v5
+
+Remove support for python3.7; add supported for python3.12
+
 v3.2.4 - 10/29/2022
 ~~~~~~~~~~~~~~~~~~~
 Add ``start`` parameter to TFT match API
 
 Correct remapping for SEA region
 
 Add python 3.11 support to CI/CD
```

### Comparing `riotwatcher-3.2.5/README.rst` & `riotwatcher-3.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 |pypi| |docs| |coverage| |black|
 
 Check for full (read: slightly better) documentation `here <http://riot-watcher.readthedocs.io/en/latest/>`__!
 
 RiotWatcher is a thin wrapper on top of the `Riot Games API for League
 of Legends <https://developer.riotgames.com/>`__. All public methods as
-of 5/20/2023 are supported in full.
+of 4/9/2024 are supported in full.
 
 RiotWatcher by default supports a naive rate limiter. This rate limiter will
 try to stop you from making too many requests, and in a single threaded test
 environment does this rather well. In a multithreaded environment, you may
 still get some 429 errors. 429 errors are currently NOT retried for you.
 
 
@@ -161,14 +161,22 @@
 Known Issues
 ------------
 
 Rate limiter has some race conditions when used concurrently.
 
 Changelog
 ---------
+v3.3.0 - 4/9/2024
+~~~~~~~~~~~~~~~~~
+LoL Champion mastery endpoints updated to use puuid
+
+LoL spectator v4 replaced with v5
+
+Remove support for python3.7; add supported for python3.12
+
 v3.2.4 - 10/29/2022
 ~~~~~~~~~~~~~~~~~~~
 Add ``start`` parameter to TFT match API
 
 Correct remapping for SEA region
 
 Add python 3.11 support to CI/CD
```

### Comparing `riotwatcher-3.2.5/setup.py` & `riotwatcher-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/DeprecationHandler.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/DeprecationHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/DeserializerAdapter.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/DeserializerAdapter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/BasicRateLimiter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/HeaderBasedLimiter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/Limits.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/Limits.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/OopsRateLimiter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimit/__init__.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimit/__init__.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RateLimiterAdapter.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RateLimiterAdapter.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/RequestHandler.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/SanitationHandler.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/SanitationHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/Handlers/TypeCorrectorHandler.py` & `riotwatcher-3.3.0/src/riotwatcher/Handlers/TypeCorrectorHandler.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/LolWatcher.py` & `riotwatcher-3.3.0/src/riotwatcher/LolWatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ChampionApiV3,
     ChampionMasteryApiV4,
     ClashApiV1,
     DataDragonApi,
     LeagueApiV4,
     LolStatusApiV3,
     LolStatusApiV4,
-    SpectatorApiV4,
+    SpectatorApiV5,
     SummonerApiV4,
     MatchApiV5,
     ChallengesApiV1,
 )
 
 LOG = logging.getLogger(__name__)
 
@@ -101,15 +101,15 @@
         self._lol_status_v3 = LolStatusApiV3(self._base_api)
         self._lol_status_v4 = LolStatusApiV4(self._base_api)
         self._data_dragon = DataDragonApi(self._base_api)
         self._clash = ClashApiV1(self._base_api)
         self._champion_mastery = ChampionMasteryApiV4(self._base_api)
         self._league = LeagueApiV4(self._base_api)
         self._match = MatchApiV5(self._base_api)
-        self._spectator = SpectatorApiV4(self._base_api)
+        self._spectator = SpectatorApiV5(self._base_api)
         self._challenges = ChallengesApiV1(self._base_api)
         self._summoner = SummonerApiV4(self._base_api)
 
         self._lol_status = (
             self._lol_status_v4 if default_status_v4 else self._lol_status_v3
         )
         # todo: tournament-stub
@@ -207,15 +207,15 @@
     def match_v5(self):
         """this property has been deprecated. Use 'match' property instead."""
         raise NotImplementedError(
             "this property has been deprecated. Use 'match' property instead."
         )
 
     @property
-    def spectator(self) -> SpectatorApiV4:
+    def spectator(self) -> SpectatorApiV5:
         """
         Interface to the Spectator Endpoint
 
         :rtype: league_of_legends.SpectatorApiV4
         """
         return self._spectator
```

### Comparing `riotwatcher-3.2.5/src/riotwatcher/LorWatcher.py` & `riotwatcher-3.3.0/src/riotwatcher/LorWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/TftWatcher.py` & `riotwatcher-3.3.0/src/riotwatcher/TftWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/ValWatcher.py` & `riotwatcher-3.3.0/src/riotwatcher/ValWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/__init__.py` & `riotwatcher-3.3.0/src/riotwatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/BaseApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/BaseApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/Endpoint.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/Endpoint.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/NamedEndpoint.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/NamedEndpoint.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/helpers.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/helpers.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ChallengesApiV1.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ChampionApiV3.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/ClashApiV1.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/DataDragonApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/MatchApiV5.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/SpectatorApiV5.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from .. import BaseApi, NamedEndpoint
-from .urls import SpectatorApiV4Urls
+from .urls import SpectatorApiV5Urls
 
 
-class SpectatorApiV4(NamedEndpoint):
+class SpectatorApiV5(NamedEndpoint):
     """
-    This class wraps the Spectator-v4 endpoint calls provided by the Riot API.
+    This class wraps the Spectator-v5 endpoint calls provided by the Riot API.
 
-    See https://developer.riotgames.com/api-methods/#spectator-v4 for more detailed
+    See https://developer.riotgames.com/api-methods/#spectator-v5 for more detailed
     information
     """
 
     def __init__(self, base_api: BaseApi):
         """
-        Initialize a new SpectatorApiV3 which uses the provided base_api
+        Initialize a new SpectatorApiV5 which uses the provided base_api
 
         :param BaseApi base_api: the root API object to use for making all requests.
         """
         super().__init__(base_api, self.__class__.__name__)
 
-    def by_summoner(self, region: str, encrypted_summoner_id: str):
+    def by_summoner(self, region: str, encrypted_puuid: str):
         """
-        Get current game information for the given summoner ID
+        Get current game information for the given PUUID
 
         :param string region:                   The region to execute this request on
-        :param string encrypted_summoner_id:    The ID of the summoner.
+        :param string encrypted_puuid:          The PUUID of the summoner.
 
         :returns: CurrentGameInfo
         """
         return self._request_endpoint(
             self.by_summoner.__name__,
             region,
-            SpectatorApiV4Urls.by_summoner,
-            encrypted_summoner_id=encrypted_summoner_id,
+            SpectatorApiV5Urls.by_summoner,
+            encrypted_puuid=encrypted_puuid,
         )
 
     def featured_games(self, region: str):
         """
         Get list of featured games.
 
         :param string region: The region to execute this request on
 
         :returns: FeaturedGames
         """
         return self._request_endpoint(
-            self.featured_games.__name__, region, SpectatorApiV4Urls.featured_games
+            self.featured_games.__name__, region, SpectatorApiV5Urls.featured_games
         )
```

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/LeagueApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/league_of_legends/urls/__init__.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/league_of_legends/urls/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .ChampionApiUrls import ChampionApiV3Urls
 from .ChampionMasteryApiUrls import ChampionMasteryApiV4Urls
 from .ClashApiUrls import ClashApiV1Urls
 from .DataDragonUrls import DataDragonUrls
 from .LeagueApiUrls import LeagueApiV4Urls
 from .LolStatusApiUrls import LolStatusApiV3Urls
 from .LolStatusApiV4Urls import LolStatusApiV4Urls
-from .SpectatorApiUrls import SpectatorApiV4Urls
+from .SpectatorApiUrls import SpectatorApiV5Urls
 from .SummonerApiUrls import SummonerApiV4Urls
 from .ThirdPartyCodeApiUrls import ThirdPartyCodeApiV4Urls
 from .MatchApiV5Urls import MatchApiV5Urls
 from .ChallengesApiV1Urls import ChallengesApiV1Urls
```

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/MatchApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/legends_of_runeterra/RankedApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/riot/AccountApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/riot/AccountApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/LeagueApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/MatchApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/SummonerApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/team_fight_tactics/urls/LeagueApiUrls.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/ContentApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/ContentApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/_apis/valorant/MatchApi.py` & `riotwatcher-3.3.0/src/riotwatcher/_apis/valorant/MatchApi.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher/riotwatcher.py` & `riotwatcher-3.3.0/src/riotwatcher/riotwatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/src/riotwatcher.egg-info/PKG-INFO` & `riotwatcher-3.3.0/src/riotwatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: riotwatcher
-Version: 3.2.5
+Version: 3.3.0
 Summary: RiotWatcher is a thin wrapper on top of the Riot Games API for League of Legends.
 Home-page: https://github.com/pseudonym117/Riot-Watcher
 Author: AG Stephan
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
 Classifier: Topic :: Games/Entertainment :: Role-Playing
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: requests
+Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: tox; extra == "dev"
 
 RiotWatcher
 ===========
 
 |pypi| |docs| |coverage| |black|
 
 Check for full (read: slightly better) documentation `here <http://riot-watcher.readthedocs.io/en/latest/>`__!
 
 RiotWatcher is a thin wrapper on top of the `Riot Games API for League
 of Legends <https://developer.riotgames.com/>`__. All public methods as
-of 5/20/2023 are supported in full.
+of 4/9/2024 are supported in full.
 
 RiotWatcher by default supports a naive rate limiter. This rate limiter will
 try to stop you from making too many requests, and in a single threaded test
 environment does this rather well. In a multithreaded environment, you may
 still get some 429 errors. 429 errors are currently NOT retried for you.
 
 
@@ -176,14 +182,22 @@
 Known Issues
 ------------
 
 Rate limiter has some race conditions when used concurrently.
 
 Changelog
 ---------
+v3.3.0 - 4/9/2024
+~~~~~~~~~~~~~~~~~
+LoL Champion mastery endpoints updated to use puuid
+
+LoL spectator v4 replaced with v5
+
+Remove support for python3.7; add supported for python3.12
+
 v3.2.4 - 10/29/2022
 ~~~~~~~~~~~~~~~~~~~
 Add ``start`` parameter to TFT match API
 
 Correct remapping for SEA region
 
 Add python 3.11 support to CI/CD
```

### Comparing `riotwatcher-3.2.5/src/riotwatcher.egg-info/SOURCES.txt` & `riotwatcher-3.3.0/src/riotwatcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 src/riotwatcher/_apis/league_of_legends/ChampionMasteryApiV4.py
 src/riotwatcher/_apis/league_of_legends/ClashApiV1.py
 src/riotwatcher/_apis/league_of_legends/DataDragonApi.py
 src/riotwatcher/_apis/league_of_legends/LeagueApiV4.py
 src/riotwatcher/_apis/league_of_legends/LolStatusApiV3.py
 src/riotwatcher/_apis/league_of_legends/LolStatusApiV4.py
 src/riotwatcher/_apis/league_of_legends/MatchApiV5.py
-src/riotwatcher/_apis/league_of_legends/SpectatorApiV4.py
+src/riotwatcher/_apis/league_of_legends/SpectatorApiV5.py
 src/riotwatcher/_apis/league_of_legends/SummonerApiV4.py
 src/riotwatcher/_apis/league_of_legends/__init__.py
 src/riotwatcher/_apis/league_of_legends/urls/ChallengesApiV1Urls.py
 src/riotwatcher/_apis/league_of_legends/urls/ChampionApiUrls.py
 src/riotwatcher/_apis/league_of_legends/urls/ChampionMasteryApiUrls.py
 src/riotwatcher/_apis/league_of_legends/urls/ClashApiUrls.py
 src/riotwatcher/_apis/league_of_legends/urls/DataDragonUrls.py
```

### Comparing `riotwatcher-3.2.5/tests/test_LolWatcher.py` & `riotwatcher-3.3.0/tests/test_LolWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/tests/test_LorWatcher.py` & `riotwatcher-3.3.0/tests/test_LorWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/tests/test_RiotWatcher.py` & `riotwatcher-3.3.0/tests/test_RiotWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/tests/test_TftWatcher.py` & `riotwatcher-3.3.0/tests/test_TftWatcher.py`

 * *Files identical despite different names*

### Comparing `riotwatcher-3.2.5/tests/test_ValWatcher.py` & `riotwatcher-3.3.0/tests/test_ValWatcher.py`

 * *Files identical despite different names*

