# Comparing `tmp/oscr_ui-2024.3b291.tar.gz` & `tmp/oscr_ui-2024.4b20.tar.gz`

## Comparing `oscr_ui-2024.3b291.tar` & `oscr_ui-2024.4b20.tar`

### file list

```diff
@@ -1,66 +1,68 @@
--rw-r--r--   0        0        0     1869 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/.OSCR_settings.ini
--rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/.flake8
--rw-r--r--   0        0        0       98 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/.pre-commit-config.yaml
--rw-r--r--   0        0        0    26495 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/main.py
--rw-r--r--   0        0        0      180 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/shell.nix
--rw-r--r--   0        0        0     1306 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/.github/workflows/build.yml
--rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/__init__.py
--rw-r--r--   0        0        0    57360 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/app.py
--rw-r--r--   0        0        0     8507 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/callbacks.py
--rw-r--r--   0        0        0    15183 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/datafunctions.py
--rw-r--r--   0        0        0    15700 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/datamodels.py
--rw-r--r--   0        0        0    14966 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/displayer.py
--rw-r--r--   0        0        0     6127 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/iofunctions.py
--rw-r--r--   0        0        0     9328 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/leagueconnector.py
--rw-r--r--   0        0        0     5052 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/style.py
--rw-r--r--   0        0        0    15517 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/subwindows.py
--rw-r--r--   0        0        0     4131 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/textedit.py
--rw-r--r--   0        0        0    14849 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/widgetbuilder.py
--rw-r--r--   0        0        0    10447 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/OSCRUI/widgets.py
--rw-r--r--   0        0        0   170564 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/Overpass-Bold.ttf
--rw-r--r--   0        0        0   170328 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/Overpass-Medium.ttf
--rw-r--r--   0        0        0   170204 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/Overpass-Regular.ttf
--rw-r--r--   0        0        0    87172 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/RobotoMono-Medium.ttf
--rw-r--r--   0        0        0    87236 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/arrow-down.svg
--rw-r--r--   0        0        0      269 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/arrow-right.svg
--rw-r--r--   0        0        0      225 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/close.svg
--rw-r--r--   0        0        0      348 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/collapse-bottom.svg
--rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/collapse-left.svg
--rw-r--r--   0        0        0      363 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/collapse-right.svg
--rw-r--r--   0        0        0      339 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/collapse-top.svg
--rw-r--r--   0        0        0      319 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/copy.svg
--rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/expand-bottom.svg
--rw-r--r--   0        0        0      362 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/expand-left.svg
--rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/expand-right.svg
--rw-r--r--   0        0        0      340 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/expand-top.svg
--rw-r--r--   0        0        0      368 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/export-parse.svg
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/fat-arrow-down.svg
--rw-r--r--   0        0        0     1006 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/gear.svg
--rw-r--r--   0        0        0      333 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/ladder.svg
--rw-r--r--   0        0        0    12787 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/loading.png
--rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/log-cut-tight.svg
--rw-r--r--   0        0        0      407 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/log-cut-wide.svg
--rw-r--r--   0        0        0      382 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/log-down.svg
--rw-r--r--   0        0        0      391 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/log-up.svg
--rw-r--r--   0        0        0    41619 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/oscr_icon_small.ico
--rw-r--r--   0        0        0    20631 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/oscr_icon_small.png
--rw-r--r--   0        0        0    25546 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/oscrbanner-slim-dark-label.png
--rw-r--r--   0        0        0    10840 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/oscrbanner-slim-dark.png
--rw-r--r--   0        0        0    10750 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/oscrbanner-slim.png
--rw-r--r--   0        0        0      449 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/parser-left.svg
--rw-r--r--   0        0        0      454 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/parser-right.svg
--rw-r--r--   0        0        0      395 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/refresh-cw.svg
--rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/rename.svg
--rw-r--r--   0        0        0      222 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/resize.svg
--rw-r--r--   0        0        0      387 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/save-cw.svg
--rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/save.svg
--rw-r--r--   0        0        0    10497 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/section31badge.png
--rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/star.svg
--rw-r--r--   0        0        0    80078 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/stobuildslogo.png
--rw-r--r--   0        0        0      443 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/assets/truncate-cw.svg
--rw-r--r--   0        0        0       12 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/.gitignore
--rw-r--r--   0        0        0    35149 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/LICENSE
--rw-r--r--   0        0        0      841 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/README.md
--rw-r--r--   0        0        0      987 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/pyproject.toml
--rw-r--r--   0        0        0    42049 1980-01-01 00:00:00.000000 oscr_ui-2024.3b291/PKG-INFO
+-rw-r--r--   0        0        0     1886 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.OSCR_settings.ini
+-rw-r--r--   0        0        0       58 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.flake8
+-rw-r--r--   0        0        0       98 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    26538 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/main.py
+-rw-r--r--   0        0        0      180 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/shell.nix
+-rw-r--r--   0        0        0 105939534 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/~temp_log_files\[24-03-29_06-54-59--24-03-30_15-01-29]combatlog.log
+-rw-r--r--   0        0        0 25252302 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/~temp_log_files\[24-03-30_15-08-23--24-03-30_20-19-03]combatlog.log
+-rw-r--r--   0        0        0     1306 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.github/workflows/build.yml
+-rw-r--r--   0        0        0      214 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/__init__.py
+-rw-r--r--   0        0        0    58232 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/app.py
+-rw-r--r--   0        0        0     8916 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/callbacks.py
+-rw-r--r--   0        0        0    15450 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/datafunctions.py
+-rw-r--r--   0        0        0    15700 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/datamodels.py
+-rw-r--r--   0        0        0    14983 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/displayer.py
+-rw-r--r--   0        0        0     6127 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/iofunctions.py
+-rw-r--r--   0        0        0     9328 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/leagueconnector.py
+-rw-r--r--   0        0        0     5052 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/style.py
+-rw-r--r--   0        0        0    16622 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/subwindows.py
+-rw-r--r--   0        0        0     4131 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/textedit.py
+-rw-r--r--   0        0        0    14849 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/widgetbuilder.py
+-rw-r--r--   0        0        0    10447 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/OSCRUI/widgets.py
+-rw-r--r--   0        0        0   170564 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/Overpass-Bold.ttf
+-rw-r--r--   0        0        0   170328 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/Overpass-Medium.ttf
+-rw-r--r--   0        0        0   170204 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/Overpass-Regular.ttf
+-rw-r--r--   0        0        0    87172 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/RobotoMono-Medium.ttf
+-rw-r--r--   0        0        0    87236 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0      268 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/arrow-down.svg
+-rw-r--r--   0        0        0      269 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/arrow-right.svg
+-rw-r--r--   0        0        0      225 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/close.svg
+-rw-r--r--   0        0        0      348 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-bottom.svg
+-rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-left.svg
+-rw-r--r--   0        0        0      363 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-right.svg
+-rw-r--r--   0        0        0      339 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/collapse-top.svg
+-rw-r--r--   0        0        0      319 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/copy.svg
+-rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-bottom.svg
+-rw-r--r--   0        0        0      362 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-left.svg
+-rw-r--r--   0        0        0      360 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-right.svg
+-rw-r--r--   0        0        0      340 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/expand-top.svg
+-rw-r--r--   0        0        0      368 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/export-parse.svg
+-rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/fat-arrow-down.svg
+-rw-r--r--   0        0        0     1006 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/gear.svg
+-rw-r--r--   0        0        0      333 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/ladder.svg
+-rw-r--r--   0        0        0    12787 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/loading.png
+-rw-r--r--   0        0        0      434 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-cut-tight.svg
+-rw-r--r--   0        0        0      407 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-cut-wide.svg
+-rw-r--r--   0        0        0      382 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-down.svg
+-rw-r--r--   0        0        0      391 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/log-up.svg
+-rw-r--r--   0        0        0    41619 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscr_icon_small.ico
+-rw-r--r--   0        0        0    20631 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscr_icon_small.png
+-rw-r--r--   0        0        0    25546 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscrbanner-slim-dark-label.png
+-rw-r--r--   0        0        0    10840 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscrbanner-slim-dark.png
+-rw-r--r--   0        0        0    10750 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/oscrbanner-slim.png
+-rw-r--r--   0        0        0      449 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/parser-left.svg
+-rw-r--r--   0        0        0      454 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/parser-right.svg
+-rw-r--r--   0        0        0      395 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/refresh-cw.svg
+-rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/rename.svg
+-rw-r--r--   0        0        0      222 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/resize.svg
+-rw-r--r--   0        0        0      387 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/save-cw.svg
+-rw-r--r--   0        0        0      389 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/save.svg
+-rw-r--r--   0        0        0    10497 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/section31badge.png
+-rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/star.svg
+-rw-r--r--   0        0        0    80078 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/stobuildslogo.png
+-rw-r--r--   0        0        0      443 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/assets/truncate-cw.svg
+-rw-r--r--   0        0        0       12 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/.gitignore
+-rw-r--r--   0        0        0    35149 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/LICENSE
+-rw-r--r--   0        0        0      841 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/README.md
+-rw-r--r--   0        0        0      986 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/pyproject.toml
+-rw-r--r--   0        0        0    42047 1980-01-01 00:00:00.000000 oscr_ui-2024.4b20/PKG-INFO
```

### Comparing `oscr_ui-2024.3b291/.OSCR_settings.ini` & `oscr_ui-2024.4b20/.OSCR_settings.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [General]
 auto_scan=true
 combats_to_parse=10
 dmg_columns_length=21
 dmg_columns%7C0=true
 dmg_columns%7C1=true
-dmg_columns%7C10=true
-dmg_columns%7C11=true
-dmg_columns%7C12=true
-dmg_columns%7C13=true
-dmg_columns%7C14=true
-dmg_columns%7C15=true
-dmg_columns%7C16=true
-dmg_columns%7C17=true
+dmg_columns%7C10=false
+dmg_columns%7C11=false
+dmg_columns%7C12=false
+dmg_columns%7C13=false
+dmg_columns%7C14=false
+dmg_columns%7C15=false
+dmg_columns%7C16=false
+dmg_columns%7C17=false
 dmg_columns%7C18=true
-dmg_columns%7C19=true
+dmg_columns%7C19=false
 dmg_columns%7C2=true
-dmg_columns%7C20=true
-dmg_columns%7C3=true
+dmg_columns%7C20=false
+dmg_columns%7C3=false
 dmg_columns%7C4=true
 dmg_columns%7C5=true
 dmg_columns%7C6=true
 dmg_columns%7C7=true
 dmg_columns%7C8=true
 dmg_columns%7C9=true
 excluded_event_ids=Autodesc.Combatevent.Falling, 
 favorite_ladders=@Invalid()
 first_overview_tab=0
-geometry=@ByteArray(\x1\xd9\xd0\xcb\0\x3\0\0\0\0\0\0\0\0\0\0\0\0\b4\0\0\x4\xa8\0\0\0\0\0\0\0\0\0\0\x5H\0\0\x3\xf9\0\0\0\0\x2\0\0\0\xf\0\0\0\0\0\0\0\0\0\0\0\b4\0\0\x4\xa8)
+geometry=@ByteArray(\x1\xd9\xd0\xcb\0\x3\0\0\0\0\0\0\0\0\0\0\0\0\a\x8f\0\0\x4\x86\0\0\0\0\0\0\0\0\0\0\x5H\0\0\x3\xf9\0\0\0\0\x2\0\0\0\xf\0\0\0\0\0\0\0\0\0\0\0\a\x8f\0\0\x4\x86)
 graph_resolution=0.2
 heal_columns_length=13
 heal_columns%7C0=true
 heal_columns%7C1=true
 heal_columns%7C10=true
 heal_columns%7C11=true
 heal_columns%7C12=true
```

### Comparing `oscr_ui-2024.3b291/main.py` & `oscr_ui-2024.4b20/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 from OSCRUI import OSCRUI
 
 
 class Launcher():
 
-    version = '2024.3b291'
+    version = '2024.04b020'
     __version__ = '0.1'
 
     # holds the style of the app
     theme = {
         # general style
         'app': {
             'bg': '#1a1a1a',
@@ -657,15 +657,15 @@
         },
         # other style decisions
         's.c': {
             'sidebar_item_width': 0.2,
             'button_icon_size': 24,
             'table_alternate': True,
             'table_gridline': False,
-            'overview_graph_stretch': 12,
+            'overview_graph_stretch': 11,
             'overview_table_stretch': 3
         }
     }
 
     @staticmethod
     def base_path() -> str:
         """initialize the base path"""
@@ -745,14 +745,15 @@
                 'live_columns|4': False,
                 'live_columns|5': False,
                 'live_columns|6': False,
                 'live_parser_opacity': 0.85,
                 'live_graph_active': False,
                 'live_graph_field': 0,
                 'first_overview_tab': 0,
+                'log_size_warning': True,
             }
         }
         return config
 
     @staticmethod
     def launch():
         args = {}
```

### Comparing `oscr_ui-2024.3b291/.github/workflows/build.yml` & `oscr_ui-2024.4b20/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/app.py` & `oscr_ui-2024.4b20/OSCRUI/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         settings = dict()
         for setting_key, settings_type in relevant_settings:
             setting = self.settings.value(setting_key, type=settings_type, defaultValue='')
             if setting:
                 settings[setting_key] = setting
         settings['templog_folder_path'] = self.config['templog_folder_path']
         return settings
-    
+
     @property
     def live_parser_settings(self) -> dict:
         """
         Returns settings relevant to the LiveParser
         """
         return {'seconds_between_combats': self.settings.value('seconds_between_combats', type=int)}
 
@@ -1154,12 +1154,24 @@
         overview_tab_combo = self.create_combo_box(
                 col_2_frame, style_override={'font': '@small_text'})
         overview_tab_combo.addItems(('DPS Bar', 'DPS Graph', 'Damage Graph'))
         overview_tab_combo.setCurrentIndex(self.settings.value('first_overview_tab', type=int))
         overview_tab_combo.currentIndexChanged.connect(
             lambda new_index: self.settings.setValue('first_overview_tab', new_index))
         col_2.addWidget(overview_tab_combo, 11, 1, alignment=ALEFT)
-        
+        size_warning_label = self.create_label('Logfile Size Warning:', 'label_subhead')
+        col_2.addWidget(size_warning_label, 12, 0, alignment=ARIGHT)
+        size_warning_button = FlipButton('Disabled', 'Enabled', col_2_frame, checkable=True)
+        size_warning_button.setStyleSheet(self.get_style_class(
+                'QPushButton', 'toggle_button', override={'margin-top': 0, 'margin-left': 0}))
+        size_warning_button.setFont(self.theme_font('app', '@font'))
+        size_warning_button.r_function = (
+                lambda: self.settings.setValue('log_size_warning', True))
+        size_warning_button.l_function = (
+                lambda: self.settings.setValue('log_size_warning', False))
+        if self.settings.value('log_size_warning', type=bool):
+            size_warning_button.flip()
+        col_2.addWidget(size_warning_button, 12, 1, alignment=ALEFT)
 
         col_2_frame.setLayout(col_2)
 
         settings_frame.setLayout(settings_layout)
```

### Comparing `oscr_ui-2024.3b291/OSCRUI/callbacks.py` & `oscr_ui-2024.4b20/OSCRUI/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from PySide6.QtWidgets import QFileDialog, QLineEdit
 
-from OSCR import LIVE_TABLE_HEADER, split_log_by_combat, split_log_by_lines
+from OSCR import LIVE_TABLE_HEADER, OSCR, split_log_by_combat, split_log_by_lines
 from .iofunctions import browse_path
 from .textedit import format_path
 
 
 def browse_log(self, entry: QLineEdit):
     """
     Callback for browse button.
@@ -241,15 +241,15 @@
     cell_data = data_model._data
     visible_columns = list()
     for i in range(len(LIVE_TABLE_HEADER)):
         visible_columns.append(self.settings.value(f'live_columns|{i}', type=bool))
     output = list()
     for player_name, row in zip(index_data, cell_data):
         output.append(f"{player_name}: {row[0]:,.2f} ({row[1]:.1f}s)")
-    output = '< OSCR > DPS (Combat time): ' + ' | '.join(output)
+    output = '{ OSCR } DPS (Combat time): ' + ' | '.join(output)
     self.app.clipboard().setText(output)
 
 
 def expand_overview_table(self):
     """
     Shows the overview table
     """
@@ -257,7 +257,20 @@
 
 
 def collapse_overview_table(self):
     """
     Hides the overview table
     """
     self.widgets.overview_table_frame.hide()
+
+
+def trim_logfile(self):
+    """
+    Removes all combats but the most recent one from a logfile
+    """
+    log_path = os.path.abspath(self.entry.text())
+    temp_parser = OSCR(log_path, self.parser_settings)
+    if os.path.getsize(log_path) > 125 * 1024 * 1024:
+        temp_parser.analyze_massive_log_file()
+    else:
+        temp_parser.analyze_log_file()
+    temp_parser.export_combat(0, log_path)
```

### Comparing `oscr_ui-2024.3b291/OSCRUI/datafunctions.py` & `oscr_ui-2024.4b20/OSCRUI/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from OSCR import OSCR, HEAL_TREE_HEADER, TREE_HEADER
 from PySide6.QtCore import Qt, QThread, Signal
 
-from .callbacks import switch_main_tab, switch_overview_tab
+from .callbacks import switch_main_tab, switch_overview_tab, trim_logfile
 from .datamodels import DamageTreeModel, HealTreeModel, TreeSelectionModel
 from .displayer import create_overview
 from .subwindows import log_size_warning, show_warning, split_dialog
 from .textedit import format_damage_tree_data, format_heal_tree_data
 
 
 class CustomThread(QThread):
@@ -107,15 +107,15 @@
 
     if not parser.active_combat:
         return
 
     duration = self.parser1.active_combat.duration.total_seconds()
     combat_time = f'{int(duration / 60):02}:{duration % 60:02.0f}'
 
-    summary = f'< OSCR > {parser.active_combat.map}'
+    summary = f'{{ OSCR }} {parser.active_combat.map}'
     difficulty = parser.active_combat.difficulty
     if difficulty and isinstance(difficulty, str) and difficulty != 'Unknown':
         summary += f' ({difficulty}) - DPS [{combat_time}]: '
     else:
         summary += f' - DPS [{combat_time}]: '
     players = sorted(
         self.parser1.active_combat.player_dict.values(),
@@ -140,18 +140,24 @@
 
     # new log file
     if combat is None:
         self.parser1.log_path = path
         try:
             self.parser1.analyze_log_file()
         except FileExistsError:
-            action = log_size_warning(self)
+            if self.settings.value('log_size_warning', type=bool):
+                action = log_size_warning(self)
+            else:
+                action = 'continue'
             if action == 'split dialog':
                 split_dialog(self)
                 return False
+            elif action == 'trim':
+                trim_logfile(self)
+                self.parser1.analyze_log_file()
             elif action == 'continue':
                 self.parser1.analyze_massive_log_file()
             else:
                 return False
         self.parser1.shallow_combat_analysis(0)
 
     # same log file, old combat
@@ -286,15 +292,15 @@
                 column = selected_cell.column()
                 row_name = selected_cell.internalPointer().get_data(0)
                 if row_name not in selection_dict:
                     selection_dict[row_name] = dict()
                 if column != 0:
                     cell_data = selected_cell.internalPointer().get_data(column)
                     selection_dict[row_name][column] = cell_data
-            output = ['< OSCR >']
+            output = ['{ OSCR }']
             for row_name, row_data in selection_dict.items():
                 formatted_row = list()
                 for col, value in row_data.items():
                     formatted_row.append(f'[{current_header[col]}] {format_function(value, col)}')
                 formatted_row_name = ''.join(row_name) if isinstance(row_name, tuple) else row_name
                 output.append(f"{formatted_row_name}: {' | '.join(formatted_row)}")
             output_string = '\n'.join(output)
@@ -311,15 +317,15 @@
             max_one_hits.append((player_item.get_data(max_one_hit_col), player_item))
         max_one_hit, max_one_hit_item = max(max_one_hits, key=lambda x: x[0])
         max_one_hit_ability = max(
                 max_one_hit_item._children, key=lambda x: x.get_data(max_one_hit_col))
         max_one_hit_ability = max_one_hit_ability.get_data(0)
         if isinstance(max_one_hit_ability, tuple):
             max_one_hit_ability = ''.join(max_one_hit_ability)
-        output_string = (f'< OSCR > {prefix}: {max_one_hit:,.2f} '
+        output_string = (f'{{ OSCR }} {prefix}: {max_one_hit:,.2f} '
                          f'({"".join(max_one_hit_item.get_data(0))} – '
                          f'{max_one_hit_ability})')
         self.app.clipboard().setText(output_string)
     elif copy_mode == 'Max One Hit':
         if current_tab <= 1:
             max_one_hit_col = 4
             prefix = 'Max One Hit'
@@ -332,15 +338,15 @@
             if selected_row._children:
                 max_one_hit_item = max(
                         selected_row._children, key=lambda child: child.get_data(max_one_hit_col))
                 max_one_hit = max_one_hit_item.get_data(max_one_hit_col)
                 max_one_hit_ability = max_one_hit_item.get_data(0)
                 if isinstance(max_one_hit_ability, tuple):
                     max_one_hit_ability = ''.join(max_one_hit_ability)
-                output_string = (f'< OSCR > {prefix}: {max_one_hit:,.2f} '
+                output_string = (f'{{ OSCR }} {prefix}: {max_one_hit:,.2f} '
                                  f'({"".join(selected_row.get_data(0))} – '
                                  f'{max_one_hit_ability})')
                 self.app.clipboard().setText(output_string)
     elif copy_mode == 'Magnitude':
         if current_tab == 0:
             prefix = 'Total Damage Out'
         elif current_tab == 1:
@@ -350,15 +356,15 @@
         else:
             prefix = 'Total Heal In'
         magnitudes = list()
         for player_item in current_table.model()._player._children:
             magnitudes.append((player_item.get_data(2), ''.join(player_item.get_data(0))))
         magnitudes.sort(key=lambda x: x[0], reverse=True)
         magnitudes = [f"[{''.join(player)}] {magnitude:,.2f}" for magnitude, player in magnitudes]
-        output_string = (f'< OSCR > {prefix}: {" | ".join(magnitudes)}')
+        output_string = (f'{{ OSCR }} {prefix}: {" | ".join(magnitudes)}')
         self.app.clipboard().setText(output_string)
     elif copy_mode == 'Magnitude / s':
         if current_tab == 0:
             prefix = 'Total DPS Out'
         elif current_tab == 1:
             prefix = 'Total DPS Taken'
         elif current_tab == 2:
@@ -366,9 +372,9 @@
         else:
             prefix = 'Total HPS In'
         magnitudes = list()
         for player_item in current_table.model()._player._children:
             magnitudes.append((player_item.get_data(1), ''.join(player_item.get_data(0))))
         magnitudes.sort(key=lambda x: x[0], reverse=True)
         magnitudes = [f"[{''.join(player)}] {magnitude:,.2f}" for magnitude, player in magnitudes]
-        output_string = (f'< OSCR > {prefix}: {" | ".join(magnitudes)}')
+        output_string = (f'{{ OSCR }} {prefix}: {" | ".join(magnitudes)}')
         self.app.clipboard().setText(output_string)
```

### Comparing `oscr_ui-2024.3b291/OSCRUI/datamodels.py` & `oscr_ui-2024.4b20/OSCRUI/datamodels.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/displayer.py` & `oscr_ui-2024.4b20/OSCRUI/displayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     group_bar_layout = create_grouped_bar_plot(self, DMG_graph_data, time_data)
     self.widgets.overview_tab_frames[2].setLayout(group_bar_layout)
 
     bar_layout = create_horizontal_bar_graph(self, current_table)
     self.widgets.overview_tab_frames[0].setLayout(bar_layout)
 
     table_layout = QVBoxLayout()
-    table_layout.setContentsMargins(0, 0, 0 ,0)
+    table_layout.setContentsMargins(0, 0, 0, 0)
     table = create_overview_table(self, current_table)
     table_layout.addWidget(table)
     self.widgets.overview_table_frame.setLayout(table_layout)
     table.resizeColumnsToContents()
     horizontal_header = table.horizontalHeader()
     for col in range(len(TABLE_HEADER)):
         horizontal_header.resizeSection(col, horizontal_header.sectionSize(col) + 5)
@@ -302,31 +302,30 @@
     plot_widget.setAxisItems({'bottom': CustomPlotAxis('bottom', unit='s')})
     plot_widget.setStyleSheet(get_style(self, 'plot_widget_nullifier'))
     plot_widget.setBackground(None)
     plot_widget.setMouseEnabled(False, False)
     plot_widget.setMenuEnabled(False)
     plot_widget.hideButtons()
     plot_widget.setDefaultPadding(padding=0)
-    plot_widget.setXRange(-9, 0, padding=0)
+    plot_widget.setXRange(-14, 0, padding=0)
     left_axis = plot_widget.getAxis('left')
     left_axis.setTickFont(theme_font(self, 'plot_widget'))
     left_axis.setTextPen(color=self.theme['defaults']['fg'])
     left_axis.setTickDensity(3)
     bottom_axis = plot_widget.getAxis('bottom')
     bottom_axis.setTickFont(theme_font(self, 'plot_widget'))
     bottom_axis.setTextPen(color=self.theme['defaults']['fg'])
 
     curves = list()
     for color_index in range(5):
         color = self.theme['plot']['color_cycler'][color_index]
         curves.append(plot_widget.plot([0], [0], pen=mkPen(color, width=1)))
 
-    frame = create_frame(
-            self, None, 'plot_widget', size_policy=SMIXMAX,
-            style_override={'margin-left': '@margin', 'margin-bottom': 0})
+    frame = create_frame(self, None, 'plot_widget', size_policy=SMIXMAX, style_override={
+            'margin-left': '@margin', 'margin-right': '@margin', 'margin-bottom': 0})
     frame.setMinimumWidth(self.sidebar_item_width * 0.25)
     frame.setMinimumHeight(self.sidebar_item_width * 0.25)
     layout = QHBoxLayout()
     layout.setContentsMargins(0, 0, 0, 0)
     layout.addWidget(plot_widget, stretch=1)
     frame.setLayout(layout)
     return frame, curves
@@ -347,15 +346,15 @@
     cells = list()
     curves = list()
     for player, player_data in data.items():
         index.append(player)
         cells.append(list(player_data.values()))
     if graph_active:
         if len(graph_data_buffer) == 0:
-            graph_data_buffer.extend(([0] * 10, [0] * 10, [0] * 10, [0] * 10, [0] * 10))
+            graph_data_buffer.extend(([0] * 15, [0] * 15, [0] * 15, [0] * 15, [0] * 15))
         zipper = zip(graph_data_buffer, cells, self.widgets.live_parser_curves)
         for buffer_item, player_data, curve in zipper:
             buffer_item.pop(0)
             buffer_item.append(player_data[graph_data_field])
             curves.append((curve, buffer_item))
         if len(curves) > 0:
             self.live_parser_window.update_graph.emit(curves)
@@ -383,10 +382,10 @@
     """
     Updates the graph of the live parser with the supplied data
 
     Parameters:
     - :param curve_data: list containing pairs of curve items and data lists; curve items will be
     updated with the data
     """
-    time_data = list(range(-9, 1))
+    time_data = list(range(-14, 1))
     for curve, data_points in curve_data:
         curve.setData(time_data, data_points)
```

### Comparing `oscr_ui-2024.3b291/OSCRUI/iofunctions.py` & `oscr_ui-2024.4b20/OSCRUI/iofunctions.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/leagueconnector.py` & `oscr_ui-2024.4b20/OSCRUI/leagueconnector.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/style.py` & `oscr_ui-2024.4b20/OSCRUI/style.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/subwindows.py` & `oscr_ui-2024.4b20/OSCRUI/subwindows.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from PySide6.QtGui import QIntValidator, QMouseEvent
 from PySide6.QtWidgets import QAbstractItemView, QDialog
 from PySide6.QtWidgets import QGridLayout, QHBoxLayout, QLineEdit
 from PySide6.QtWidgets import QMessageBox, QSpacerItem, QTableView
 from PySide6.QtWidgets import QVBoxLayout
 
 from OSCR import LiveParser, LIVE_TABLE_HEADER
-from .callbacks import auto_split_callback, combat_split_callback, copy_live_data_callback
+from .callbacks import (
+        auto_split_callback, combat_split_callback, copy_live_data_callback, trim_logfile)
 from .displayer import create_live_graph, update_live_display, update_live_graph, update_live_table
 from .datamodels import LiveParserTableModel
 from .style import get_style, get_style_class, theme_font
 from .textedit import format_path
 from .widgetbuilder import create_button, create_frame, create_icon_button, create_label
 from .widgetbuilder import ABOTTOM, ALEFT, ARIGHT, AVCENTER, RFIXED
 from .widgetbuilder import SEXPAND, SMAX, SMAXMAX, SMINMIN
@@ -50,20 +51,23 @@
             'the file, "Cancel" to abort combatlog analysis or "Continue" to analyze the log '
             'nevertheless.')
     dialog.setText(message)
     dialog.setWindowTitle('Open Source Combalog Reader')
     dialog.setWindowIcon(self.icons['oscr'])
     dialog.addButton('Cancel', QMessageBox.ButtonRole.RejectRole)
     default_button = dialog.addButton('Split Dialog', QMessageBox.ButtonRole.ActionRole)
+    dialog.addButton('Trim', QMessageBox.ButtonRole.ActionRole)
     dialog.addButton('Continue', QMessageBox.ButtonRole.AcceptRole)
     dialog.setDefaultButton(default_button)
     clicked = dialog.exec()
     if clicked == 1:
         return 'split dialog'
     elif clicked == 2:
+        return 'trim'
+    elif clicked == 3:
         return 'continue'
     else:
         return 'cancel'
 
 
 def split_dialog(self):
     """
@@ -92,44 +96,63 @@
     seperator_1.setFixedHeight(self.theme['hr']['height'])
     vertical_layout.addWidget(seperator_1)
     grid_layout = QGridLayout()
     grid_layout.setContentsMargins(0, 0, 0, 0)
     grid_layout.setVerticalSpacing(0)
     grid_layout.setHorizontalSpacing(item_spacing)
     vertical_layout.addLayout(grid_layout)
+
+    trim_heading = create_label(self, 'Trim Logfile:', 'label_heading')
+    grid_layout.addWidget(trim_heading, 0, 0, alignment=ALEFT)
+    label_text = (
+            'Removes all combats but the most recent one from the selected logfile. '
+            'All previous combats will be lost!')
+    trim_text = create_label(self, label_text, 'label')
+    trim_text.setWordWrap(True)
+    trim_text.setFixedWidth(self.sidebar_item_width)
+    grid_layout.addWidget(trim_text, 1, 0, alignment=ALEFT)
+    trim_button = create_button(self, 'Trim')
+    trim_button.clicked.connect(lambda: trim_logfile(self))
+    grid_layout.addWidget(trim_button, 1, 2, alignment=ARIGHT | ABOTTOM)
+    grid_layout.setRowMinimumHeight(2, item_spacing)
+    seperator_8 = create_frame(self, content_frame, 'hr', size_policy=SMINMIN)
+    seperator_8.setFixedHeight(self.theme['hr']['height'])
+    grid_layout.addWidget(seperator_8, 3, 0, 1, 3)
+    grid_layout.setRowMinimumHeight(4, item_spacing)
+
     auto_split_heading = create_label(self, 'Split Log Automatically:', 'label_heading')
-    grid_layout.addWidget(auto_split_heading, 0, 0, alignment=ALEFT)
+    grid_layout.addWidget(auto_split_heading, 5, 0, alignment=ALEFT)
     label_text = (
             'Automatically splits the logfile at the next combat end after '
             f'{self.settings.value("split_log_after", type=int):,} lines until the entire file has '
             ' been split. The new files are written to the selected folder. It is advised to '
             'select an empty folder to ensure all files are saved correctly.')
     auto_split_text = create_label(self, label_text, 'label')
     auto_split_text.setWordWrap(True)
     auto_split_text.setFixedWidth(self.sidebar_item_width)
-    grid_layout.addWidget(auto_split_text, 1, 0, alignment=ALEFT)
+    grid_layout.addWidget(auto_split_text, 6, 0, alignment=ALEFT)
     auto_split_button = create_button(self, 'Auto Split')
     auto_split_button.clicked.connect(lambda: auto_split_callback(self, current_logpath))
-    grid_layout.addWidget(auto_split_button, 1, 2, alignment=ARIGHT | ABOTTOM)
-    grid_layout.setRowMinimumHeight(2, item_spacing)
-    seperator_3 = create_frame(self, content_frame, 'hr', size_policy=SMINMIN)
-    seperator_3.setFixedHeight(self.theme['hr']['height'])
-    grid_layout.addWidget(seperator_3, 3, 0, 1, 3)
-    grid_layout.setRowMinimumHeight(4, item_spacing)
+    grid_layout.addWidget(auto_split_button, 6, 2, alignment=ARIGHT | ABOTTOM)
+    grid_layout.setRowMinimumHeight(7, item_spacing)
+    seperator_8 = create_frame(self, content_frame, 'hr', size_policy=SMINMIN)
+    seperator_8.setFixedHeight(self.theme['hr']['height'])
+    grid_layout.addWidget(seperator_8, 8, 0, 1, 3)
+    grid_layout.setRowMinimumHeight(9, item_spacing)
     range_split_heading = create_label(self, 'Export Range of Combats:', 'label_heading')
-    grid_layout.addWidget(range_split_heading, 5, 0, alignment=ALEFT)
+    grid_layout.addWidget(range_split_heading, 10, 0, alignment=ALEFT)
     label_text = (
             'Exports combats including and between lower and upper limit to selected file. '
             'Both limits refer to the indexed list of all combats in the file starting with 1. '
             'An upper limit larger than the total number of combats or of "-1", is treated as '
             'being equal to the total number of combats.')
     range_split_text = create_label(self, label_text, 'label')
     range_split_text.setWordWrap(True)
     range_split_text.setFixedWidth(self.sidebar_item_width)
-    grid_layout.addWidget(range_split_text, 6, 0, alignment=ALEFT)
+    grid_layout.addWidget(range_split_text, 11, 0, alignment=ALEFT)
     range_limit_layout = QGridLayout()
     range_limit_layout.setContentsMargins(0, 0, 0, 0)
     range_limit_layout.setSpacing(0)
     range_limit_layout.setRowStretch(0, 1)
     lower_range_label = create_label(self, 'Lower Limit:', 'label')
     range_limit_layout.addWidget(lower_range_label, 1, 0, alignment=AVCENTER)
     upper_range_label = create_label(self, 'Upper Limit:', 'label')
@@ -148,20 +171,20 @@
     upper_validator.setBottom(-1)
     upper_range_entry.setValidator(upper_validator)
     upper_range_entry.setText('1')
     upper_range_entry.setStyleSheet(
             get_style(self, 'entry', {'margin-top': 0, 'margin-left': '@csp'}))
     upper_range_entry.setFixedWidth(self.sidebar_item_width // 7)
     range_limit_layout.addWidget(upper_range_entry, 2, 1, alignment=AVCENTER)
-    grid_layout.addLayout(range_limit_layout, 6, 1)
+    grid_layout.addLayout(range_limit_layout, 11, 1)
     range_split_button = create_button(self, 'Export Combats')
     range_split_button.clicked.connect(
             lambda le=lower_range_entry, ue=upper_range_entry:
             combat_split_callback(self, current_logpath, le.text(), ue.text()))
-    grid_layout.addWidget(range_split_button, 6, 2, alignment=ARIGHT | ABOTTOM)
+    grid_layout.addWidget(range_split_button, 11, 2, alignment=ARIGHT | ABOTTOM)
 
     content_frame.setLayout(vertical_layout)
 
     dialog = QDialog(self.window)
     dialog.setLayout(main_layout)
     dialog.setWindowTitle('OSCR - Split Logfile')
     dialog.setStyleSheet(get_style(self, 'dialog_window'))
```

### Comparing `oscr_ui-2024.3b291/OSCRUI/textedit.py` & `oscr_ui-2024.4b20/OSCRUI/textedit.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/widgetbuilder.py` & `oscr_ui-2024.4b20/OSCRUI/widgetbuilder.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/OSCRUI/widgets.py` & `oscr_ui-2024.4b20/OSCRUI/widgets.py`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/Overpass-Bold.ttf` & `oscr_ui-2024.4b20/assets/Overpass-Bold.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/Overpass-Medium.ttf` & `oscr_ui-2024.4b20/assets/Overpass-Medium.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/Overpass-Regular.ttf` & `oscr_ui-2024.4b20/assets/Overpass-Regular.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/RobotoMono-Medium.ttf` & `oscr_ui-2024.4b20/assets/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/RobotoMono-Regular.ttf` & `oscr_ui-2024.4b20/assets/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/gear.svg` & `oscr_ui-2024.4b20/assets/gear.svg`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/loading.png` & `oscr_ui-2024.4b20/assets/loading.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/oscr_icon_small.ico` & `oscr_ui-2024.4b20/assets/oscr_icon_small.ico`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/oscr_icon_small.png` & `oscr_ui-2024.4b20/assets/oscr_icon_small.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/oscrbanner-slim-dark-label.png` & `oscr_ui-2024.4b20/assets/oscrbanner-slim-dark-label.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/oscrbanner-slim-dark.png` & `oscr_ui-2024.4b20/assets/oscrbanner-slim-dark.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/oscrbanner-slim.png` & `oscr_ui-2024.4b20/assets/oscrbanner-slim.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/section31badge.png` & `oscr_ui-2024.4b20/assets/section31badge.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/assets/stobuildslogo.png` & `oscr_ui-2024.4b20/assets/stobuildslogo.png`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/LICENSE` & `oscr_ui-2024.4b20/LICENSE`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/README.md` & `oscr_ui-2024.4b20/README.md`

 * *Files identical despite different names*

### Comparing `oscr_ui-2024.3b291/pyproject.toml` & `oscr_ui-2024.4b20/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "OSCR-UI"
 dependencies = [
   "PySide6>=6.6.0",
   "pyqtgraph>=0.13.4",
   "numpy>=1.26.1",
-  "STO-OSCR>=2024.3b261",
+  "STO-OSCR>=2024.4b20",
   "OSCR-django-client>=2024.3b40",
 ]
 requires-python = ">=3.10"
 authors = []
 maintainers = []
 description = " Frontend for the OSCR parser."
 readme = "README.md"
```

### Comparing `oscr_ui-2024.3b291/PKG-INFO` & `oscr_ui-2024.4b20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: OSCR-UI
-Version: 2024.3b291
+Version: 2024.4b20
 Summary:  Frontend for the OSCR parser.
 Project-URL: Homepage, https://github.com/STOCD/OSCR-UI
 Project-URL: Repository, https://github.com/STOCD/OSCR-UI.git
 Project-URL: Bug Tracker, https://github.com/STOCD/OSCR-UI/issues
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -683,15 +683,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: oscr-django-client>=2024.3b40
 Requires-Dist: pyqtgraph>=0.13.4
 Requires-Dist: pyside6>=6.6.0
-Requires-Dist: sto-oscr>=2024.3b261
+Requires-Dist: sto-oscr>=2024.4b20
 Provides-Extra: cli
 Provides-Extra: gui
 Description-Content-Type: text/markdown
 
 # OSCR-UI
 
 [![PyPI version](https://badge.fury.io/py/OSCR-UI.svg)](https://badge.fury.io/py/OSCR-UI)
```

