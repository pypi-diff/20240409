# Comparing `tmp/ocatari-1.0.4.tar.gz` & `tmp/ocatari-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocatari-1.0.4.tar", last modified: Thu Apr  4 12:45:31 2024, max compression
+gzip compressed data, was "ocatari-1.0.5.tar", last modified: Tue Apr  9 09:14:58 2024, max compression
```

## Comparing `ocatari-1.0.4.tar` & `ocatari-1.0.5.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.534425 ocatari-1.0.4/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.4/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-04 12:45:31.534425 ocatari-1.0.4/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.4/README.md
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.522425 ocatari-1.0.4/ocatari/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.4/ocatari/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    22811 2024-03-19 14:31:16.000000 ocatari-1.0.4/ocatari/core.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/environments.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.526425 ocatari-1.0.4/ocatari/ram/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.4/ocatari/ram/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/ram/_helper_methods.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15652 2024-03-19 14:28:41.000000 ocatari-1.0.4/ocatari/ram/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.4/ocatari/ram/asterix_old.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.4/ocatari/ram/asterix_old2.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14228 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5593 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    29613 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/extract_ram_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/extract_ram_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4745 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/ram/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.4/ocatari/ram/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    15746 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5915 2024-03-23 11:45:59.000000 ocatari-1.0.4/ocatari/ram/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10776 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    14452 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9441 2024-03-18 13:29:46.000000 ocatari-1.0.4/ocatari/ram/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    12471 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.4/ocatari/ram/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.4/ocatari/ram/yarsrevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10737 2024-03-18 11:06:15.000000 ocatari-1.0.4/ocatari/utils.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.534425 ocatari-1.0.4/ocatari/vision/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.4/ocatari/vision/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/adventure.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.4/ocatari/vision/alien.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.4/ocatari/vision/amidar.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/assault.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.4/ocatari/vision/asterix.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.4/ocatari/vision/asteroids.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.4/ocatari/vision/atlantis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/bankheist.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/battlezone.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.4/ocatari/vision/beamrider.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.4/ocatari/vision/berzerk.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.4/ocatari/vision/bowling.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.4/ocatari/vision/boxing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/breakout.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/carnival.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/centipede.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/choppercommand.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.4/ocatari/vision/crazyclimber.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.4/ocatari/vision/demonattack.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.4/ocatari/vision/donkeykong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/enduro.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.4/ocatari/vision/extract_vision_info.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.4/ocatari/vision/extract_vision_info_short.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/fishingderby.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/freeway.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/frostbite.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/game_objects.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/gopher.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.4/ocatari/vision/hero.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.4/ocatari/vision/icehockey.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/jamesbond.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/kangaroo.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/krull.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/montezumarevenge.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/mspacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.4/ocatari/vision/pacman.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.4/ocatari/vision/pitfall.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.4/ocatari/vision/pong.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.4/ocatari/vision/privateeye.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/qbert.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/riverraid.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/roadrunner.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.4/ocatari/vision/seaquest.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/skiing.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/spaceinvaders.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.4/ocatari/vision/tennis.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/timepilot.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/upndown.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.4/ocatari/vision/utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.4/ocatari/vision/venture.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.4/ocatari/vision/videopinball.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.4/ocatari/vision/yarsrevenge.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.522425 ocatari-1.0.4/ocatari.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-04-04 12:45:31.000000 ocatari-1.0.4/ocatari.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-04-04 12:45:31.534425 ocatari-1.0.4/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1025 2024-04-04 12:45:17.000000 ocatari-1.0.4/setup.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-04 12:45:31.534425 ocatari-1.0.4/tests/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.4/tests/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/display_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.4/tests/display_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.4/tests/get_metrics.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.4/tests/metrics_utils.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.4/tests/plot_speed_results.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/pong_test.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/test_explanation.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/test_game.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.4/tests/test_game_both.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.4/tests/test_game_both_interactive.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.4/tests/test_speed.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.329941 ocatari-1.0.5/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1171 2023-06-14 17:01:45.000000 ocatari-1.0.5/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-09 09:14:58.329941 ocatari-1.0.5/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6297 2024-03-13 13:04:01.000000 ocatari-1.0.5/README.md
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.317941 ocatari-1.0.5/ocatari/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       25 2024-02-13 13:58:13.000000 ocatari-1.0.5/ocatari/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    25223 2024-04-09 09:13:01.000000 ocatari-1.0.5/ocatari/core.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2891 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/environments.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.325941 ocatari-1.0.5/ocatari/ram/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:57:07.000000 ocatari-1.0.5/ocatari/ram/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3297 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/ram/_helper_methods.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14387 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/adventure.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7586 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/alien.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4015 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/amidar.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    15652 2024-03-19 14:28:41.000000 ocatari-1.0.5/ocatari/ram/assault.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5552 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/asterix.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9111 2023-08-23 09:50:18.000000 ocatari-1.0.5/ocatari/ram/asterix_old.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14794 2024-02-12 14:35:56.000000 ocatari-1.0.5/ocatari/ram/asterix_old2.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12738 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/asteroids.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14228 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/atlantis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4552 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/bankheist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    19073 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/battlezone.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5410 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/beamrider.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10096 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/berzerk.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5888 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/bowling.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5593 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/boxing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7113 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/breakout.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11564 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/carnival.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11345 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/centipede.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    29613 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/choppercommand.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10183 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/crazyclimber.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6241 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/demonattack.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8247 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/donkeykong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2102 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/enduro.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    17884 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/extract_ram_info.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2068 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/extract_ram_info_short.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4745 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/fishingderby.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3136 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/freeway.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12497 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/frostbite.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6054 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/ram/game_objects.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8640 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/gopher.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)   426388 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/hero.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4005 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/icehockey.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5966 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/jamesbond.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13579 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/kangaroo.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14946 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/krull.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    38831 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/montezumarevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6500 2024-03-20 15:36:32.000000 ocatari-1.0.5/ocatari/ram/mspacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4625 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/pacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    15746 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/pitfall.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5915 2024-04-09 09:11:16.000000 ocatari-1.0.5/ocatari/ram/pong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16424 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/privateeye.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14403 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/qbert.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10776 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/riverraid.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    13893 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/roadrunner.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    14619 2024-04-09 09:11:51.000000 ocatari-1.0.5/ocatari/ram/seaquest.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9441 2024-03-18 13:29:46.000000 ocatari-1.0.5/ocatari/ram/skiing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    12471 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/spaceinvaders.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8869 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/tennis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16258 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/timepilot.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7136 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/upndown.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3036 2023-07-31 09:59:59.000000 ocatari-1.0.5/ocatari/ram/utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     9308 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/venture.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5063 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/videopinball.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5946 2024-03-13 13:04:01.000000 ocatari-1.0.5/ocatari/ram/yarsrevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10737 2024-03-18 11:06:15.000000 ocatari-1.0.5/ocatari/utils.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.329941 ocatari-1.0.5/ocatari/vision/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      394 2024-02-13 13:55:37.000000 ocatari-1.0.5/ocatari/vision/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5880 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/adventure.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2888 2023-09-07 09:07:40.000000 ocatari-1.0.5/ocatari/vision/alien.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2003 2023-11-15 16:35:48.000000 ocatari-1.0.5/ocatari/vision/amidar.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6175 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/assault.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8795 2023-03-14 16:04:08.000000 ocatari-1.0.5/ocatari/vision/asterix.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2588 2023-10-26 14:02:07.000000 ocatari-1.0.5/ocatari/vision/asteroids.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7361 2023-04-12 13:10:52.000000 ocatari-1.0.5/ocatari/vision/atlantis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2106 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/bankheist.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4570 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/battlezone.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6024 2023-04-12 13:10:52.000000 ocatari-1.0.5/ocatari/vision/beamrider.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2817 2023-05-29 14:25:14.000000 ocatari-1.0.5/ocatari/vision/berzerk.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2486 2023-03-14 16:04:08.000000 ocatari-1.0.5/ocatari/vision/bowling.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1812 2023-10-18 14:47:32.000000 ocatari-1.0.5/ocatari/vision/boxing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2992 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/breakout.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5182 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/carnival.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4292 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/centipede.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5801 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/choppercommand.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3765 2023-11-15 16:35:48.000000 ocatari-1.0.5/ocatari/vision/crazyclimber.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3168 2023-11-23 15:00:40.000000 ocatari-1.0.5/ocatari/vision/demonattack.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4350 2024-02-24 17:10:04.000000 ocatari-1.0.5/ocatari/vision/donkeykong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2418 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/enduro.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7526 2024-02-13 14:20:55.000000 ocatari-1.0.5/ocatari/vision/extract_vision_info.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      597 2023-11-14 14:22:11.000000 ocatari-1.0.5/ocatari/vision/extract_vision_info_short.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5495 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/fishingderby.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1579 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/freeway.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5612 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/frostbite.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3683 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/game_objects.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3016 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/gopher.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11578 2023-10-10 09:58:35.000000 ocatari-1.0.5/ocatari/vision/hero.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2639 2023-07-19 13:40:30.000000 ocatari-1.0.5/ocatari/vision/icehockey.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4096 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/jamesbond.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5690 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/kangaroo.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8432 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/krull.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6525 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/montezumarevenge.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2631 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/mspacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2334 2024-02-14 13:21:26.000000 ocatari-1.0.5/ocatari/vision/pacman.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     7216 2023-11-12 17:10:19.000000 ocatari-1.0.5/ocatari/vision/pitfall.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2065 2023-06-16 08:15:13.000000 ocatari-1.0.5/ocatari/vision/pong.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10116 2023-07-19 13:40:30.000000 ocatari-1.0.5/ocatari/vision/privateeye.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3978 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/qbert.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3867 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/riverraid.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8142 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/roadrunner.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4653 2023-08-23 08:04:55.000000 ocatari-1.0.5/ocatari/vision/seaquest.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2143 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/skiing.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2909 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/spaceinvaders.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2499 2023-06-14 17:01:46.000000 ocatari-1.0.5/ocatari/vision/tennis.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6771 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/timepilot.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3629 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/upndown.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    21751 2024-02-09 12:58:51.000000 ocatari-1.0.5/ocatari/vision/utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6659 2023-08-31 10:23:09.000000 ocatari-1.0.5/ocatari/vision/venture.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4132 2023-08-31 10:23:09.000000 ocatari-1.0.5/ocatari/vision/videopinball.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4128 2023-10-10 09:58:35.000000 ocatari-1.0.5/ocatari/vision/yarsrevenge.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.317941 ocatari-1.0.5/ocatari.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     7744 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3413 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      122 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       14 2024-04-09 09:14:58.000000 ocatari-1.0.5/ocatari.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       38 2024-04-09 09:14:58.329941 ocatari-1.0.5/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1025 2024-04-09 09:14:55.000000 ocatari-1.0.5/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2024-04-09 09:14:58.329941 ocatari-1.0.5/tests/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-14 17:01:46.000000 ocatari-1.0.5/tests/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2509 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/display_game.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4339 2023-08-23 08:04:55.000000 ocatari-1.0.5/tests/display_game_both.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10431 2024-02-24 17:17:25.000000 ocatari-1.0.5/tests/get_metrics.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10493 2023-08-23 09:50:18.000000 ocatari-1.0.5/tests/metrics_utils.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1673 2023-06-14 17:01:46.000000 ocatari-1.0.5/tests/plot_speed_results.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1604 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/pong_test.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1851 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/test_explanation.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2921 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/test_game.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     4637 2024-02-24 17:08:28.000000 ocatari-1.0.5/tests/test_game_both.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     5963 2023-10-26 14:02:07.000000 ocatari-1.0.5/tests/test_game_both_interactive.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1281 2024-03-13 13:04:01.000000 ocatari-1.0.5/tests/test_speed.py
```

### Comparing `ocatari-1.0.4/LICENSE` & `ocatari-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/PKG-INFO` & `ocatari-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.4
+Version: 1.0.5
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 License: UNKNOWN
 Description: # Object-Centric Atari Environments
         Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
```

### Comparing `ocatari-1.0.4/README.md` & `ocatari-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/core.py` & `ocatari-1.0.5/ocatari/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,22 @@
                 self._fill_buffer = self._fill_buffer_dqn
                 self._reset_buffer = self._reset_buffer_dqn
             else:
                 print("To use the buffer of OCAtari, you need to install torch.")
         elif obs_mode == "ori":
             self._fill_buffer = self._fill_buffer_ori
             self._reset_buffer = self._reset_buffer_ori
+        elif obs_mode == "obj":
+            print("Using OBJ State Representation")
+            if mode == "ram":
+                self._fill_buffer = self._fill_buffer_obj
+                self._reset_buffer = self._reset_buffer_obj
+            else:
+                print(colored("This obs mode is only available in ram mode", "red"))
+                exit(1)
         elif obs_mode is not None:
             print(colored("Undefined mode for observation (obs_mode), has to be one of ['dqn', 'ori', None]", "red"))
             exit(1)
 
         self.render_mode = render_mode
         self.render_oc_overlay = render_oc_overlay
         self.rendering_initialized = False
@@ -154,18 +162,18 @@
         :param action: The action to perform at this step.
         :type action: int
         """
         raise NotImplementedError()
 
     def _step_ram(self, *args, **kwargs):
         obs, reward, terminated, truncated, info = self._env.step(*args, **kwargs)
-        if self.mode == "ram":
+        if self.mode == "ram" or self.mode == "revised":
             self.detect_objects(self._objects, self._env.env.unwrapped.ale.getRAM(), self.game_name, self.hud)
         else:  # mode == "raw" because in raw mode we augment the info dictionary
-            self.detect_objects(info, self._env.env.unwrapped.ale.getRAM(), self.game_name)
+            self.detect_objects(info, self._env.env.unwrapped.ale.getRAM(), self.game_name, self.hud)
         self._fill_buffer()
         return obs, reward, truncated, terminated, info
 
     def _step_vision(self, *args, **kwargs):
         obs, reward, terminated, truncated, info = self._env.step(*args, **kwargs)
         self.detect_objects(self._objects, obs, self.game_name, self.hud)
         self._fill_buffer()
@@ -188,14 +196,20 @@
 
     def _reset_buffer_ori(self):
         for _ in range(self.buffer_window_size):
             self._state_buffer.append(
                 torch.zeros(210, 160, 3, device=DEVICE, dtype=torch.uint8)
             )
 
+    def _reset_buffer_obj(self):
+        for _ in range(self.buffer_window_size):
+            self._state_buffer.append(
+                torch.zeros(len(self._objects), 4, device=DEVICE, dtype=torch.uint8)
+            )
+
     def reset(self, *args, **kwargs):
         """
         Resets the buffer and environment to an initial internal state, returning an initial observation and info.
         See `env.reset() <https://gymnasium.farama.org/api/env/#gymnasium.Env.reset>`_ for gymnasium details.
         """
         self._reset_buffer()
         self._objects = init_objects(self.game_name, self.hud)
@@ -209,14 +223,22 @@
                                                device=DEVICE))
 
     def _fill_buffer_ori(self):
         state = self._ale.getScreenRGB()
         self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
                                                device=DEVICE))
 
+    def _fill_buffer_obj(self):
+        tensor = []
+        for obj in self._objects:
+            tensor.append(np.asarray(obj.xywh))
+        state = np.asarray(tensor)
+        self._state_buffer.append(torch.tensor(state, dtype=torch.uint8,
+                                               device=DEVICE))
+
     def _get_buffer_as_stack(self):
         return torch.stack(list(self._state_buffer), 0).unsqueeze(0).byte()
 
     window : pygame.Surface = None
     clock : pygame.time.Clock = None
 
     def _initialize_rendering(self, sample_image):
@@ -344,15 +366,15 @@
     @property
     def nb_actions(self):
         """
         The number of actions available in this environments.
 
         :type: int
         """
-        return self._env.unwrapped.action_space.n
+        return self.action_space.n
 
     @property
     def dqn_obs(self):
         """
         The 4 (grey+down)scaled last frames (84x84) of the environment, used notably by dqn agents as states.
 
         :type: torch.tensor
@@ -540,17 +562,59 @@
         self._env.step(1) # activate the game
         [self._env.step(0) for _ in range(8)] 
         startp = pot_start_pos[rndinit]
         for rp, sp in zip([19, 27], startp):
             self.set_ram(rp, sp)
         self.lasty = startp[1]
 
+
+def extra_rew(game_objects, episode_starts, last_crashed):
+    player = [o for o in game_objects if "Player" in str(o)][0]
+    # Get current platform
+    platform = np.ceil((player.xy[1] - player.h - 16) / 48)  # 0: topmost, 3: lowest platform
+
+    # Encourage moving to the child
+    if not episode_starts and not last_crashed:
+        if platform % 2 == 0:  # even platform, encourage left movement
+            reward = - player.dx
+        else:  # encourage right movement
+            reward = player.dx
+
+        # Encourage upward movement
+        reward -= player.dy / 5
+    else:
+        reward = 0
+    return reward
+
+
+class EasyKangaroo(OCAtari):
+    def __init__(self, env_name="ALE/Kangaroo", mode="ram", hud=False, obs_mode="dqn", render_mode=None, render_oc_overlay=False, *args, **kwargs):
+        self.lasty = 154
+        self.nb_lives = 2
+        super().__init__(env_name, mode, hud, obs_mode, render_mode, render_oc_overlay, *args, **kwargs)
+
+    def _step_ram(self, *args, **kwargs):
+        obs, reward, truncated, terminated, info = super()._step_ram(*args, **kwargs)
+        last_crashed = self.nb_lives != info["lives"]
+        self.nb_lives = info["lives"]
+        reward += extra_rew(self.objects, last_crashed, last_crashed)
+        
+        return obs, reward, truncated, terminated, info
+
+
 if __name__ == "__main__":
-    env = EasyDonkey(render_mode="human")
+    env = EasyKangaroo(render_mode="human")
     env.reset()
-    for _ in range(1000):
-        _, rew, truncated, terminated, _ = env.step(env.action_space.sample())
-        # if rew:
-        #     print(rew)
+    for st in range(1000):
+        # _, rew, truncated, terminated, _ = env.step(env.action_space.sample())
+        if st < 120:
+            action = 3
+        elif st < 150:
+            action = 2
+        else:
+            action = 4
+        _, rew, truncated, terminated, _ = env.step(action)
+        if rew:
+            print(rew)
         if truncated or terminated:
             env.reset()
         env.render()
```

### Comparing `ocatari-1.0.4/ocatari/environments.py` & `ocatari-1.0.5/ocatari/environments.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/_helper_methods.py` & `ocatari-1.0.5/ocatari/ram/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/adventure.py` & `ocatari-1.0.5/ocatari/ram/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/alien.py` & `ocatari-1.0.5/ocatari/ram/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/amidar.py` & `ocatari-1.0.5/ocatari/ram/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/assault.py` & `ocatari-1.0.5/ocatari/ram/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/asterix.py` & `ocatari-1.0.5/ocatari/ram/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/asterix_old.py` & `ocatari-1.0.5/ocatari/ram/asterix_old.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/asterix_old2.py` & `ocatari-1.0.5/ocatari/ram/asterix_old2.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/asteroids.py` & `ocatari-1.0.5/ocatari/ram/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/atlantis.py` & `ocatari-1.0.5/ocatari/ram/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/bankheist.py` & `ocatari-1.0.5/ocatari/ram/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/battlezone.py` & `ocatari-1.0.5/ocatari/ram/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/beamrider.py` & `ocatari-1.0.5/ocatari/ram/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/berzerk.py` & `ocatari-1.0.5/ocatari/ram/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/bowling.py` & `ocatari-1.0.5/ocatari/ram/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/boxing.py` & `ocatari-1.0.5/ocatari/ram/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/breakout.py` & `ocatari-1.0.5/ocatari/ram/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/carnival.py` & `ocatari-1.0.5/ocatari/ram/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/centipede.py` & `ocatari-1.0.5/ocatari/ram/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/choppercommand.py` & `ocatari-1.0.5/ocatari/ram/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/crazyclimber.py` & `ocatari-1.0.5/ocatari/ram/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/demonattack.py` & `ocatari-1.0.5/ocatari/ram/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/donkeykong.py` & `ocatari-1.0.5/ocatari/ram/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/enduro.py` & `ocatari-1.0.5/ocatari/ram/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/extract_ram_info.py` & `ocatari-1.0.5/ocatari/ram/extract_ram_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/extract_ram_info_short.py` & `ocatari-1.0.5/ocatari/ram/extract_ram_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/fishingderby.py` & `ocatari-1.0.5/ocatari/ram/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/freeway.py` & `ocatari-1.0.5/ocatari/ram/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/frostbite.py` & `ocatari-1.0.5/ocatari/ram/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/game_objects.py` & `ocatari-1.0.5/ocatari/ram/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/gopher.py` & `ocatari-1.0.5/ocatari/ram/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/hero.py` & `ocatari-1.0.5/ocatari/ram/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/icehockey.py` & `ocatari-1.0.5/ocatari/ram/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/jamesbond.py` & `ocatari-1.0.5/ocatari/ram/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/kangaroo.py` & `ocatari-1.0.5/ocatari/ram/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/krull.py` & `ocatari-1.0.5/ocatari/ram/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/montezumarevenge.py` & `ocatari-1.0.5/ocatari/ram/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/mspacman.py` & `ocatari-1.0.5/ocatari/ram/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/pacman.py` & `ocatari-1.0.5/ocatari/ram/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/pitfall.py` & `ocatari-1.0.5/ocatari/ram/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/pong.py` & `ocatari-1.0.5/ocatari/ram/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/privateeye.py` & `ocatari-1.0.5/ocatari/ram/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/qbert.py` & `ocatari-1.0.5/ocatari/ram/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/riverraid.py` & `ocatari-1.0.5/ocatari/ram/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/roadrunner.py` & `ocatari-1.0.5/ocatari/ram/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/seaquest.py` & `ocatari-1.0.5/ocatari/ram/seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
 def _update_enemies(ram_state):
     """The diving area is divided into 4 lanes (plus the surface lane).
     Enemies come in batches. Each batch has three slots that can be
     arbitrarily filled up by enemies. Consequently, there are 8 possible
     combinations (formations) of enemy/empty slots for each batch. For each lane,
     one single RAM value determines the current formation. Moreover, each
-    batch consits purely of sharks or of submarines, determined by another value."""
+    batch consists purely of sharks or of submarines, determined by another value."""
 
     for i in range(4):  # for each of the 4 lanes (from bottom to top lane)
         present_enemy_type = Submarine if _is_submarine(i, ram_state) else Shark
         hidden_enemy_type = Shark if _is_submarine(i, ram_state) else Submarine
         batch_formation = ram_state[36 + i]
 
         for j in range(3):  # for each of the three slots (left to right)
@@ -385,15 +385,18 @@
             idx = i * 3 + j
             if enemy_in_slot:
                 x = (ram_state[30 + i] + 16 * j) % 256
                 y = 141 - i * 24
                 if present_enemy_type == Shark:
                     # Sharks float up and down, determined by an offset
                     y += ram_state[93] - 4
-                _update_object(present_enemy_type, "xy", (x, y), idx=idx)
+                if -5 <= x <= 165:  # Only track objects that are on the screen
+                    _update_object(present_enemy_type, "xy", (x, y), idx=idx)
+                else:
+                    _remove_object(present_enemy_type, idx)
             else:
                 _remove_object(present_enemy_type, idx)
             _remove_object(hidden_enemy_type, idx)  # always remove the invisible enemy
 
 
 def _update_divers_and_enemy_missiles(ram_state):
     # divers and enemy_missiles share a ram position
```

### Comparing `ocatari-1.0.4/ocatari/ram/skiing.py` & `ocatari-1.0.5/ocatari/ram/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/spaceinvaders.py` & `ocatari-1.0.5/ocatari/ram/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/tennis.py` & `ocatari-1.0.5/ocatari/ram/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/timepilot.py` & `ocatari-1.0.5/ocatari/ram/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/upndown.py` & `ocatari-1.0.5/ocatari/ram/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/utils.py` & `ocatari-1.0.5/ocatari/ram/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/venture.py` & `ocatari-1.0.5/ocatari/ram/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/videopinball.py` & `ocatari-1.0.5/ocatari/ram/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/ram/yarsrevenge.py` & `ocatari-1.0.5/ocatari/ram/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/utils.py` & `ocatari-1.0.5/ocatari/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/adventure.py` & `ocatari-1.0.5/ocatari/vision/adventure.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/alien.py` & `ocatari-1.0.5/ocatari/vision/alien.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/amidar.py` & `ocatari-1.0.5/ocatari/vision/amidar.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/assault.py` & `ocatari-1.0.5/ocatari/vision/assault.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/asterix.py` & `ocatari-1.0.5/ocatari/vision/asterix.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/asteroids.py` & `ocatari-1.0.5/ocatari/vision/asteroids.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/atlantis.py` & `ocatari-1.0.5/ocatari/vision/atlantis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/bankheist.py` & `ocatari-1.0.5/ocatari/vision/bankheist.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/battlezone.py` & `ocatari-1.0.5/ocatari/vision/battlezone.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/beamrider.py` & `ocatari-1.0.5/ocatari/vision/beamrider.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/berzerk.py` & `ocatari-1.0.5/ocatari/vision/berzerk.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/bowling.py` & `ocatari-1.0.5/ocatari/vision/bowling.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/boxing.py` & `ocatari-1.0.5/ocatari/vision/boxing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/breakout.py` & `ocatari-1.0.5/ocatari/vision/breakout.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/carnival.py` & `ocatari-1.0.5/ocatari/vision/carnival.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/centipede.py` & `ocatari-1.0.5/ocatari/vision/centipede.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/choppercommand.py` & `ocatari-1.0.5/ocatari/vision/choppercommand.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/crazyclimber.py` & `ocatari-1.0.5/ocatari/vision/crazyclimber.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/demonattack.py` & `ocatari-1.0.5/ocatari/vision/demonattack.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/donkeykong.py` & `ocatari-1.0.5/ocatari/vision/donkeykong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/enduro.py` & `ocatari-1.0.5/ocatari/vision/enduro.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/extract_vision_info.py` & `ocatari-1.0.5/ocatari/vision/extract_vision_info.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/extract_vision_info_short.py` & `ocatari-1.0.5/ocatari/vision/extract_vision_info_short.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/fishingderby.py` & `ocatari-1.0.5/ocatari/vision/fishingderby.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/freeway.py` & `ocatari-1.0.5/ocatari/vision/freeway.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/frostbite.py` & `ocatari-1.0.5/ocatari/vision/frostbite.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/game_objects.py` & `ocatari-1.0.5/ocatari/vision/game_objects.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/gopher.py` & `ocatari-1.0.5/ocatari/vision/gopher.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/hero.py` & `ocatari-1.0.5/ocatari/vision/hero.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/icehockey.py` & `ocatari-1.0.5/ocatari/vision/icehockey.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/jamesbond.py` & `ocatari-1.0.5/ocatari/vision/jamesbond.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/kangaroo.py` & `ocatari-1.0.5/ocatari/vision/kangaroo.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/krull.py` & `ocatari-1.0.5/ocatari/vision/krull.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/montezumarevenge.py` & `ocatari-1.0.5/ocatari/vision/montezumarevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/mspacman.py` & `ocatari-1.0.5/ocatari/vision/mspacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/pacman.py` & `ocatari-1.0.5/ocatari/vision/pacman.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/pitfall.py` & `ocatari-1.0.5/ocatari/vision/pitfall.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/pong.py` & `ocatari-1.0.5/ocatari/vision/pong.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/privateeye.py` & `ocatari-1.0.5/ocatari/vision/privateeye.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/qbert.py` & `ocatari-1.0.5/ocatari/vision/qbert.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/riverraid.py` & `ocatari-1.0.5/ocatari/vision/riverraid.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/roadrunner.py` & `ocatari-1.0.5/ocatari/vision/roadrunner.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/seaquest.py` & `ocatari-1.0.5/ocatari/vision/seaquest.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/skiing.py` & `ocatari-1.0.5/ocatari/vision/skiing.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/spaceinvaders.py` & `ocatari-1.0.5/ocatari/vision/spaceinvaders.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/tennis.py` & `ocatari-1.0.5/ocatari/vision/tennis.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/timepilot.py` & `ocatari-1.0.5/ocatari/vision/timepilot.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/upndown.py` & `ocatari-1.0.5/ocatari/vision/upndown.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/utils.py` & `ocatari-1.0.5/ocatari/vision/utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/venture.py` & `ocatari-1.0.5/ocatari/vision/venture.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/videopinball.py` & `ocatari-1.0.5/ocatari/vision/videopinball.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari/vision/yarsrevenge.py` & `ocatari-1.0.5/ocatari/vision/yarsrevenge.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/ocatari.egg-info/PKG-INFO` & `ocatari-1.0.5/ocatari.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocatari
-Version: 1.0.4
+Version: 1.0.5
 Summary: Object Centric Atari 2600
 Home-page: https://github.com/k4ntz/OC_Atari
 Author: Quentin Delfosse
 Author-email: quentin.delfosse@cs.tu-darmstadt.de
 License: UNKNOWN
 Description: # Object-Centric Atari Environments
         Quentin Delfosse, Jannis Blüml, Bjarne Gregori, Sebastian Sztwiertnia, Anurag Maurya, Kévin-Lâm Quesnel and Simon Wulf
```

### Comparing `ocatari-1.0.4/ocatari.egg-info/SOURCES.txt` & `ocatari-1.0.5/ocatari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/setup.py` & `ocatari-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
```

### Comparing `ocatari-1.0.4/tests/display_game.py` & `ocatari-1.0.5/tests/display_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/display_game_both.py` & `ocatari-1.0.5/tests/display_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/get_metrics.py` & `ocatari-1.0.5/tests/get_metrics.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/metrics_utils.py` & `ocatari-1.0.5/tests/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/plot_speed_results.py` & `ocatari-1.0.5/tests/plot_speed_results.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/pong_test.py` & `ocatari-1.0.5/tests/pong_test.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/test_explanation.py` & `ocatari-1.0.5/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/test_game.py` & `ocatari-1.0.5/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/test_game_both.py` & `ocatari-1.0.5/tests/test_game_both.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/test_game_both_interactive.py` & `ocatari-1.0.5/tests/test_game_both_interactive.py`

 * *Files identical despite different names*

### Comparing `ocatari-1.0.4/tests/test_speed.py` & `ocatari-1.0.5/tests/test_speed.py`

 * *Files identical despite different names*

