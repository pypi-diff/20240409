# Comparing `tmp/sliceitoff-0.3b0.tar.gz` & `tmp/sliceitoff-0.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceitoff-0.3b0.tar", max compression
+gzip compressed data, was "sliceitoff-0.3b1.tar", max compression
```

## Comparing `sliceitoff-0.3b0.tar` & `sliceitoff-0.3b1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
--rw-r--r--   0        0        0    18092 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/LICENSE.txt
--rw-r--r--   0        0        0      998 2024-04-08 20:29:10.619811 sliceitoff-0.3b0/README.txt
--rw-r--r--   0        0        0      837 2024-04-08 20:29:32.956942 sliceitoff-0.3b0/pyproject.toml
--rw-r--r--   0        0        0      143 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/__main__.py
--rw-r--r--   0        0        0       84 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/assets/fonts.lst
--rw-r--r--   0        0        0      213 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.DE
--rw-r--r--   0        0        0      208 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.FR
--rw-r--r--   0        0        0      606 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM
--rw-r--r--   0        0        0      207 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.SV
--rw-r--r--   0        0        0      211 2024-04-08 14:33:13.397835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.TR
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT
--rw-r--r--   0        0        0      186 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/display/__init__.py
--rw-r--r--   0        0        0     1661 2024-04-08 15:50:01.476357 sliceitoff-0.3b0/src/sliceitoff/display/display.py
--rw-r--r--   0        0        0     3234 2024-04-08 17:50:32.660333 sliceitoff-0.3b0/src/sliceitoff/display/scaling.py
--rw-r--r--   0        0        0      680 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/display/static.py
--rw-r--r--   0        0        0       77 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/enemies/__init__.py
--rw-r--r--   0        0        0      984 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/enemies/ball.py
--rw-r--r--   0        0        0     1375 2024-04-08 14:33:13.402835 sliceitoff-0.3b0/src/sliceitoff/enemies/bouncher.py
--rw-r--r--   0        0        0     1301 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/enemies/enemies.py
--rw-r--r--   0        0        0     1299 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/enemies/enemy.py
--rw-r--r--   0        0        0       72 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/field/__init__.py
--rw-r--r--   0        0        0     5000 2024-04-08 17:43:45.838360 sliceitoff-0.3b0/src/sliceitoff/field/field.py
--rw-r--r--   0        0        0      113 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/game/__init__.py
--rw-r--r--   0        0        0      302 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/game/anykey.py
--rw-r--r--   0        0        0     1019 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/game/explodeout.py
--rw-r--r--   0        0        0     2953 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/game/game.py
--rw-r--r--   0        0        0     2163 2024-04-08 17:37:54.535912 sliceitoff-0.3b0/src/sliceitoff/game/gameplay.py
--rw-r--r--   0        0        0     1815 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/game/initials.py
--rw-r--r--   0        0        0     2163 2024-04-08 18:00:26.116871 sliceitoff-0.3b0/src/sliceitoff/game/level.py
--rw-r--r--   0        0        0      809 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/game/show.py
--rw-r--r--   0        0        0       83 2024-04-08 14:33:13.403835 sliceitoff-0.3b0/src/sliceitoff/hiscores/__init__.py
--rw-r--r--   0        0        0     2723 2024-04-08 20:47:50.294397 sliceitoff-0.3b0/src/sliceitoff/hiscores/hiscores.py
--rw-r--r--   0        0        0      493 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/hiscores/static.py
--rw-r--r--   0        0        0      275 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/main.py
--rw-r--r--   0        0        0      100 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/mainmenu/__init__.py
--rw-r--r--   0        0        0     2415 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/mainmenu/mainmenu.py
--rw-r--r--   0        0        0       98 2024-04-08 17:31:35.995903 sliceitoff-0.3b0/src/sliceitoff/player/__init__.py
--rw-r--r--   0        0        0     1541 2024-04-08 20:19:11.595260 sliceitoff-0.3b0/src/sliceitoff/player/life.py
--rw-r--r--   0        0        0     1974 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/player/player.py
--rw-r--r--   0        0        0     1067 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/player/static.py
--rw-r--r--   0        0        0      412 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/__init__.py
--rw-r--r--   0        0        0      327 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/gameover.py
--rw-r--r--   0        0        0      380 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/hiscores.py
--rw-r--r--   0        0        0      505 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/initials.py
--rw-r--r--   0        0        0      758 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/instructions1.py
--rw-r--r--   0        0        0      837 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/instructions2.py
--rw-r--r--   0        0        0      316 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/level.py
--rw-r--r--   0        0        0     1116 2024-04-08 14:33:13.404835 sliceitoff-0.3b0/src/sliceitoff/screens/levelup.py
--rw-r--r--   0        0        0      811 2024-04-08 15:46:44.803620 sliceitoff-0.3b0/src/sliceitoff/screens/mainmenu.py
--rw-r--r--   0        0        0       98 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/stats/__init__.py
--rw-r--r--   0        0        0     1435 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/stats/stats.py
--rw-r--r--   0        0        0       95 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/status/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/status/status.py
--rw-r--r--   0        0        0      178 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/text/__init__.py
--rw-r--r--   0        0        0      929 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/text/explode.py
--rw-r--r--   0        0        0     1520 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/text/fonts.py
--rw-r--r--   0        0        0     2671 2024-04-08 14:33:13.405835 sliceitoff-0.3b0/src/sliceitoff/text/text.py
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 sliceitoff-0.3b0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/LICENSE.txt
+-rw-r--r--   0        0        0      998 2024-04-08 20:29:10.619811 sliceitoff-0.3b1/README.txt
+-rw-r--r--   0        0        0      839 2024-04-08 21:43:19.437127 sliceitoff-0.3b1/pyproject.toml
+-rw-r--r--   0        0        0      143 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/__main__.py
+-rw-r--r--   0        0        0       84 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/fonts.lst
+-rw-r--r--   0        0        0      213 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.DE
+-rw-r--r--   0        0        0      208 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.FR
+-rw-r--r--   0        0        0      606 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM
+-rw-r--r--   0        0        0      207 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.SV
+-rw-r--r--   0        0        0      211 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.TR
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT
+-rw-r--r--   0        0        0      186 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/display/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-08 15:50:01.476357 sliceitoff-0.3b1/src/sliceitoff/display/display.py
+-rw-r--r--   0        0        0     3234 2024-04-08 17:50:32.660333 sliceitoff-0.3b1/src/sliceitoff/display/scaling.py
+-rw-r--r--   0        0        0      680 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/display/static.py
+-rw-r--r--   0        0        0       77 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/enemies/__init__.py
+-rw-r--r--   0        0        0      984 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/enemies/ball.py
+-rw-r--r--   0        0        0     1375 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/enemies/bouncher.py
+-rw-r--r--   0        0        0     1301 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/enemies/enemies.py
+-rw-r--r--   0        0        0     1299 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/enemies/enemy.py
+-rw-r--r--   0        0        0       72 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/field/__init__.py
+-rw-r--r--   0        0        0     5000 2024-04-08 17:43:45.838360 sliceitoff-0.3b1/src/sliceitoff/field/field.py
+-rw-r--r--   0        0        0      113 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/anykey.py
+-rw-r--r--   0        0        0     1019 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/explodeout.py
+-rw-r--r--   0        0        0     2953 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/game.py
+-rw-r--r--   0        0        0     2163 2024-04-08 17:37:54.535912 sliceitoff-0.3b1/src/sliceitoff/game/gameplay.py
+-rw-r--r--   0        0        0     1815 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/initials.py
+-rw-r--r--   0        0        0     2163 2024-04-08 18:00:26.116871 sliceitoff-0.3b1/src/sliceitoff/game/level.py
+-rw-r--r--   0        0        0      809 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/show.py
+-rw-r--r--   0        0        0       83 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/hiscores/__init__.py
+-rw-r--r--   0        0        0     2702 2024-04-08 21:42:16.610756 sliceitoff-0.3b1/src/sliceitoff/hiscores/hiscores.py
+-rw-r--r--   0        0        0      493 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/hiscores/static.py
+-rw-r--r--   0        0        0      275 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/main.py
+-rw-r--r--   0        0        0      100 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/mainmenu/__init__.py
+-rw-r--r--   0        0        0     2415 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/mainmenu/mainmenu.py
+-rw-r--r--   0        0        0       98 2024-04-08 17:31:35.995903 sliceitoff-0.3b1/src/sliceitoff/player/__init__.py
+-rw-r--r--   0        0        0     1541 2024-04-08 20:19:11.595260 sliceitoff-0.3b1/src/sliceitoff/player/life.py
+-rw-r--r--   0        0        0     1974 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/player/player.py
+-rw-r--r--   0        0        0     1067 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/player/static.py
+-rw-r--r--   0        0        0      412 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/gameover.py
+-rw-r--r--   0        0        0      380 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/hiscores.py
+-rw-r--r--   0        0        0      505 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/initials.py
+-rw-r--r--   0        0        0      758 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/instructions1.py
+-rw-r--r--   0        0        0      837 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/instructions2.py
+-rw-r--r--   0        0        0      316 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/level.py
+-rw-r--r--   0        0        0     1116 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/levelup.py
+-rw-r--r--   0        0        0      811 2024-04-08 15:46:44.803620 sliceitoff-0.3b1/src/sliceitoff/screens/mainmenu.py
+-rw-r--r--   0        0        0       98 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/stats/__init__.py
+-rw-r--r--   0        0        0     1435 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/stats/stats.py
+-rw-r--r--   0        0        0       95 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/status/__init__.py
+-rw-r--r--   0        0        0     1122 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/status/status.py
+-rw-r--r--   0        0        0      178 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/explode.py
+-rw-r--r--   0        0        0     1520 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/fonts.py
+-rw-r--r--   0        0        0     2671 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/text.py
+-rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 sliceitoff-0.3b1/PKG-INFO
```

### Comparing `sliceitoff-0.3b0/LICENSE.txt` & `sliceitoff-0.3b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/README.txt` & `sliceitoff-0.3b1/README.txt`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/pyproject.toml` & `sliceitoff-0.3b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sliceitoff"
-version = "0.3-beta"
+version = "0.3-beta.1"
 description = "Arcade game where one slices play area off avoiding enemies."
 authors = ["Viljami Ilola <+@hix.fi>"]
 readme = "README.txt"
 packages = [{include = "sliceitoff", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT` & `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/display/display.py` & `sliceitoff-0.3b1/src/sliceitoff/display/display.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/display/scaling.py` & `sliceitoff-0.3b1/src/sliceitoff/display/scaling.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/display/static.py` & `sliceitoff-0.3b1/src/sliceitoff/display/static.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/enemies/ball.py` & `sliceitoff-0.3b1/src/sliceitoff/enemies/ball.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/enemies/bouncher.py` & `sliceitoff-0.3b1/src/sliceitoff/enemies/bouncher.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/enemies/enemies.py` & `sliceitoff-0.3b1/src/sliceitoff/enemies/enemies.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/enemies/enemy.py` & `sliceitoff-0.3b1/src/sliceitoff/enemies/enemy.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/field/field.py` & `sliceitoff-0.3b1/src/sliceitoff/field/field.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/game/explodeout.py` & `sliceitoff-0.3b1/src/sliceitoff/game/explodeout.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/game/game.py` & `sliceitoff-0.3b1/src/sliceitoff/game/game.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/game/gameplay.py` & `sliceitoff-0.3b1/src/sliceitoff/game/gameplay.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/game/initials.py` & `sliceitoff-0.3b1/src/sliceitoff/game/initials.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/game/level.py` & `sliceitoff-0.3b1/src/sliceitoff/game/level.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/game/show.py` & `sliceitoff-0.3b1/src/sliceitoff/game/show.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/hiscores/hiscores.py` & `sliceitoff-0.3b1/src/sliceitoff/hiscores/hiscores.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,17 +17,17 @@
                     ".config",
                     "sliceitoffrc")
         if not os.path.isfile(self.config_filename):
             self.table=INITIAL_HIGHSCORES[:]
             return
         with open(self.config_filename, "r", encoding="utf-8") as config_file:
             for line in config_file:
-                option, value = line.split('=')
-                if option == 'hiscore':
-                    score, name = value.split('!')
+                option, *value = line.split('=')
+                if option == 'hiscore' and value:
+                    score, name = value[0].split('!')
                     self.add(int(score.strip()),name.strip())
         if len(self.table)<MAX_HIGHSCORES:
             self.table+=[(0,"") for _ in range(MAX_HIGHSCORES-len(self.table))]
 
     def add(self, score, initials):
         """ Add new high score and reranks top """
         self.table.append( (score, initials) )
@@ -41,22 +41,21 @@
     def __del__(self):
         """ On object deletion save current high scores to config file """
         oldlines=[]
         if os.path.isfile(self.config_filename):
             with (open(self.config_filename, "r", encoding="utf-8")
                     as config_file):
                 for line in config_file:
-                    option, _ = line.split('=')
+                    option, *_ = line.split('=')
                     if option != 'hiscore':
                         oldlines.append(line)
         with open(self.config_filename, 'w', encoding="utf-8") as config_file:
             config_file.writelines(oldlines)
             for score, name in self.table:
                 config_file.write(f"hiscore={score}!{name}\n")
-            config_file.write("\n")
 
     def __str__(self):
         text = (
                 "      "
                 "\xeeH\xecI\xedG\xe9H "
                 "\xeaS\xedC\xeeO\xebR\xe9E\xecS\xeb!\xed!\n\n")
         half = len(self.table) // 2
```

### Comparing `sliceitoff-0.3b0/src/sliceitoff/mainmenu/mainmenu.py` & `sliceitoff-0.3b1/src/sliceitoff/mainmenu/mainmenu.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/player/life.py` & `sliceitoff-0.3b1/src/sliceitoff/player/life.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/player/player.py` & `sliceitoff-0.3b1/src/sliceitoff/player/player.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/player/static.py` & `sliceitoff-0.3b1/src/sliceitoff/player/static.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/screens/instructions1.py` & `sliceitoff-0.3b1/src/sliceitoff/screens/instructions1.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/screens/instructions2.py` & `sliceitoff-0.3b1/src/sliceitoff/screens/instructions2.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/screens/levelup.py` & `sliceitoff-0.3b1/src/sliceitoff/screens/levelup.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/screens/mainmenu.py` & `sliceitoff-0.3b1/src/sliceitoff/screens/mainmenu.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/stats/stats.py` & `sliceitoff-0.3b1/src/sliceitoff/stats/stats.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/status/status.py` & `sliceitoff-0.3b1/src/sliceitoff/status/status.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/text/explode.py` & `sliceitoff-0.3b1/src/sliceitoff/text/explode.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/text/fonts.py` & `sliceitoff-0.3b1/src/sliceitoff/text/fonts.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/src/sliceitoff/text/text.py` & `sliceitoff-0.3b1/src/sliceitoff/text/text.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b0/PKG-INFO` & `sliceitoff-0.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliceitoff
-Version: 0.3b0
+Version: 0.3b1
 Summary: Arcade game where one slices play area off avoiding enemies.
 Author: Viljami Ilola
 Author-email: +@hix.fi
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

