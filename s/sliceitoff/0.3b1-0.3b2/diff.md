# Comparing `tmp/sliceitoff-0.3b1.tar.gz` & `tmp/sliceitoff-0.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceitoff-0.3b1.tar", max compression
+gzip compressed data, was "sliceitoff-0.3b2.tar", max compression
```

## Comparing `sliceitoff-0.3b1.tar` & `sliceitoff-0.3b2.tar`

### file list

```diff
@@ -1,116 +1,115 @@
--rw-r--r--   0        0        0    18092 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/LICENSE.txt
--rw-r--r--   0        0        0      998 2024-04-08 20:29:10.619811 sliceitoff-0.3b1/README.txt
--rw-r--r--   0        0        0      839 2024-04-08 21:43:19.437127 sliceitoff-0.3b1/pyproject.toml
--rw-r--r--   0        0        0      143 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/__main__.py
--rw-r--r--   0        0        0       84 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/fonts.lst
--rw-r--r--   0        0        0      213 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.DE
--rw-r--r--   0        0        0      208 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.FR
--rw-r--r--   0        0        0      606 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM
--rw-r--r--   0        0        0      207 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.SV
--rw-r--r--   0        0        0      211 2024-04-08 14:33:13.397835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.TR
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT
--rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT
--rw-r--r--   0        0        0      186 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/display/__init__.py
--rw-r--r--   0        0        0     1661 2024-04-08 15:50:01.476357 sliceitoff-0.3b1/src/sliceitoff/display/display.py
--rw-r--r--   0        0        0     3234 2024-04-08 17:50:32.660333 sliceitoff-0.3b1/src/sliceitoff/display/scaling.py
--rw-r--r--   0        0        0      680 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/display/static.py
--rw-r--r--   0        0        0       77 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/enemies/__init__.py
--rw-r--r--   0        0        0      984 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/enemies/ball.py
--rw-r--r--   0        0        0     1375 2024-04-08 14:33:13.402835 sliceitoff-0.3b1/src/sliceitoff/enemies/bouncher.py
--rw-r--r--   0        0        0     1301 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/enemies/enemies.py
--rw-r--r--   0        0        0     1299 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/enemies/enemy.py
--rw-r--r--   0        0        0       72 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/field/__init__.py
--rw-r--r--   0        0        0     5000 2024-04-08 17:43:45.838360 sliceitoff-0.3b1/src/sliceitoff/field/field.py
--rw-r--r--   0        0        0      113 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/__init__.py
--rw-r--r--   0        0        0      302 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/anykey.py
--rw-r--r--   0        0        0     1019 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/explodeout.py
--rw-r--r--   0        0        0     2953 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/game.py
--rw-r--r--   0        0        0     2163 2024-04-08 17:37:54.535912 sliceitoff-0.3b1/src/sliceitoff/game/gameplay.py
--rw-r--r--   0        0        0     1815 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/initials.py
--rw-r--r--   0        0        0     2163 2024-04-08 18:00:26.116871 sliceitoff-0.3b1/src/sliceitoff/game/level.py
--rw-r--r--   0        0        0      809 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/game/show.py
--rw-r--r--   0        0        0       83 2024-04-08 14:33:13.403835 sliceitoff-0.3b1/src/sliceitoff/hiscores/__init__.py
--rw-r--r--   0        0        0     2702 2024-04-08 21:42:16.610756 sliceitoff-0.3b1/src/sliceitoff/hiscores/hiscores.py
--rw-r--r--   0        0        0      493 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/hiscores/static.py
--rw-r--r--   0        0        0      275 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/main.py
--rw-r--r--   0        0        0      100 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/mainmenu/__init__.py
--rw-r--r--   0        0        0     2415 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/mainmenu/mainmenu.py
--rw-r--r--   0        0        0       98 2024-04-08 17:31:35.995903 sliceitoff-0.3b1/src/sliceitoff/player/__init__.py
--rw-r--r--   0        0        0     1541 2024-04-08 20:19:11.595260 sliceitoff-0.3b1/src/sliceitoff/player/life.py
--rw-r--r--   0        0        0     1974 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/player/player.py
--rw-r--r--   0        0        0     1067 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/player/static.py
--rw-r--r--   0        0        0      412 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/__init__.py
--rw-r--r--   0        0        0      327 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/gameover.py
--rw-r--r--   0        0        0      380 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/hiscores.py
--rw-r--r--   0        0        0      505 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/initials.py
--rw-r--r--   0        0        0      758 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/instructions1.py
--rw-r--r--   0        0        0      837 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/instructions2.py
--rw-r--r--   0        0        0      316 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/level.py
--rw-r--r--   0        0        0     1116 2024-04-08 14:33:13.404835 sliceitoff-0.3b1/src/sliceitoff/screens/levelup.py
--rw-r--r--   0        0        0      811 2024-04-08 15:46:44.803620 sliceitoff-0.3b1/src/sliceitoff/screens/mainmenu.py
--rw-r--r--   0        0        0       98 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/stats/__init__.py
--rw-r--r--   0        0        0     1435 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/stats/stats.py
--rw-r--r--   0        0        0       95 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/status/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/status/status.py
--rw-r--r--   0        0        0      178 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/__init__.py
--rw-r--r--   0        0        0      929 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/explode.py
--rw-r--r--   0        0        0     1520 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/fonts.py
--rw-r--r--   0        0        0     2671 2024-04-08 14:33:13.405835 sliceitoff-0.3b1/src/sliceitoff/text/text.py
--rw-r--r--   0        0        0     1475 1970-01-01 00:00:00.000000 sliceitoff-0.3b1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/LICENSE.txt
+-rw-r--r--   0        0        0     1065 2024-04-08 21:56:04.160643 sliceitoff-0.3b2/README.txt
+-rw-r--r--   0        0        0      893 2024-04-08 22:54:09.424171 sliceitoff-0.3b2/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/src/sliceitoff/assets/fonts.lst
+-rw-r--r--   0        0        0      213 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.DE
+-rw-r--r--   0        0        0      208 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.FR
+-rw-r--r--   0        0        0      606 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM
+-rw-r--r--   0        0        0      207 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.SV
+-rw-r--r--   0        0        0      211 2024-04-08 14:33:13.397835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.TR
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.398835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.399835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.400835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.401835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT
+-rw-r--r--   0        0        0     4096 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT
+-rw-r--r--   0        0        0      186 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/display/__init__.py
+-rw-r--r--   0        0        0     1661 2024-04-08 15:50:01.476357 sliceitoff-0.3b2/src/sliceitoff/display/display.py
+-rw-r--r--   0        0        0     3234 2024-04-08 17:50:32.660333 sliceitoff-0.3b2/src/sliceitoff/display/scaling.py
+-rw-r--r--   0        0        0      680 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/display/static.py
+-rw-r--r--   0        0        0       77 2024-04-08 14:33:13.402835 sliceitoff-0.3b2/src/sliceitoff/enemies/__init__.py
+-rw-r--r--   0        0        0      995 2024-04-08 22:43:01.935260 sliceitoff-0.3b2/src/sliceitoff/enemies/ball.py
+-rw-r--r--   0        0        0     1386 2024-04-08 22:43:07.887295 sliceitoff-0.3b2/src/sliceitoff/enemies/bouncher.py
+-rw-r--r--   0        0        0     1301 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/enemies/enemies.py
+-rw-r--r--   0        0        0     1310 2024-04-08 22:43:19.776364 sliceitoff-0.3b2/src/sliceitoff/enemies/enemy.py
+-rw-r--r--   0        0        0       72 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/field/__init__.py
+-rw-r--r--   0        0        0     5022 2024-04-08 22:43:32.039436 sliceitoff-0.3b2/src/sliceitoff/field/field.py
+-rw-r--r--   0        0        0      113 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/game/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/game/anykey.py
+-rw-r--r--   0        0        0     1019 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/game/explodeout.py
+-rw-r--r--   0        0        0     3019 2024-04-08 22:44:01.672609 sliceitoff-0.3b2/src/sliceitoff/game/game.py
+-rw-r--r--   0        0        0     2163 2024-04-08 17:37:54.535912 sliceitoff-0.3b2/src/sliceitoff/game/gameplay.py
+-rw-r--r--   0        0        0     1826 2024-04-08 22:44:16.831697 sliceitoff-0.3b2/src/sliceitoff/game/initials.py
+-rw-r--r--   0        0        0     2218 2024-04-08 22:44:31.152781 sliceitoff-0.3b2/src/sliceitoff/game/level.py
+-rw-r--r--   0        0        0      809 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/game/show.py
+-rw-r--r--   0        0        0       83 2024-04-08 14:33:13.403835 sliceitoff-0.3b2/src/sliceitoff/hiscores/__init__.py
+-rw-r--r--   0        0        0     2701 2024-04-08 22:51:08.487108 sliceitoff-0.3b2/src/sliceitoff/hiscores/hiscores.py
+-rw-r--r--   0        0        0      493 2024-04-08 14:33:13.404835 sliceitoff-0.3b2/src/sliceitoff/hiscores/static.py
+-rw-r--r--   0        0        0      170 2024-04-08 22:50:37.134924 sliceitoff-0.3b2/src/sliceitoff/main.py
+-rw-r--r--   0        0        0      100 2024-04-08 14:33:13.404835 sliceitoff-0.3b2/src/sliceitoff/mainmenu/__init__.py
+-rw-r--r--   0        0        0     2448 2024-04-08 22:45:07.560994 sliceitoff-0.3b2/src/sliceitoff/mainmenu/mainmenu.py
+-rw-r--r--   0        0        0       98 2024-04-08 17:31:35.995903 sliceitoff-0.3b2/src/sliceitoff/player/__init__.py
+-rw-r--r--   0        0        0     1562 2024-04-08 22:45:21.050073 sliceitoff-0.3b2/src/sliceitoff/player/life.py
+-rw-r--r--   0        0        0     1985 2024-04-08 22:45:28.074114 sliceitoff-0.3b2/src/sliceitoff/player/player.py
+-rw-r--r--   0        0        0     1079 2024-04-08 22:45:34.658152 sliceitoff-0.3b2/src/sliceitoff/player/static.py
+-rw-r--r--   0        0        0      412 2024-04-08 14:33:13.404835 sliceitoff-0.3b2/src/sliceitoff/screens/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-08 22:45:42.274197 sliceitoff-0.3b2/src/sliceitoff/screens/gameover.py
+-rw-r--r--   0        0        0      391 2024-04-08 22:45:46.122219 sliceitoff-0.3b2/src/sliceitoff/screens/hiscores.py
+-rw-r--r--   0        0        0      516 2024-04-08 22:45:50.297244 sliceitoff-0.3b2/src/sliceitoff/screens/initials.py
+-rw-r--r--   0        0        0      769 2024-04-08 22:45:55.626275 sliceitoff-0.3b2/src/sliceitoff/screens/instructions1.py
+-rw-r--r--   0        0        0      848 2024-04-08 22:45:58.930294 sliceitoff-0.3b2/src/sliceitoff/screens/instructions2.py
+-rw-r--r--   0        0        0      327 2024-04-08 22:46:02.041313 sliceitoff-0.3b2/src/sliceitoff/screens/level.py
+-rw-r--r--   0        0        0     1127 2024-04-08 22:46:05.050330 sliceitoff-0.3b2/src/sliceitoff/screens/levelup.py
+-rw-r--r--   0        0        0      822 2024-04-08 22:46:09.794358 sliceitoff-0.3b2/src/sliceitoff/screens/mainmenu.py
+-rw-r--r--   0        0        0       98 2024-04-08 14:33:13.405835 sliceitoff-0.3b2/src/sliceitoff/stats/__init__.py
+-rw-r--r--   0        0        0     1435 2024-04-08 14:33:13.405835 sliceitoff-0.3b2/src/sliceitoff/stats/stats.py
+-rw-r--r--   0        0        0       95 2024-04-08 14:33:13.405835 sliceitoff-0.3b2/src/sliceitoff/status/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-08 22:46:22.169430 sliceitoff-0.3b2/src/sliceitoff/status/status.py
+-rw-r--r--   0        0        0      178 2024-04-08 14:33:13.405835 sliceitoff-0.3b2/src/sliceitoff/text/__init__.py
+-rw-r--r--   0        0        0      940 2024-04-08 22:46:31.962488 sliceitoff-0.3b2/src/sliceitoff/text/explode.py
+-rw-r--r--   0        0        0     1520 2024-04-08 14:33:13.405835 sliceitoff-0.3b2/src/sliceitoff/text/fonts.py
+-rw-r--r--   0        0        0     2682 2024-04-08 22:46:45.850569 sliceitoff-0.3b2/src/sliceitoff/text/text.py
+-rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 sliceitoff-0.3b2/PKG-INFO
```

### Comparing `sliceitoff-0.3b1/LICENSE.txt` & `sliceitoff-0.3b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/README.txt` & `sliceitoff-0.3b2/README.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,39 @@
--- Slice It Off! --
+-- Slice It Off! v0.3b --
+
 
 Description:
 
 	Small game where goal is to beat hiscores. Score is gained by
 	slicing parts of playing area off. Faster you do it more score you
 	get. If you hit enemies while slicing you lose healt. There will be
 	also bonuses to boost the scores.
 
+
 Installing:
 	
-	One can use provided `./dev.sh` shell script to buid and install any
-	versionof game:
+	Get version on PyPI:
+	- pip install sliceitoff
+
+	One can also use provided `./dev.sh` shell script to buid and install
+	any version of game:
 	- `git clone https://git.hix.fi/scliceitoff.git`
 	- `cd sliceitoff`
 	- `./dev.sh install`
 
 	Distribution package can be installed normally:
-	- `pipx install sliceitoff.*.tar.gz`
+	- `pip(x) install sliceitoff.*.tar.gz`
+
 
 License:
 
 	This project uses GPL-2 license. Used components uses their
-	licenses. There is gnufonts package from Freedos included in the
-	source tree and it's license can be fount on it's directory.
+	licenses. There is gnufonts package from FreeDOS included in the
+	source tree and it's license can be found on it's directory.
+
 
 Developement:
 	
 	Project makes heavy use of poetry build and dependencies control
 	system. Many shortcuts can be run easily from `./dev.sh` script:
 	- `./dev.sh`
 	- `./dev.sh dev`
```

### Comparing `sliceitoff-0.3b1/pyproject.toml` & `sliceitoff-0.3b2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [tool.poetry]
 name = "sliceitoff"
-version = "0.3-beta.1"
+version = "0.3-beta.2"
 description = "Arcade game where one slices play area off avoiding enemies."
+repository = "https://git.hix.fi/sliceitoff.git/"
 authors = ["Viljami Ilola <+@hix.fi>"]
 readme = "README.txt"
-packages = [{include = "sliceitoff", from = "src"}]
+packages = [
+	{include = "sliceitoff", from = "src"},
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pygame = "^2.5.2"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.1.0"
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/APPINFO/GNUFONTS.LSM`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X10.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X11SNSF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X14.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/8X8.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ANTIQUE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ARCHON.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BACKWARD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BIGSERIF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLCKSNSF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BLOCK.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BOLD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BREEZE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/BROADWAY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COMPUTER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/COURIER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/CYRILLIC.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/DECO.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EMPTY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/EUROTYPE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FAT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FINNISH.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FLAT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRANCE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FRESNO.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/FUTURA-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/GREEK.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEARST.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HEBREW.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/HYLAS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/INVERTED.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ITALICS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/KIDS-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/LCD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MEDIEVAL.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/MODERN-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/NORWAY.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REV8X8.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/REVERSE.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/ROMAN-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSERIF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SANSURF.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCOTT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SCRIPT.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SILVER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STANDARD.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/STRETCH.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SUPER.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SURREAL.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-1.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-2.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/SWISS-3.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TEKTON.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/TERMINUS.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THAI.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT` & `sliceitoff-0.3b2/src/sliceitoff/assets/gnufonts/UTIL/GNUFONTS/THIN.FNT`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/display/display.py` & `sliceitoff-0.3b2/src/sliceitoff/display/display.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/display/scaling.py` & `sliceitoff-0.3b2/src/sliceitoff/display/scaling.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/display/static.py` & `sliceitoff-0.3b2/src/sliceitoff/display/static.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/enemies/ball.py` & `sliceitoff-0.3b2/src/sliceitoff/enemies/ball.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ enemies.ball - Enemy type that goes straight line hitting walls """
 from random import randrange, choice
 
-from text import get_letter_surface
+from sliceitoff.text import get_letter_surface
 from .enemy import Enemy
 
 BALL_SPAWN_AREA = (0, 0, 300_000, 200_000)
 BALL_MOVEMENT = (100, 100)
 BALL_SYMBOLS = (0x1,0x2)
 BALL_SIZE = 8_000
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/enemies/bouncher.py` & `sliceitoff-0.3b2/src/sliceitoff/enemies/bouncher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ enemies.bouncher - Enemy type that bouches around """
 from random import randrange, choice
 
-from text import get_letter_surface
+from sliceitoff.text import get_letter_surface
 from .enemy import Enemy
 
 BOUNCHER_SPAWN_AREA = (0, 0, 300_000, 80_000)
 BOUNCHER_MOVEMENT = (200, 20)
 BOUNCHER_SIZE = 12_000
 BOUNCHER_SYMBOLS = (0x1,0x2)
 GRAVITY = 4
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/enemies/enemies.py` & `sliceitoff-0.3b2/src/sliceitoff/enemies/enemies.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/enemies/enemy.py` & `sliceitoff-0.3b2/src/sliceitoff/enemies/enemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ enemy.enemy - Enemy super class. Wall hitting and other commons """
 import pygame
 
-from display import Scaling
+from sliceitoff.display import Scaling
 
 class Enemy(pygame.sprite.Sprite):
     """ Enemy super class. Just common movements. """
     def __init__(self):
         super().__init__()
         self.position = (0, 0)
         self.movement = (0, 0)
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/field/field.py` & `sliceitoff-0.3b2/src/sliceitoff/field/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ field.field - The playing area or slices, lazer of explosions of it """
 import os
 from random import randrange, choice
 
 import pygame
 
-from display import Scaling, CGA_COLORS
-from text import LetterSprite
+from sliceitoff.display import Scaling, CGA_COLORS
+from sliceitoff.text import LetterSprite
 
 DEBUG = os.getenv("DEBUG")
 
 class FieldSprite(pygame.sprite.Sprite):
     """ Playing area consist of these sprites """
     def __init__(self, area: tuple):
         super().__init__()
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/game/explodeout.py` & `sliceitoff-0.3b2/src/sliceitoff/game/explodeout.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/game/game.py` & `sliceitoff-0.3b2/src/sliceitoff/game/game.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,23 @@
     the minimum
 """
 
 from pathlib import Path
 
 import pygame
 
-from display import Display
-from text import Fonts
-from stats import Stats
-from screens import (
+from sliceitoff.display import Display
+from sliceitoff.text import Fonts
+from sliceitoff.stats import Stats
+from sliceitoff.screens import (
     hiscores_screen,
     instructions1_screen,
     instructions2_screen)
-from hiscores import HiScores
-from mainmenu import Mainmenu, MenuItems
+from sliceitoff.hiscores import HiScores
+from sliceitoff.mainmenu import Mainmenu, MenuItems
 
 from .level import Level
 from .show import Show
 from .initials import Initials
 
 class Game:
     """ This is the whole game. """
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/game/gameplay.py` & `sliceitoff-0.3b2/src/sliceitoff/game/gameplay.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/game/initials.py` & `sliceitoff-0.3b2/src/sliceitoff/game/initials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ game.initials - Use will be asked for initials """
 import pygame
 
-from screens import initials_screen
+from sliceitoff.screens import initials_screen
 
 from .explodeout import ExplodeOutGroup
 
 class Initials(ExplodeOutGroup):
     """ Sprite group that asks initials to self.name from user """
     def __init__(self):
         super().__init__()
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/game/level.py` & `sliceitoff-0.3b2/src/sliceitoff/game/level.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ game.level - This is what runs invidual levels """
 import pygame
 
-from status import Status
-from player import Player, Life
-from field import Field
-from enemies import Enemies
-from screens import levelup_screen, gameover_screen, level_screen
+from sliceitoff.status import Status
+from sliceitoff.player import Player, Life
+from sliceitoff.field import Field
+from sliceitoff.enemies import Enemies
+from sliceitoff.screens import levelup_screen, gameover_screen, level_screen
 from .gameplay import Gameplay
 from .show import Show
 
 class Level(pygame.sprite.Group):
     """ One level that can be played """
     # pylint: disable = too-many-instance-attributes
     def __init__(self, stats = None):
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/game/show.py` & `sliceitoff-0.3b2/src/sliceitoff/game/show.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/hiscores/hiscores.py` & `sliceitoff-0.3b2/src/sliceitoff/hiscores/hiscores.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class HiScores:
     """ Keeps track of high scores """
     def __init__(self):
         """ On creation load high scores from config file """
         self.table=[]
         if os.name == 'nt':
             self.config_filename = os.path.join(Path.home(), "sliceitoff.cfg")
-        else: 
+        else:
             self.config_filename = os.path.join(
                     Path.home(),
                     ".config",
                     "sliceitoffrc")
         if not os.path.isfile(self.config_filename):
             self.table=INITIAL_HIGHSCORES[:]
             return
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/mainmenu/mainmenu.py` & `sliceitoff-0.3b2/src/sliceitoff/mainmenu/mainmenu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ mainmenu.mainmenu - Let's user choose """
 from enum import IntEnum
 import pygame
 
-from screens import mainmenu_screen
-from display import Scaling
+from sliceitoff.screens import mainmenu_screen
+from sliceitoff.display import Scaling
 
-from game.explodeout import ExplodeOutGroup
+from sliceitoff.game.explodeout import ExplodeOutGroup
 
 MOUSE_TRESHOLD = 100
 
 class MenuItems(IntEnum):
     """ Items in the menu. Should match mainmenu_screen """
     NEWGAME = 0
     HISCORES = 1
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/player/life.py` & `sliceitoff-0.3b2/src/sliceitoff/player/life.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ player.life - Hearth that will explode """
 import pygame
 
-from display import Scaling
-
-from text import get_letter_surface, ExplodingSprite
+from sliceitoff.display import Scaling
+from sliceitoff.text import get_letter_surface, ExplodingSprite
 
 class PieceOfHearth(ExplodingSprite):
     """ Eploding piece. Hearth consist of these """
     def __init__(self, image, pos):
         super().__init__()
         self.image = image
         self.rect = self.image.get_rect().move(pos)
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/player/player.py` & `sliceitoff-0.3b2/src/sliceitoff/player/player.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ player.player - Player sprite group and actions """
 import os
 import pygame
 
-from display import Scaling
+from sliceitoff.display import Scaling
 
 from .static import SLICER
 
 DEBUG = os.getenv("DEBUG")
 
 def dataclass_to_surface(dc):
     """ Converts dataclass to surface """
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/player/static.py` & `sliceitoff-0.3b2/src/sliceitoff/player/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ player.static - static data related to player - now just slicer """
 from dataclasses import dataclass
-from display import CGA_COLORS
+
+from sliceitoff.display import CGA_COLORS
 
 @dataclass
 class SLICER:
     """ Slicer tool """
     DIMENSIONS = (32, 8)
     COLORS = [
         CGA_COLORS[0],
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/screens/instructions1.py` & `sliceitoff-0.3b2/src/sliceitoff/screens/instructions1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ screens.instructions1 - First page of instructions"""
-from text import TextPage
+from sliceitoff.text import TextPage
 
 def instructions1_screen():
     """ Instructions about the goal """
     return TextPage(
             "\n       Slice It Off!\n\n"
             "\n"
             " What to do?\n"
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/screens/levelup.py` & `sliceitoff-0.3b2/src/sliceitoff/screens/levelup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ screen.levelup - Screen to show after succesfully completing level """
-from text import TextPage
+from sliceitoff.text import TextPage
 
 def levelup_screen(stats = None):
     """ levelup_screen - screen full of stats how bonus is calculated """
     (
             total_bonus,
             level_bonus,
             life_bonus,
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/screens/mainmenu.py` & `sliceitoff-0.3b2/src/sliceitoff/screens/mainmenu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ screens.mainmenu - Screen for mainmenu"""
 from random import randrange
-from text import TextPage
+from sliceitoff.text import TextPage
 
 def mainmenu_screen(selection):
     """ Screen where current selection is flashing """
     active = randrange(0xe9,0xf0)
     inactive = 0xe7
     text =  (
             f" Slice it off!!\n"
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/stats/stats.py` & `sliceitoff-0.3b2/src/sliceitoff/stats/stats.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/status/status.py` & `sliceitoff-0.3b2/src/sliceitoff/status/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ status.status - The statusline bottom of screen showinf all stats """
 import pygame
 
-from text import TextPage
+from sliceitoff.text import TextPage
 
 class Status(pygame.sprite.Group):
     """ Statusline bottom of screen """
     def __init__(self, stats = None):
         super().__init__()
         self.stats = stats
         self.old_srt = None
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/text/explode.py` & `sliceitoff-0.3b2/src/sliceitoff/text/explode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ text.explode - Exploding effect movements and updates for the sprite """
 from random import randrange
 
 import pygame
 
-from display import Scaling
+from sliceitoff.display import Scaling
 
 class ExplodingSprite(pygame.sprite.Sprite):
     """ Just adds exloding movement to the sprite """
     def __init__(self):
         super().__init__()
         self.rect = None
         self.direction = (
```

### Comparing `sliceitoff-0.3b1/src/sliceitoff/text/fonts.py` & `sliceitoff-0.3b2/src/sliceitoff/text/fonts.py`

 * *Files identical despite different names*

### Comparing `sliceitoff-0.3b1/src/sliceitoff/text/text.py` & `sliceitoff-0.3b2/src/sliceitoff/text/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ text.text - letters, texts and scaling and coloring of fonts """
 import pygame
 
-from display import Scaling, CGA_COLORS
+from sliceitoff.display import Scaling, CGA_COLORS
 from .fonts import Fonts
 from .explode import ExplodingSprite
 
 scaled_fonts = {}
 
 def get_letter_surface(font_key, ch):
     """ Get letter surface at given properties hopefully from cache
```

### Comparing `sliceitoff-0.3b1/PKG-INFO` & `sliceitoff-0.3b2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 Metadata-Version: 2.1
 Name: sliceitoff
-Version: 0.3b1
+Version: 0.3b2
 Summary: Arcade game where one slices play area off avoiding enemies.
+Home-page: https://git.hix.fi/sliceitoff.git/
 Author: Viljami Ilola
 Author-email: +@hix.fi
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pygame (>=2.5.2,<3.0.0)
+Project-URL: Repository, https://git.hix.fi/sliceitoff.git/
 Description-Content-Type: text/plain
 
--- Slice It Off! --
+-- Slice It Off! v0.3b --
+
 
 Description:
 
 	Small game where goal is to beat hiscores. Score is gained by
 	slicing parts of playing area off. Faster you do it more score you
 	get. If you hit enemies while slicing you lose healt. There will be
 	also bonuses to boost the scores.
 
+
 Installing:
 	
-	One can use provided `./dev.sh` shell script to buid and install any
-	versionof game:
+	Get version on PyPI:
+	- pip install sliceitoff
+
+	One can also use provided `./dev.sh` shell script to buid and install
+	any version of game:
 	- `git clone https://git.hix.fi/scliceitoff.git`
 	- `cd sliceitoff`
 	- `./dev.sh install`
 
 	Distribution package can be installed normally:
-	- `pipx install sliceitoff.*.tar.gz`
+	- `pip(x) install sliceitoff.*.tar.gz`
+
 
 License:
 
 	This project uses GPL-2 license. Used components uses their
-	licenses. There is gnufonts package from Freedos included in the
-	source tree and it's license can be fount on it's directory.
+	licenses. There is gnufonts package from FreeDOS included in the
+	source tree and it's license can be found on it's directory.
+
 
 Developement:
 	
 	Project makes heavy use of poetry build and dependencies control
 	system. Many shortcuts can be run easily from `./dev.sh` script:
 	- `./dev.sh`
 	- `./dev.sh dev`
```

