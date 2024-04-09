# Comparing `tmp/sto_oscr-2024.3b40.tar.gz` & `tmp/sto_oscr-2024.4b20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sto_oscr-2024.3b40.tar` & `sto_oscr-2024.4b20.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       44 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/.flake8
--rw-r--r--   0        0        0       98 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1237 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/__init__.py
--rw-r--r--   0        0        0     2228 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/cli.py
--rw-r--r--   0        0        0    13485 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/combat.py
--rw-r--r--   0        0        0    16346 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/datamodels.py
--rw-r--r--   0        0        0     9478 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/detection.py
--rw-r--r--   0        0        0    10903 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/iofunc.py
--rw-r--r--   0        0        0     9614 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/main.py
--rw-r--r--   0        0        0    22922 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/parser.py
--rw-r--r--   0        0        0     3222 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/OSCR/utilities.py
--rw-r--r--   0        0        0    35149 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/LICENSE
--rw-r--r--   0        0        0      181 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/README.md
--rw-r--r--   0        0        0      899 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/pyproject.toml
--rw-r--r--   0        0        0    41255 1980-01-01 00:00:00.000000 sto_oscr-2024.3b40/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/.flake8
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/cli.py
+-rw-r--r--   0        0        0    14233 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/combat.py
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/datamodels.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/detection.py
+-rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/iofunc.py
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/liveparser.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/main.py
+-rw-r--r--   0        0        0    23569 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/parser.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/utilities.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/LICENSE
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/pyproject.toml
+-rw-r--r--   0        0        0    41255 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/PKG-INFO
```

### Comparing `sto_oscr-2024.3b40/OSCR/__init__.py` & `sto_oscr-2024.4b20/OSCR/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-__all__ = ['cli', 'datamodels', 'iofunc', 'main', 'parser', 'utilities']
+__all__ = [
+        'cli', 'combat', 'datamodels', 'detection', 'iofunc', 'liveparser', 'main', 'parser',
+        'utilities']
 
-TABLE_HEADER = ('Combat Time', 'DPS', 'Total Damage', 'Debuff', 'Attacks-in Share', 'Taken Damage Share', 
-        'Damage Share', 'Max One Hit', 'Crit Chance', 'Deaths', 'Total Heals', 'Heal Share', 
-        'Heal Crit Chance', 'Total Damage Taken', 'Total Hull Damage Taken', 'Total Shield Damage Taken',
-        'Total Attacks', 'Hull Attacks', 'Attacks-in Number', 'Heal Crit Number', 'Heal Number', 
-        'Crit Number', 'Misses')
+TABLE_HEADER = (
+    'Combat Time', 'DPS', 'Total Damage', 'Debuff', 'Attacks-in Share',
+    'Taken Damage Share', 'Damage Share', 'Max One Hit', 'Crit Chance', 'Deaths', 'Total Heals',
+    'Heal Share', 'Heal Crit Chance', 'Total Damage Taken', 'Total Hull Damage Taken',
+    'Total Shield Damage Taken', 'Total Attacks', 'Hull Attacks', 'Attacks-in Number',
+    'Heal Crit Number', 'Heal Number', 'Crit Number', 'Misses')
 
-TREE_HEADER = ('', 'DPS', 'Total Damage', 'Debuff', 'Max One Hit', 'Crit Chance', 'Accuracy', 'Flank Rate', 
-        'Kills', 'Attacks', 'Misses', 'Critical Hits', 'Flank Hits', 'Shield Damage', 'Shield DPS',
-        'Hull Damage', 'Hull DPS', 'Base Damage', 'Base DPS', 'Combat Time', 'Hull Attacks', 
-        'Shield Attacks') #, 'Hull Resistance', 'Shield Resistance')
+TREE_HEADER = (
+    '', 'DPS', 'Total Damage', 'Debuff', 'Max One Hit', 'Crit Chance', 'Accuracy', 'Flank Rate',
+    'Kills', 'Attacks', 'Misses', 'Critical Hits', 'Flank Hits', 'Shield Damage', 'Shield DPS',
+    'Hull Damage', 'Hull DPS', 'Base Damage', 'Base DPS', 'Combat Time', 'Hull Attacks',
+    'Shield Attacks')  # , 'Shield Resistance')
 
-HEAL_TREE_HEADER = ('', 'HPS', 'Total Heal', 'Hull Heal', 'Hull HPS', 'Shield Heal', 'Shield HPS', 
-        'Max One Heal', 'Crit Chance', 'Heal Ticks', 'Critical Heals', 'Combat Time', 'Hull Heal Ticks',
-        'Shield Heal Ticks')
+HEAL_TREE_HEADER = (
+    '', 'HPS', 'Total Heal', 'Hull Heal', 'Hull HPS', 'Shield Heal', 'Shield HPS',
+    'Max One Heal', 'Crit Chance', 'Heal Ticks', 'Critical Heals', 'Combat Time', 'Hull Heal Ticks',
+    'Shield Heal Ticks')
+
+LIVE_TABLE_HEADER = (
+    'DPS', 'Combat Time', 'Debuff', 'Attacks-in', 'HPS', 'Kills', 'Deaths')
 
 from .main import OSCR
 from .datamodels import TreeItem
 from .iofunc import split_log_by_lines, split_log_by_combat
+from .liveparser import LiveParser
```

### Comparing `sto_oscr-2024.3b40/OSCR/cli.py` & `sto_oscr-2024.4b20/OSCR/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,49 +10,56 @@
 import OSCR
 
 
 def list_combats(parser):
     """List the parsed combats but do not do any analysis"""
     for combat in parser.combats:
         print(
-            f"start={combat.start_time} end={combat.end_time} duration={combat.duration} map={combat.map} difficulty={combat.difficulty}"
+            f"start={combat.start_time} end={combat.end_time} duration={combat.duration} "
+            "map={combat.map} difficulty={combat.difficulty}"
         )
 
 
 def shallow(args, parser):
     """Print the combat summary for each combat"""
     for idx, _ in enumerate(parser.analyzed_combats):
         parser.shallow_combat_analysis(idx)
         combat = parser.active_combat
         print(
             f"start={combat.start_time} end={combat.end_time} duration={combat.duration} map={combat.map} difficulty={combat.difficulty}"
         )
 
         print("  Players (Damage)")
         for k, v in parser.active_combat.player_dict.items():
-            print(f"    {v.name}{v.handle}: {v.total_damage:,.0f} ({v.DPS:,.0f} DPS)")
+            print(f"    {v.name}{v.handle}: damage={v.total_damage:,.0f} dps={v.DPS:,.0f} build={v.build}")
 
         if args.metadata:
             print("  Computers:")
-            for k, v in parser.active_combat.computer_meta.items():
+            for k, v in parser.active_combat.critter_meta.items():
                 if v["deaths"] == 0:
                     continue
                 perc = numpy.percentile(v["total_hull_damage_taken"], 50)
-                print(
-                    f"    {k}: count={v['count']} deaths={v['deaths']} hull={perc:.0f}"
-                )
+                print(f"    {k}: count={v['count']} deaths={v['deaths']} hull={perc:.0f}")
+
+        if args.events:
+            print(" Events (Players)")
+            for k, v in parser.active_combat.player_dict.items():
+                print(f"    {v.name}{v.handle}:")
+                for event in v.events:
+                    print(f"      {event}")
 
 
 def main():
     """Main"""
     parser = argparse.ArgumentParser()
     parser.add_argument("-i", "--input")
     parser.add_argument("-l", "--list", action=argparse.BooleanOptionalAction)
     parser.add_argument("-s", "--shallow", action=argparse.BooleanOptionalAction)
     parser.add_argument("-m", "--metadata", action=argparse.BooleanOptionalAction)
+    parser.add_argument("-e", "--events", action=argparse.BooleanOptionalAction)
     args = parser.parse_args()
 
     parser = OSCR.OSCR(args.input)
     parser.analyze_log_file()
 
     if args.list:
         list_combats(parser)
```

### Comparing `sto_oscr-2024.3b40/OSCR/combat.py` & `sto_oscr-2024.4b20/OSCR/combat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """ This file implements the Combat class """
 
 from collections import deque
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timedelta
 
 import numpy
 
 from .datamodels import OverviewTableRow
 from .detection import Detection
 from .utilities import get_entity_name, get_flags, get_handle_from_id
 
 
 def check_difficulty_deaths(data, metadata):
     """
     Check deaths against combat metadata
     data: difficulty-based dicitionary in MAP_DIFFICULTY_ENTITY_DEATH_COUNTS
-    metadata: Combat metadata from analyze_computers
+    metadata: Combat metadata from analyze_critters
     returns True on match, otherwise False
     """
 
     for k, v in data.items():
         meta = metadata.get(k)
         if meta is None:
             # Map is missing some NPC data - it's invalid.
@@ -29,15 +29,15 @@
     return True
 
 
 def check_difficulty_damage(data, metadata):
     """
     Check hull damage taken against combat metadata
     data: difficulty-based dicitionary in MAP_DIFFICULTY_ENTITY_HULL_COUNTS
-    metadata: Combat metadata from analyze_computers
+    metadata: Combat metadata from analyze_critters
     returns True on match, otherwise False
     """
 
     # I had issues detecting HSA. This really should be lower.
     # Maybe make it per-map?
     var = 0.20
 
@@ -53,26 +53,27 @@
             # Map damage don't line up - it's invalid (possible over/underkill)
             return False
     return True
 
 
 class Combat:
     """
-    Contains a single combat including raw log lines, map and combat information and shallow parse results.
+    Contains a single combat including raw log lines, map and combat information and shallow parse
+    results.
     """
 
     def __init__(self):
         self.log_data = deque()
         self.map = None
         self.difficulty = None
         self.start_time = None
         self.end_time = None
         self.players = {}
-        self.computers = {}
-        self.computer_meta = {}
+        self.critters = {}
+        self.critter_meta = {}
 
     def analyze_last_line(self):
         """Analyze the last line and try and detect the map and difficulty"""
 
         if self.map is not None and self.map != "Combat" and self.difficulty is not None:
             return
 
@@ -92,69 +93,62 @@
         damage over time graphs so that the log does not need to be iterated
         over again.
         """
 
         self.graph_resolution = graph_resolution
         self.analyze_log_data()
         self.analyze_players()
-        self.analyze_computers()
+        self.analyze_critters()
 
     def analyze_log_data(self):
         """ """
 
         graph_timedelta = timedelta(seconds=self.graph_resolution)
-        graph_points = 1
+        graph_points = 0
         last_graph_time = self.log_data[0].timestamp
 
         self.players = {}
-        self.computers = {}
-        self.computer_meta = {}
+        self.critters = {}
+        self.critter_meta = {}
 
         for line in self.log_data:
             # manage entites
             player_attacks = line.owner_id.startswith("P")
             player_attacked = line.target_id.startswith("P")
             if not player_attacks and not player_attacked:
                 continue
             attacker = None
             target = None
             crit_flag, miss_flag, kill_flag = get_flags(line.flags)
             if player_attacks:
                 if line.owner_id not in self.players:
-                    self.players[line.owner_id] = OverviewTableRow(
-                        line.owner_name, get_handle_from_id(line.owner_id)
-                    )
-                    self.players[line.owner_id].combat_start = line.timestamp.timestamp()
-                attacker = self.players[line.owner_id]
-                attacker.combat_end = line.timestamp.timestamp()
+                    attacker = OverviewTableRow(line.owner_name, get_handle_from_id(line.owner_id))
+                    self.players[line.owner_id] = attacker
+                    attacker.events = []
+                else:
+                    attacker = self.players[line.owner_id]
             else:
-                if line.owner_id not in self.computers:
-                    self.computers[line.owner_id] = OverviewTableRow(
+                if line.owner_id not in self.critters:
+                    self.critters[line.owner_id] = OverviewTableRow(
                         line.owner_name, get_handle_from_id(line.owner_id)
                     )
-                    self.computers[line.owner_id].combat_start = line.timestamp.timestamp()
-                attacker = self.computers[line.owner_id]
-                attacker.combat_end = line.timestamp.timestamp()
+                attacker = self.critters[line.owner_id]
 
             if player_attacked:
                 if line.target_id not in self.players:
                     self.players[line.target_id] = OverviewTableRow(
                         line.target_name, get_handle_from_id(line.target_id)
                     )
-                    self.players[line.target_id].combat_start = line.timestamp.timestamp()
                 target = self.players[line.target_id]
-                target.combat_end = line.timestamp.timestamp()
             else:
-                if line.target_id not in self.computers:
-                    self.computers[line.target_id] = OverviewTableRow(
+                if line.target_id not in self.critters:
+                    self.critters[line.target_id] = OverviewTableRow(
                         line.target_name, get_handle_from_id(line.target_id)
                     )
-                    self.computers[line.target_id].combat_start = line.timestamp.timestamp()
-                target = self.computers[line.target_id]
-                target.combat_end = line.timestamp.timestamp()
+                target = self.critters[line.target_id]
 
             # get table data
             if miss_flag:
                 attacker.misses += 1
             if kill_flag:
                 target.deaths += 1
 
@@ -162,14 +156,23 @@
                 line.type == "Shield" and line.magnitude < 0 and line.magnitude2 >= 0
             ) or line.type == "HitPoints":
                 attacker.total_heals += abs(line.magnitude)
                 attacker.heal_num += 1
                 if crit_flag:
                     attacker.heal_crit_num += 1
             else:
+                # Combat Duration
+                # Heals, damage taken and self-damage don't affect combat time
+                if line.target_id != '*':
+                    current_time = line.timestamp.timestamp()
+                    try:
+                        attacker.combat_interval[1] = current_time
+                    except TypeError:
+                        attacker.combat_interval = [current_time, current_time]
+
                 magnitude = abs(line.magnitude)
                 target.total_damage_taken += magnitude
                 if line.type == "Shield":
                     target.total_shield_damage_taken += magnitude
                 else:
                     target.total_hull_damage_taken += magnitude
                 target.attacks_in_num += 1
@@ -183,39 +186,51 @@
                 if not line.type == "Shield" and not miss_flag:
                     if line.magnitude != 0 and line.magnitude2 != 0:
                         attacker.resistance_sum += line.magnitude / line.magnitude2
                         attacker.hull_attacks += 1
 
             # update graph
             if line.timestamp - last_graph_time >= graph_timedelta:
+                current_graph_timedelta = (line.timestamp - last_graph_time).total_seconds()
+                graph_points += current_graph_timedelta // graph_timedelta.total_seconds()
                 for player in self.players.values():
-                    player.DMG_graph_data.append(player.damage_buffer)
-                    player.damage_buffer = 0.0
-                    player.graph_time.append(graph_points * self.graph_resolution)
-                graph_points += 1
+                    if player.damage_buffer != 0:
+                        player.DMG_graph_data.append(player.damage_buffer)
+                        player.damage_buffer = 0.0
+                        player.graph_time.append(graph_points * self.graph_resolution)
                 last_graph_time = line.timestamp
 
+            if line.event_name not in attacker.events:
+                attacker.events.append(line.event_name)
+
     def analyze_players(self):
         """
         Analyze players to determine time-based metrics such as DPS.
         """
 
         total_damage = 0
         total_damage_taken = 0
         total_attacks = 0
         total_heals = 0
 
+        # Filter out players with no combat time.
+        players = {}
+        for key, player in self.players.items():
+            if player.combat_interval is not None and player.events is not None:
+                players[key] = player
+        self.players = players
+
         for player in self.players.values():
             total_damage += player.total_damage
             total_damage_taken += player.total_damage_taken
             total_attacks += player.attacks_in_num
             total_heals += player.total_heals
 
         for player in self.players.values():
-            player.combat_time = player.combat_end - player.combat_start
+            player.combat_time = player.combat_interval[1] - player.combat_interval[0]
             successful_attacks = player.hull_attacks - player.misses
 
             try:
                 player.debuff = player.resistance_sum / successful_attacks * 100
             except ZeroDivisionError:
                 player.debuff = 0.0
             try:
@@ -244,19 +259,25 @@
             except ZeroDivisionError:
                 player.attacks_in_share = 0.0
             try:
                 player.heal_share = player.total_heals / total_heals * 100
             except ZeroDivisionError:
                 player.heal_share = 0.0
 
+            for k, v in Detection.BUILD_DETECTION_ABILITIES.items():
+                for event in player.events:
+                    if k in event:
+                        player.build = v
+                        break
+
             player.graph_time = tuple(map(lambda x: round(x, 1), player.graph_time))
             DPS_data = numpy.array(player.DMG_graph_data, dtype=numpy.float64).cumsum()
             player.DPS_graph_data = tuple(DPS_data / player.graph_time)
 
-    def analyze_computers(self):
+    def analyze_critters(self):
         """
         Analyze map entities Computers to determine:
             - The map type
             - The difficulty of the map
 
         If new results are obtained, this overrides the values previously set
         if detect_line() was called during the creation of the Combat object.
@@ -277,51 +298,52 @@
 
         if self.map and self.difficulty:
             return
 
         if self.map == "Combat":
             return
 
-        for entity_id, entity in self.computers.items():
+        for entity_id, entity in self.critters.items():
             entity_name = get_entity_name(entity_id)
-            self.add_entity_to_computer_meta(entity_name)
-            self.computer_meta[entity_name]["count"] += 1
-            self.computer_meta[entity_name]["deaths"] += entity.deaths
-            self.computer_meta[entity_name]["total_hull_damage_taken"].append(entity.total_hull_damage_taken)
+            self.add_entity_to_critter_meta(entity_name)
+            self.critter_meta[entity_name]["count"] += 1
+            self.critter_meta[entity_name]["deaths"] += entity.deaths
+            total_hull_damage_taken = self.critter_meta[entity_name]["total_hull_damage_taken"]
+            total_hull_damage_taken.append(entity.total_hull_damage_taken)
 
         data = Detection.MAP_DIFFICULTY_ENTITY_DEATH_COUNTS.get(self.map)
         if data is None:
             self.difficulty = _difficulty
             return
 
         for difficulty, entry in data.items():
-            if check_difficulty_deaths(entry, self.computer_meta):
+            if check_difficulty_deaths(entry, self.critter_meta):
                 _difficulty = difficulty
                 break
 
         data = Detection.MAP_DIFFICULTY_ENTITY_HULL_COUNTS.get(self.map)
         if data is None:
             self.difficulty = _difficulty
             return
 
         matched = False
         for difficulty, entry in data.items():
-            if check_difficulty_damage(entry, self.computer_meta):
+            if check_difficulty_damage(entry, self.critter_meta):
                 matched = True
                 _difficulty = difficulty
                 break
         if not matched:
             return
 
         self.difficulty = _difficulty
 
-    def add_entity_to_computer_meta(self, entity_name):
-        """Adds a new entry to the computer metadata"""
-        if self.computer_meta.get(entity_name) is None:
-            self.computer_meta[entity_name] = {
+    def add_entity_to_critter_meta(self, entity_name):
+        """Adds a new entry to the critter metadata"""
+        if self.critter_meta.get(entity_name) is None:
+            self.critter_meta[entity_name] = {
                 "count": 0,
                 "deaths": 0,
                 "total_hull_damage_taken": [],
             }
 
     @property
     def duration(self):
@@ -335,20 +357,21 @@
     @property
     def player_dict(self):
         """Returns the list of players - for compatibility with previous versions"""
         return self.players
 
     def __repr__(self) -> str:
         return (
-            f"<{self.__class__.__name__} - Map: {self.map} - Difficulty: {self.difficulty} - Datetime: "
-            f"{self.start_time}>"
+            f"<{self.__class__.__name__} - Map: {self.map} - Difficulty: {self.difficulty} - "
+            f"Datetime: {self.start_time}>"
         )
 
     def __gt__(self, other):
         if not isinstance(other, Combat):
-            raise TypeError(f"Cannot compare {self.__class__.__name__} to {other.__class__.__name__}")
+            raise TypeError(
+                    f"Cannot compare {self.__class__.__name__} to {other.__class__.__name__}")
         if isinstance(self.date_time, datetime) and isinstance(self.date_time, datetime):
             return self.date_time > other.date_time
         if not isinstance(self.date_time, datetime) and isinstance(self.date_time, datetime):
             return False
         if isinstance(self.date_time, datetime) and not isinstance(other.date_time, datetime):
             return True
```

### Comparing `sto_oscr-2024.3b40/OSCR/datamodels.py` & `sto_oscr-2024.4b20/OSCR/datamodels.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from typing import Optional, Iterable
 from datetime import datetime
 from collections import namedtuple
 
 import numpy
 
-LogLine = namedtuple('LogLine', 
-        ('timestamp',
-        'owner_name', 
-        'owner_id', 
-        'source_name', 
-        'source_id', 
-        'target_name', 
-        'target_id', 
-        'event_name', 
-        'event_id', 
-        'type', 
-        'flags', 
-        'magnitude', 
-        'magnitude2'))
+LogLine = namedtuple(
+    'LogLine',
+    (
+        'timestamp',
+        'owner_name',
+        'owner_id',
+        'source_name',
+        'source_id',
+        'target_name',
+        'target_id',
+        'event_name',
+        'event_id',
+        'type',
+        'flags',
+        'magnitude',
+        'magnitude2'
+    )
+)
+
 
 class OverviewTableRow:
     '''
     Contains a single row of data
     '''
 
-    def __init__(self, name:str, handle:str):
+    def __init__(self, name: str, handle: str):
         self.name: str = name
         self.handle: str = handle
         self.combat_time: float = 0.0
         self.DPS: float = 0.0
         self.total_damage: float = 0.0
         self.debuff: float = 0.0
         self.attacks_in_share: float = 0.0
@@ -46,29 +51,30 @@
         self.total_attacks: int = 0
         self.hull_attacks: int = 0
         self.attacks_in_num: int = 0
         self.heal_crit_num: int = 0
         self.heal_num: int = 0
         self.crit_num: int = 0
         self.misses: int = 0
-        
+
         self.resistance_sum: float = 0.0
         self.DMG_graph_data: list[float] = list()
         self.DPS_graph_data: list[float] = list()
         self.graph_time: list[float] = list()
         self.damage_buffer: float = 0.0
-        self.combat_start: float = None
-        self.combat_end: float = None
+        self.combat_interval: tuple[float] = None
+        self.events: list[str] = list()
+        self.build: str = "Unknown"
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}: {self.name}{self.handle}>'
-    
+
     def __len__(self) -> int:
         return 25
-    
+
     def __getitem__(self, position):
         entries = {
             0: self.name,
             1: self.handle,
             2: self.combat_time,
             3: self.DPS,
             4: self.total_damage,
@@ -123,37 +129,41 @@
             "attacks_in_num": self.attacks_in_num,
             "attacks_in_share": self.attacks_in_share,
             "heal_crit_chance": self.heal_crit_chance,
             "taken_damage_share": self.taken_damage_share,
             "total_damage_taken": self.total_damage_taken,
             "total_hull_damage_taken": self.total_hull_damage_taken,
             "total_shield_damage_taken": self.total_shield_damage_taken,
+            "build": self.build,
         }
 
+
 class AnalysisTableRow():
     """
     Superclass for damage and heal table rows
     """
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}: {self.name}{self.handle}>'
 
+
 class DamageTableRow(AnalysisTableRow):
     """
-    Contains a single row of data in the analysis table. Unpacks into: (name, handle, total_damage, 
-    max_one_hit, kills, total_attacks, misses, crit_num, flank_num, total_shield_damage, total_hull_damage,
-    total_base_damage, combat_time, hull_attacks, shield_attacks)
+    Contains a single row of data in the analysis table. Unpacks into: (name, handle, total_damage,
+    max_one_hit, kills, total_attacks, misses, crit_num, flank_num, total_shield_damage,
+    total_hull_damage, total_base_damage, combat_time, hull_attacks, shield_attacks)
     """
     def __init__(self, name: str, handle: str, id: str):
         """
         Parameters:
         - :param name: name of the entity
         - :param handle: handle of the entity
         - :param id: id of the entity
         """
-        # commented attributes represent additional fields in the final result, but are not required here
+        # commented attributes represent additional fields in the final result, that are not
+        # required here
         self.name: str = name if name else '*'
         self.handle: str = handle
         # self.DPS: float = 0.0
         self.total_damage: float = 0.0
         # self.debuff: float = 0.0
         self.max_one_hit: float = 0.0
         # self.crit_chance: float = 0.0
@@ -169,23 +179,23 @@
         self.total_hull_damage: float = 0.0
         # self.hull_DPS: float = 0.0
         self.total_base_damage: float = 0.0
         # self.total_base_DPS: float = 0.0
         self.combat_time: float = 0.0
         self.hull_attacks: int = 0
         self.shield_attacks: int = 0
-        
+
         self.id: str = id
         self.resistance_sum: float = 0.0
         self.combat_start: float = None
         self.combat_end: float = None
-    
+
     def __len__(self) -> int:
         return 15
-    
+
     def __getitem__(self, position: int):
         entries = {
             0: self.name,
             1: self.handle,
             2: self.total_damage,
             3: self.max_one_hit,
             4: self.kills,
@@ -201,29 +211,32 @@
             14: self.shield_attacks,
         }
 
         if position >= len(entries):
             raise StopIteration()
 
         return entries[position]
-    
+
+
 class HealTableRow(AnalysisTableRow):
     """
-    Contains a single row of data in the analysis table. Unpacks into: (name, handle, total_heal, hull_heal, 
-    shield_heal, max_one_heal, heal_ticks, critical_heals, combat_time, hull_heal_ticks, shield_heal_ticks)
+    Contains a single row of data in the analysis table. Unpacks into: (name, handle, total_heal,
+    hull_heal, shield_heal, max_one_heal, heal_ticks, critical_heals, combat_time, hull_heal_ticks,
+    shield_heal_ticks)
     """
 
     def __init__(self, name: str, handle: str, id: str):
         """
         Parameters:
         - :param name: name of the entity
         - :param handle: handle of the entity
         - :param id: id of the entity
         """
-        # commented attributes represent additional fields in the final result, but are not required here
+        # commented attributes represent additional fields in the final result, that are not
+        # required here
         self.name: str = name if name else '*'
         self.handle: str = handle
         # self.HPS: float = 0.0
         self.total_heal: float = 0.0
         self.hull_heal: float = 0.0
         # self.hull_HPS: float = 0.0
         self.shield_heal: float = 0.0
@@ -234,19 +247,19 @@
         self.critical_heals: int = 0
         self.combat_time: float = 0.0
         self.hull_heal_ticks: int = 0
         self.shield_heal_ticks: int = 0
 
         self.id: str = id
         self.combat_start: float = None
-        self.combat_end: flaot = None
+        self.combat_end: float = None
 
     def __len__(self) -> int:
         return 11
-    
+
     def __getitem__(self, position: int):
         entries = {
             0: self.name,
             1: self.handle,
             2: self.total_heal,
             3: self.hull_heal,
             4: self.shield_heal,
@@ -259,14 +272,15 @@
         }
 
         if position >= len(entries):
             raise StopIteration()
 
         return entries[position]
 
+
 class TreeItem():
     """
     Item that contains data and children optionally.
     """
 
     def __init__(self, data: Iterable, parent, parse_duration: int = 0):
         """
@@ -278,54 +292,55 @@
         self.data = data
         self.graph_data = numpy.zeros(parse_duration, numpy.float64)
         self.parent = parent
         self._children = list()
 
     def __repr__(self):
         return f'<{self.__class__.__name__}: data={self.data}>'
-    
+
     def __iter__(self):
         return iter(self.data)
 
-    def get_child(self, row:int):
+    def get_child(self, row: int):
         try:
             return self._children[row]
         except IndexError:
             return None
-    
+
     def append_child(self, item):
         self._children.append(item)
 
     @property
     def child_count(self):
         return len(self._children)
-    
+
     @property
     def row(self):
         if self.parent is not None:
             return self.parent._children.index(self)
         return 0
-    
+
     @property
     def column_count(self):
         return len(self.data)
-    
-    def get_data(self, column:int):
+
+    def get_data(self, column: int):
         try:
             return self.data[column]
         except IndexError:
             if column == 0:
                 return self.data
             return None
 
+
 class TreeModel():
     """
     Data model that contains a hierachical table.
     """
-    
+
     def __init__(self, header: tuple[str]):
         self.actor_index = dict()
         self.ability_index = dict()
         self.pet_group_index = dict()
         self.pet_index = dict()
         self.target_index = dict()
         self.source_index = dict()
@@ -333,16 +348,17 @@
         self._player = TreeItem(['Player'] + [''] * (len(header) - 1), self._root)
         self._npc = TreeItem(['NPC'] + [''] * (len(header) - 1), self._root)
         self._root.append_child(self._player)
         self._root.append_child(self._npc)
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__} with columns {self._root.data}>'
-    
-    def add_actor(self, name: str, handle: str, id: str, row_constructor: AnalysisTableRow,
+
+    def add_actor(
+            self, name: str, handle: str, id: str, row_constructor: AnalysisTableRow,
             player: bool = True) -> TreeItem:
         """
         Adds Player or NPC to model.
 
         Parameters:
         - :param name: name of the player or NPC
         - :param handle: handle of the player or NPC (NPC handle is an id number)
@@ -412,15 +428,16 @@
         pet = TreeItem(name, pet_group)
         pet_group.append_child(pet)
         self.pet_index[pet_id] = pet
         self.ability_index[pet_id] = dict()
         self.target_index[pet_id] = dict()
         return pet
 
-    def add_target(self, data: AnalysisTableRow, target_id: str, ability: TreeItem, ability_id: str,
+    def add_target(
+            self, data: AnalysisTableRow, target_id: str, ability: TreeItem, ability_id: str,
             actor_id: str, parse_duration: int) -> TreeItem:
         """
         Adds target to model. target is inserted as child to the given ability.
 
         Parameters:
         - :param data: row of data for the target. First entry must be the name of the target
         - :param target_id: unique id string of the target for use in index
@@ -429,38 +446,40 @@
 
         :return: added target
         """
         target = TreeItem(data, ability, parse_duration)
         ability.append_child(target)
         self.target_index[actor_id][ability_id][target_id] = target
         return target
-    
-    def add_source_actor(self, name: tuple[str], source_id: str, actor: TreeItem, actor_id: str) -> TreeItem:
+
+    def add_source_actor(
+            self, name: tuple[str], source_id: str, actor: TreeItem, actor_id: str) -> TreeItem:
         """
-        Adds source actor to model. Source actor is inserted as child to the given actor. Used for incoming
-        damage / heal table.
+        Adds source actor to model. Source actor is inserted as child to the given actor. Used for
+        incoming damage / heal table.
 
         Parameters:
         - :param name: name of the source
         - :param source_id: unique id string of the source for use in index
         - :param actor: actor TreeItem that is the parent of the ability
 
         :return: added source
         """
         source = TreeItem(name, actor)
         actor.append_child(source)
         self.source_index[actor_id][source_id] = source
         self.ability_index[actor_id][source_id] = dict()
         return source
-    
-    def add_source_ability(self, data: AnalysisTableRow, ability_id: str, source: TreeItem, source_id: str,
+
+    def add_source_ability(
+            self, data: AnalysisTableRow, ability_id: str, source: TreeItem, source_id: str,
             actor_id: str, parse_duration: int) -> TreeItem:
         """
-        Adds ability to model. Ability is inserted as child to the given source. Used for incoming damage / 
-        heal table
+        Adds ability to model. Ability is inserted as child to the given source. Used for incoming
+        damage / heal table
 
         Parameters:
         - :param data: row of data for the target. First entry must be the name of the target
         - :param ability_id: unique id string of the target for use in index
         - :param ability: ability TreeItem that is the parent of the target
         - :param parse_duration: seconds between the first and last line of the combat, rounded up
```

### Comparing `sto_oscr-2024.3b40/OSCR/detection.py` & `sto_oscr-2024.4b20/OSCR/detection.py`

 * *Files 26% similar despite different names*

```diff
@@ -238,14 +238,39 @@
                 "Space_Borg_Wolf359_Escape_Pod_Tractor_Beam": 2081960,  # Assumption
                 "Space_Borg_Frigate_Wolf359": 2081960,
                 "Space_Borg_Cruiser_Wolf359": 0,
             }
         },
     }
 
+    BUILD_DETECTION_ABILITIES = {
+        # DEW
+        "Surgical Strikes III": "Surgical Strikes",
+        "Reroute Reserves to Weapons": "Reroute Reserves to Weapons",
+        "Exceed Rated Limits": "Exceed Rated Limits",
+        "Rapid Fire III": "Cannons: Rapid Fire",
+        "Scatter Volley III": "Cannons: Scatter Volley",
+        "Overload III": "Beams: Overload",
+        "Fire at Will III": "Beams: Fire At Will",
+        # Kinetic
+        "Isolytic Tear": "Kinetic",
+        # EPG
+        "Electrified Anomalies": "Exotic",
+        "Deteriorating Secondary Deflector": "Exotic",
+        "Gravity Well III": "Exotic",
+        # Support
+        "Greater Than The Sum": "Support",
+        # Lower Rank abilities that may be commonly used.
+        "Rapid Fire II": "Cannons: Rapid Fire",
+        "Scatter Volley II": "Cannons: Scatter Volley",
+        "Fire at Will II": "Beams: Fire At Will",
+        # Classify these last
+        "Thalaron Pulse": "Thalaron Pulse",
+    }
+
     @staticmethod
     def detect_line(line: LogLine) -> tuple:
         """
         Do a very shallow map detect based on a log line only
         taking NPCs into consideration.
 
         return: a tuple in the form of (Map, Difficulty)
```

### Comparing `sto_oscr-2024.3b40/OSCR/iofunc.py` & `sto_oscr-2024.4b20/OSCR/iofunc.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import gzip
 from io import TextIOWrapper
 from re import sub as re_sub
 from datetime import timedelta
 
 from .utilities import to_datetime, logline_to_str
 
-def format_timestamp(timestamp:str) -> str:
+
+def format_timestamp(timestamp: str) -> str:
     '''
     Formats timestamp. '24:01:13:04:37:45.7' becomes '24-01-13_04:37:45'
     '''
     return timestamp.replace(':', '-', 2).replace(':', '_', 1).split('.')[0]
 
+
 def is_gz_file(filepath):
     with open(filepath, 'rb') as test_f:
         return test_f.read(2) == b'\x1f\x8b'
 
-def get_lines(log_path:str) -> list:
+
+def get_lines(log_path: str) -> list:
     '''
     Returns a list of lines parsed from the log file.
     This function is aware that the file being passed in could be gzipped.
     '''
     lines_list = list()
 
     if is_gz_file(log_path):
@@ -29,52 +32,61 @@
             lines_list = file.readlines()
     else:
         with open(log_path, 'r', encoding='utf-8') as file:
             lines_list = file.readlines()
 
     return lines_list
 
-def get_combat_log_data(log_path:str):
+
+def get_combat_log_data(log_path: str):
     if not (os.path.exists(log_path) and os.path.isfile(log_path)):
         raise FileNotFoundError(f'Invalid Path: {log_path}')
     if os.path.getsize(log_path) > 125 * 1024 * 1024:
-        raise FileExistsError(f'File at {log_path} is too large. Use get_massive_log_data(...) instead')
+        raise FileExistsError(
+                f'File at {log_path} is too large. Use get_massive_log_data(...) instead')
     lines_list = get_lines(log_path)
     if len(lines_list) < 1 or not lines_list[0].strip():
         raise TypeError('File must contain at least one not-empty line')
-    if not '::' in lines_list[0] or not ',' in lines_list[0]:
-        raise TypeError("First line invalid. First line may not be empty and must contain '::' and ','.")
+    if '::' not in lines_list[0] or ',' not in lines_list[0]:
+        raise TypeError(
+                "First line invalid. First line may not be empty and must contain '::' and ','.")
     return lines_list
 
-def get_massive_log_data(log_path:str, temp_folder_path:str, combat_distance:int = 100) -> tuple[list, list]:
+
+def get_massive_log_data(
+        log_path: str, temp_folder_path: str, combat_distance: int = 100) -> tuple[list, list]:
     '''
-    Get log lines from massive combatlog file. Return the latest about 480000 lines of the log as well
-    as paths to temporary files containing the remaining lines.
+    Get log lines from massive combatlog file. Return the latest about 480000 lines of the log as
+    well as paths to temporary files containing the remaining lines.
     '''
     absolute_target_path = os.path.abspath(temp_folder_path)
     if not (os.path.exists(log_path) and os.path.isfile(log_path)):
         raise FileNotFoundError(f'Invalid Log Path: {log_path}')
     if not (os.path.exists(absolute_target_path) and os.path.isdir(absolute_target_path)):
         raise FileNotFoundError(f'Invalid or not existing target path: {absolute_target_path}')
-    splitted_log_paths = split_log_by_lines(log_path, temp_folder_path, combat_distance=combat_distance)
+    splitted_log_paths = split_log_by_lines(
+            log_path, temp_folder_path, combat_distance=combat_distance)
     with open(splitted_log_paths[-1], 'r', encoding='utf-8') as file:
         lines_list = file.readlines()
     return (lines_list, splitted_log_paths)
 
-def split_log_by_lines(log_path:str, target_path:str, approx_lines_per_file:int = 480000, 
-        combat_distance:int = 100) -> list:
+
+def split_log_by_lines(
+        log_path: str, target_path: str, approx_lines_per_file: int = 480000,
+        combat_distance: int = 100) -> list:
     '''
-    Splits the combat at log_path into multiple files saved in the directory at target_path and 
+    Splits the combat at log_path into multiple files saved in the directory at target_path and
     returns the paths to the files.
     '''
-    def save_partial_log(directory_path:str, filename:str, lines:list, filepath_list:list) -> str:
+    def save_partial_log(
+            directory_path: str, filename: str, lines: list, filepath_list: list) -> str:
         start_time = format_timestamp(lines[0].split('::')[0])
         end_time = format_timestamp(lines[-1].split('::')[0])
         new_filename = sanitize_file_name(f'[{start_time}--{end_time}]{filename}')
-        new_path = f'{directory_path}\\{new_filename}'
+        new_path = f'{directory_path}/{new_filename}'
         try:
             save_log(new_path, lines)
         except FileExistsError:
             new_path += sanitize_file_name(f'{new_path}(2).log')
             try:
                 save_log(new_path, lines)
             except FileExistsError:
@@ -98,43 +110,48 @@
                 save_partial_log(absolute_target_path, original_filename, current_lines, filepaths)
                 return filepaths
             last_log_time = to_datetime(current_lines[-1].split('::')[0])
             # inner loop: finds the end of the combat
             while True:
                 line = log_file.readline()
                 if not line:
-                    save_partial_log(absolute_target_path, original_filename, current_lines, filepaths)
+                    save_partial_log(
+                            absolute_target_path, original_filename, current_lines, filepaths)
                     return filepaths
                 log_time = to_datetime(line.split('::')[0])
                 if log_time - last_log_time > combat_delta:
-                    save_partial_log(absolute_target_path, original_filename, current_lines, filepaths)
+                    save_partial_log(
+                            absolute_target_path, original_filename, current_lines, filepaths)
                     current_lines = [line]
                     break
                 current_lines.append(line)
-        
-def read_lines(file:TextIOWrapper, num:int, input_list=None) -> tuple[list, bool]:
+
+
+def read_lines(file: TextIOWrapper, num: int, input_list=None) -> tuple[list, bool]:
     '''
-    Read num lines from file and return them along with a boolean value indicating whether the end of the
-    file was reached during the read process.
+    Read num lines from file and return them along with a boolean value indicating whether the end
+    of the file was reached during the read process.
     '''
     if input_list is None:
         lines = list()
     else:
         lines = input_list
     end_of_file = False
     for _ in range(num):
         line = file.readline()
         if not line:
             end_of_file = True
             break
         lines.append(line)
     return (lines, end_of_file)
 
-def split_log_by_combat(log_path: str, target_path: str, first_num: str, last_num: str, 
-        combat_distance: int = 100, excluded_event_ids: list = []):
+
+def split_log_by_combat(
+        log_path: str, target_path: str, first_num: str, last_num: str, combat_distance: int = 100,
+        excluded_event_ids: list = []):
     """
     Splits off a number of combats from logfile and saves them to target path.
 
     Parameters:
     - :param log_path: path to existing logfile
     - :param target_path: path to target file; will be overwritten if already existing!
     - :param first_num: first combat to include in the new file
@@ -166,79 +183,80 @@
                     break
                 log_time = to_datetime(current_line.split('::')[0])
                 if log_time - last_log_time > combat_delta:
                     if first_num <= current_combat and current_combat <= last_num:
                         if not current_combat_lines[0].split(',')[7] in excluded_event_ids:
                             target_file.writelines(current_combat_lines)
                     if to_end:
-                            last_num += 1
+                        last_num += 1
                     if current_combat >= last_num:
                         return
                     if not current_combat_lines[0].split(',')[7] in excluded_event_ids:
                         current_combat += 1
                     current_combat_lines = list()
                 current_combat_lines.append(current_line)
                 last_log_time = log_time
 
 
-def save_log(path:str, lines:list, overwrite: bool = False):
+def save_log(path: str, lines: list, overwrite: bool = False):
     '''
     Saves lines to new file.
 
     Parameters:
     - :param path: path to log file
     - :param lines: list of lines to write to file; individual lines may be  of type str or LogLine
     - :param overwrite: overwrites existing file when set to True
     '''
     if os.path.exists(path) and not overwrite:
         raise FileExistsError(f'File "{path}" already exists.')
     with open(path, 'w', encoding='utf-8') as file:
         for line in map(logline_to_str, lines):
             file.write(line)
 
-def reset_temp_folder(path:str):
+
+def reset_temp_folder(path: str):
     '''
     Deletes and re-creates folder housing temporary log files.
     '''
     if os.path.exists(path):
         if os.path.isdir(path):
             shutil.rmtree(path)
         else:
             raise FileExistsError(f'Expected path to folder, got "{path}"')
     os.mkdir(path)
-        
 
 
 def sanitize_file_name(txt, chr_set='extended') -> str:
     """Converts txt to a valid filename.
 
     Parameters:
     - :param txt: The path to convert.
-    - :param chr_set: 
+    - :param chr_set:
         - 'printable':    Any printable character except those disallowed on Windows/*nix.
         - 'extended':     'printable' + extended ASCII character codes 128-255
         - 'universal':    For almost *any* file system.
     """
     FILLER = '-'
     MAX_LEN = 255  # Maximum length of filename is 255 bytes in Windows and some *nix flavors.
 
     # Step 1: Remove excluded characters.
     BLACK_LIST = set(chr(127) + r'<>:"/\|?*')
     white_lists = {
         'universal': {'-.0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'},
         'printable': {chr(x) for x in range(32, 127)} - BLACK_LIST,     # 0-32, 127 are unprintable,
-        'extended' : {chr(x) for x in range(32, 256)} - BLACK_LIST,
+        'extended': {chr(x) for x in range(32, 256)} - BLACK_LIST,
     }
     white_list = white_lists[chr_set]
     result = ''.join(x if x in white_list else FILLER for x in txt)
 
     # Step 2: Device names, '.', and '..' are invalid filenames in Windows.
-    DEVICE_NAMES = ('CON', 'PRN', 'AUX', 'NUL', 'COM1', 'COM2', 'COM3', 'COM4', 'COM5', 'COM6', 'COM7',
-            'COM8', 'COM9', 'LPT1', 'LPT2', 'LPT3', 'LPT4', 'LPT5', 'LPT6', 'LPT7', 'LPT8', 'LPT9', 'CONIN$',
-            'CONOUT$', '..', '.')
+    DEVICE_NAMES = (
+            'CON', 'PRN', 'AUX', 'NUL', 'COM1', 'COM2', 'COM3', 'COM4', 'COM5', 'COM6',
+            'COM7', 'COM8', 'COM9', 'LPT1', 'LPT2', 'LPT3', 'LPT4', 'LPT5', 'LPT6', 'LPT7', 'LPT8',
+            'LPT9', 'CONIN$', 'CONOUT$', '..', '.')
     if '.' in txt:
         name, _, ext = result.rpartition('.')
         ext = f'.{ext}'
     else:
         name = result
         ext = ''
     if name in DEVICE_NAMES:
```

### Comparing `sto_oscr-2024.3b40/OSCR/main.py` & `sto_oscr-2024.4b20/OSCR/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from datetime import timedelta
 import os
 
 from .datamodels import LogLine, TreeItem
-from .iofunc import get_combat_log_data, split_log_by_lines, reset_temp_folder, save_log
-from .utilities import to_datetime, datetime_to_display
-from .parser import analyze_combat
 from .combat import Combat
+from .iofunc import get_combat_log_data, reset_temp_folder, save_log, split_log_by_lines
+from .parser import analyze_combat
+from .utilities import datetime_to_display, to_datetime
+
 
 class OSCR():
 
-    version = '2024.03b040'
+    version = '2024.04b020'
 
-    def __init__(self, log_path:str = None, settings:dict = None):
+    def __init__(self, log_path: str = None, settings: dict = None):
         self.log_path = log_path
         self.combats: list[Combat] = list()
         self.combats_pointer = None
         self.excess_log_lines = list()
         self.combatlog_tempfiles = list()
         self.combatlog_tempfiles_pointer = None
         self._settings = {
             'combats_to_parse': 10,
             'seconds_between_combats': 100,
             'excluded_event_ids': ['Autodesc.Combatevent.Falling'],
             'graph_resolution': 0.2,
             'split_log_after': 480000,
-            'templog_folder_path': f'{os.path.dirname(os.path.abspath(__file__))}\\~temp_log_files'
+            'templog_folder_path': f'{os.path.dirname(os.path.abspath(__file__))}/~temp_log_files'
         }
         if settings is not None:
             self._settings.update(settings)
 
     @property
     def analyzed_combats(self) -> list[str]:
         '''
@@ -37,59 +38,61 @@
         res = list()
         for c in self.combats:
             if c.difficulty:
                 res.append(f'{c.map} {c.difficulty} {datetime_to_display(c.start_time)}')
             else:
                 res.append(f'{c.map} {datetime_to_display(c.start_time)}')
         return res
-    
+
     @property
     def active_combat(self):
         '''
         Combat currently active (selected).
         '''
         if self.combats_pointer is not None:
             return self.combats[self.combats_pointer]
         else:
             return None
-    
+
     @property
     def navigation_up(self) -> bool:
         '''
         Indicates whether newer combats are available, but not yet analyzed.
         '''
         if self.combatlog_tempfiles_pointer is None:
             return False
         return self.combatlog_tempfiles_pointer < len(self.combatlog_tempfiles) - 1
-    
+
     @property
     def navigation_down(self) -> bool:
         '''
         Indicates whether older combats are available, but not yet analyzed.
         '''
         if len(self.excess_log_lines) > 0:
             return True
         if self.combatlog_tempfiles_pointer is None:
             return False
         return self.combatlog_tempfiles_pointer > 0
 
     def analyze_log_file(self, total_combats=None, extend=False, log_path=None):
         '''
-        Analyzes the combat at self.log_path and replaces self.combats with the newly parsed combats.
-        
+        Analyzes the combat at self.log_path and replaces self.combats with the newly parsed
+        combats.
+
         Parameters:
-        - :param total_combats: holds the number of combats that should be in self.combats after the method is 
-        finished.
-        - :param extend: extends the list of current combats to match the number of total_combats by analyzing
-        excess_log_lines
-        - :param log_path: specify log path different from self.log_path to be analyzed. Has no effect when
-        parameter extend is True
+        - :param total_combats: holds the number of combats that should be in self.combats after
+        the method is finished.
+        - :param extend: extends the list of current combats to match the number of total_combats
+        by analyzing excess_log_lines
+        - :param log_path: specify log path different from self.log_path to be analyzed. Has no
+        effect when parameter extend is True
         '''
         if self.log_path is None and log_path is None:
-            raise AttributeError('"self.log_path" or parameter "log_path" must contain a path to a log file.')
+            raise AttributeError(
+                    '"self.log_path" or parameter "log_path" must contain a path to a log file.')
         if total_combats is None:
             total_combats = self._settings['combats_to_parse']
         if extend:
             if total_combats <= len(self.combats):
                 return
             log_lines = self.excess_log_lines
             self.excess_log_lines = list()
@@ -131,96 +134,100 @@
                 current_combat.end_time = last_log_time
 
         current_combat.start_time = last_log_time
         self.combats.append(current_combat)
 
     def analyze_massive_log_file(self, total_combats=None):
         '''
-        Analyzes the combat at self.log_path and replaces self.combats with the newly parsed combats.
-        Used to analyze log files larger than around 500000 lines. Wraps around self.analyze_log_file.
+        Analyzes the combat at self.log_path and replaces self.combats with the newly parsed
+        combats. Used to analyze log files larger than around 500000 lines. Wraps around
+        self.analyze_log_file.
 
         Parameters:
-        - :param total_combats: holds the number of combats that should be in self.combats after the method is 
-        finished.
+        - :param total_combats: holds the number of combats that should be in self.combats after
+        the method is finished.
         '''
         if self.log_path is None:
             raise AttributeError('"self.log_path" must contain a path to a log file.')
         temp_folder_path = self._settings['templog_folder_path']
         reset_temp_folder(temp_folder_path)
-        self.combatlog_tempfiles = split_log_by_lines(self.log_path, temp_folder_path, 
-                approx_lines_per_file=480000)
+        self.combatlog_tempfiles = split_log_by_lines(
+                self.log_path, temp_folder_path, approx_lines_per_file=480000)
         self.combatlog_tempfiles_pointer = len(self.combatlog_tempfiles) - 1
-        self.analyze_log_file(total_combats, 
-                log_path=self.combatlog_tempfiles[self.combatlog_tempfiles_pointer])
-        
+        self.analyze_log_file(
+                total_combats, log_path=self.combatlog_tempfiles[self.combatlog_tempfiles_pointer])
+
     def navigate_log(self, direction: str = 'down'):
         '''
-        Analyzes earlier combats when direction is "down"; loads earlier templog file if current file is
-        exhausted; loads later combatlog file if direction is "up".
+        Analyzes earlier combats when direction is "down"; loads earlier templog file if current
+        file is exhausted; loads later combatlog file if direction is "up".
 
         Parameters:
         - :param direction: "down" and "up"
 
         :return: True when logfile was changed; False otherwise
         '''
         if direction == 'down' and self.navigation_down:
             if self.combatlog_tempfiles_pointer is None:
                 total_combat_num = len(self.combats) + self._settings['combats_to_parse']
                 self.analyze_log_file(total_combats=total_combat_num, extend=True)
                 return False
             else:
                 self.combatlog_tempfiles_pointer -= 1
-                self.analyze_log_file(log_path=self.combatlog_tempfiles[self.combatlog_tempfiles_pointer])
+                self.analyze_log_file(
+                        log_path=self.combatlog_tempfiles[self.combatlog_tempfiles_pointer])
                 return True
         elif direction == 'up' and self.navigation_up:
-           self.combatlog_tempfiles_pointer += 1
-           self.analyze_log_file(log_path=self.combatlog_tempfiles[self.combatlog_tempfiles_pointer])
-           return True
-
+            self.combatlog_tempfiles_pointer += 1
+            self.analyze_log_file(
+                    log_path=self.combatlog_tempfiles[self.combatlog_tempfiles_pointer])
+            return True
 
-    def shallow_combat_analysis(self, combat_num:int) -> tuple[list, ...]:
+    def shallow_combat_analysis(self, combat_num: int) -> tuple[list, ...]:
         '''
         Analyzes combat from currently available combats in self.combat.
 
         Parameters:
         - :param combat_num: index of the combat in self.combats
 
         :return: tuple containing the overview table, DPS graph data and DMG graph data
         '''
         try:
             combat = self.combats[combat_num]
             combat.analyze_shallow(graph_resolution=self._settings['graph_resolution'])
             self.combats_pointer = combat_num
         except IndexError:
-            raise AttributeError(f'Combat #{combat_num} you are trying to analyze has not been isolated yet.'
-                                 f'Number of isolated combats: {len(self.combats)} -- '
-                                 'Use OSCR.analyze_log_file() with appropriate arguments first.')
-        
+            raise AttributeError(
+                    f'Combat #{combat_num} you are trying to analyze has not been isolated yet. '
+                    f'Number of isolated combats: {len(self.combats)} -- Use '
+                    'OSCR.analyze_log_file() with appropriate arguments first.')
+
     def full_combat_analysis(self, combat_num: int) -> tuple[TreeItem]:
         '''
-        Analyzes combat 
+        Analyzes combat
         '''
         try:
             combat = self.combats[combat_num]
         except IndexError:
-            raise AttributeError(f'Combat #{combat_num} you are trying to analyze has not been isolated yet.'
-                                 f'Number of isolated combats: {len(self.combats)} -- '
-                                 'Use OSCR.analyze_log_file() with appropriate arguments first.')
+            raise AttributeError(
+                    f'Combat #{combat_num} you are trying to analyze has not been isolated yet.'
+                    f'Number of isolated combats: {len(self.combats)} -- Use '
+                    'OSCR.analyze_log_file() with appropriate arguments first.')
         dmg_out, dmg_in, heal_out, heal_in = analyze_combat(combat, self._settings)
         return dmg_out._root, dmg_in._root, heal_out._root, heal_in._root
-    
+
     def export_combat(self, combat_num: int, path: str):
         '''
         Exports combat to new logfile
 
         Parameters:
         - :param combat_num: index of the combat in self.combats
         - :param path: path to export the log to, will overwrite existing files
         '''
         try:
             log_lines = self.combats[combat_num].log_data
         except IndexError:
-            raise AttributeError(f'Combat #{combat_num} you are trying to save has not been isolated yet.'
-                                 f'Number of isolated combats: {len(self.combats)} -- '
-                                 'Use OSCR.analyze_log_file() with appropriate arguments first.')
+            raise AttributeError(
+                    f'Combat #{combat_num} you are trying to save has not been isolated yet.'
+                    f'Number of isolated combats: {len(self.combats)} -- Use '
+                    'OSCR.analyze_log_file() with appropriate arguments first.')
         save_log(path, log_lines, True)
-
```

### Comparing `sto_oscr-2024.3b40/OSCR/parser.py` & `sto_oscr-2024.4b20/OSCR/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,47 @@
 import numpy
 
-from .datamodels import TreeItem, TreeModel, AnalysisTableRow, DamageTableRow, HealTableRow, LogLine
 from . import TREE_HEADER, HEAL_TREE_HEADER
-from .utilities import get_handle_from_id, bundle
+from .datamodels import AnalysisTableRow, DamageTableRow, HealTableRow, LogLine, TreeItem, TreeModel
 from .combat import Combat
+from .utilities import bundle, get_handle_from_id
+
 
 def analyze_combat(combat: Combat, settings: dict) -> tuple[TreeModel, ...]:
     """
     Fully analyzes the given combat and returns the root TreeItem from the output model.
     """
     dmg_out_model = TreeModel(TREE_HEADER)
     dmg_in_model = TreeModel(TREE_HEADER)
     heal_out_model = TreeModel(HEAL_TREE_HEADER)
     heal_in_model = TreeModel(HEAL_TREE_HEADER)
     actor_combat_durations = dict()
     combat_duration_delta = combat.log_data[-1].timestamp - combat.log_data[0].timestamp
-    combat_duration_sec = int(combat_duration_delta.total_seconds()) + 1 # round up to full second
+    combat_duration_sec = int(combat_duration_delta.total_seconds()) + 1  # round up to full second
     combat_start = combat.log_data[0].timestamp
     relative_combat_sec = 0
     for line in combat.log_data:
-        
+
         timestamp = line.timestamp
         player_attacks = line.owner_id.startswith('P')
         player_attacked = line.target_id.startswith('P')
         is_shield_line = line.type == 'Shield'
         crit_flag, miss_flag, flank_flag, kill_flag, shield_break_flag = get_flags(line.flags)
-        is_heal = ((is_shield_line and line.magnitude < 0 and line.magnitude2 >= 0) 
+        is_heal = (
+                (is_shield_line and line.magnitude < 0 and line.magnitude2 >= 0)
                 or line.type == 'HitPoints')
 
         relative_combat_sec = (timestamp - combat_start).seconds
 
-        # Combat Duration
-        try:
-            actor_combat_durations[line.owner_id][1] = timestamp
-        except KeyError:
-            actor_combat_durations[line.owner_id] = [timestamp, timestamp]
-        try:
-            actor_combat_durations[line.source_id][1] = timestamp
-        except KeyError:
-            actor_combat_durations[line.source_id] = [timestamp, timestamp]
-        try:
-            actor_combat_durations[line.target_id][1] = timestamp
-        except KeyError:
-            actor_combat_durations[line.target_id] = [timestamp, timestamp]
-
         # HEALS
         if is_heal:
-            target_item, ability_target = get_outgoing_heal_target_row(heal_out_model, line, player_attacks,
-                    combat_duration_sec)
-            source_item, source_ability = get_incoming_target_row(heal_in_model, line, player_attacked, 
-                    HealTableRow, combat_duration_sec)
+            target_item, ability_target = get_outgoing_target_row(
+                    heal_out_model, line, player_attacks, HealTableRow, combat_duration_sec)
+            source_item, source_ability = get_incoming_target_row(
+                    heal_in_model, line, player_attacked, HealTableRow, combat_duration_sec)
 
             if crit_flag:
                 ability_target.critical_heals += 1
                 source_ability.critical_heals += 1
 
             magnitude = abs(line.magnitude)
             ability_target.total_heal += magnitude
@@ -77,33 +65,45 @@
                 source_ability.max_one_heal = magnitude
 
             target_item.graph_data[relative_combat_sec] += magnitude
             source_item.graph_data[relative_combat_sec] += magnitude
 
         # DAMAGE
         else:
-            target_item, ability_target = get_outgoing_target_row(dmg_out_model, line, player_attacks,
-                    combat_duration_sec)
-            source_item, source_ability = get_incoming_target_row(dmg_in_model, line, player_attacked, 
-                    DamageTableRow, combat_duration_sec)
-        
+            target_item, ability_target = get_outgoing_target_row(
+                    dmg_out_model, line, player_attacks, DamageTableRow, combat_duration_sec)
+            source_item, source_ability = get_incoming_target_row(
+                    dmg_in_model, line, player_attacked, DamageTableRow, combat_duration_sec)
+
+            # Combat Duration
+            # Heals, damage taken and self-damage don't affect combat time
+            if ability_target.name != '*':
+                try:
+                    actor_combat_durations[line.owner_id][1] = timestamp
+                except KeyError:
+                    actor_combat_durations[line.owner_id] = [timestamp, timestamp]
+                try:
+                    actor_combat_durations[line.source_id][1] = timestamp
+                except KeyError:
+                    actor_combat_durations[line.source_id] = [timestamp, timestamp]
+
             # get table data
             if miss_flag:
                 ability_target.misses += 1
                 source_ability.misses += 1
             if kill_flag:
                 ability_target.kills += 1
                 source_ability.kills += 1
             if flank_flag:
                 ability_target.flank_num += 1
                 source_ability.flank_num += 1
             if crit_flag:
                 ability_target.crit_num += 1
                 source_ability.crit_num += 1
-        
+
             magnitude = abs(line.magnitude)
             magnitude2 = abs(line.magnitude2)
             ability_target.total_damage += magnitude
             ability_target.total_base_damage += magnitude2
             ability_target.total_attacks += 1
             source_ability.total_damage += magnitude
             source_ability.total_base_damage += magnitude2
@@ -117,92 +117,100 @@
                 ability_target.total_hull_damage += magnitude
                 source_ability.total_hull_damage += magnitude
                 if not miss_flag and magnitude != 0 and magnitude2 != 0:
                     ability_target.resistance_sum += magnitude / magnitude2
                     source_ability.resistance_sum += magnitude / magnitude2
                 ability_target.hull_attacks += 1
                 source_ability.hull_attacks += 1
-            
+
             if magnitude > ability_target.max_one_hit:
                 ability_target.max_one_hit = magnitude
             if magnitude > source_ability.max_one_hit:
                 source_ability.max_one_hit = magnitude
 
             target_item.graph_data[relative_combat_sec] += magnitude
             source_item.graph_data[relative_combat_sec] += magnitude
-    
+
     for actor_id, (start_time, end_time) in actor_combat_durations.items():
         actor_combat_durations[actor_id] = round((end_time - start_time).total_seconds(), 1)
 
     merge_single_lines(dmg_out_model)
-    complete_damage_tree(dmg_out_model, actor_combat_durations)
-    complete_damage_tree(dmg_in_model, actor_combat_durations)
-    complete_heal_tree(heal_out_model, actor_combat_durations)
-    complete_heal_tree(heal_in_model, actor_combat_durations)
+    combat_duration = combat_duration_delta.total_seconds()
+    complete_damage_tree(dmg_out_model, actor_combat_durations, combat_duration)
+    complete_damage_tree(dmg_in_model, actor_combat_durations, combat_duration)
+    complete_heal_tree(heal_out_model, actor_combat_durations, combat_duration)
+    complete_heal_tree(heal_in_model, actor_combat_durations, combat_duration)
     return dmg_out_model, dmg_in_model, heal_out_model, heal_in_model
 
-def get_outgoing_target_row(tree_model: TreeModel, line: LogLine, player_attacks: bool, parse_duration: int
-        ) -> tuple[TreeItem, DamageTableRow]:
+
+def get_outgoing_target_row(
+        tree_model: TreeModel, line: LogLine, player_attacks: bool, row_constructor,
+        parse_duration: int) -> tuple[TreeItem, DamageTableRow]:
     '''
-    Adds the needed parents to the tree model and returns the newly created or already existing data row.
-    Also updates combat time of the actor.
+    Adds the needed parents to the tree model and returns the newly created or already existing
+    data row. Also updates combat time of the actor.
 
     Parameters:
     - :param tree_model: model to work on
     - :param line: log line that contains the ability
     - :param player_attacks: True when player attacks, False otherwise
     - :param parse_duration: seconds between the first and last line of the combat, rounded up
 
     :return: reference to newly created or existing data row
     '''
     attacker_id = (line.owner_id,)
     attacker_handle = get_handle_from_id(line.owner_id)
     if attacker_id in tree_model.actor_index:
         attacker = tree_model.actor_index[attacker_id]
     else:
-        attacker = tree_model.add_actor(line.owner_name, attacker_handle, attacker_id, 
-                DamageTableRow, player_attacks)
+        attacker = tree_model.add_actor(
+                line.owner_name, attacker_handle, attacker_id, DamageTableRow, player_attacks)
         attacker.data.combat_start = line.timestamp
     attacker.data.combat_end = line.timestamp
 
     if line.source_name:
         pet_group_id = (line.owner_id, line.source_name)
+        attacker_id = (line.owner_id, line.source_id)
         if pet_group_id in tree_model.pet_group_index:
             attacker = tree_model.pet_group_index[pet_group_id]
-        else:
+        # if attacking pet already in pet index: logfile is bugged (one pet has more than one
+        # entity name); pet group is not created in this case as it would not have any children
+        elif attacker_id not in tree_model.pet_index:
             attacker = tree_model.add_pet_group(line.source_name, pet_group_id, attacker)
 
-        attacker_id = (line.owner_id, line.source_id)
         if attacker_id in tree_model.pet_index:
             attacker = tree_model.pet_index[attacker_id]
         else:
-            attacker = tree_model.add_pet(line.source_name + 
-                    get_handle_from_id(line.source_id), attacker_id, attacker)
-    
+            attacker = tree_model.add_pet(
+                    line.source_name + get_handle_from_id(line.source_id), attacker_id, attacker)
+
     ability_id = line.event_name
     if ability_id in tree_model.ability_index[attacker_id]:
         ability = tree_model.ability_index[attacker_id][ability_id]
     else:
         ability = tree_model.add_ability(line.event_name, ability_id, attacker, attacker_id)
 
     ability_target_id = line.target_id
     if ability_target_id in tree_model.target_index[attacker_id][ability_id]:
         ability_target = tree_model.target_index[attacker_id][ability_id][ability_target_id]
     else:
-        ability_target = tree_model.add_target(DamageTableRow(line.target_name, 
+        ability_target = tree_model.add_target(row_constructor(
+                line.target_name,
                 get_handle_from_id(ability_target_id), ability_target_id), ability_target_id,
                 ability, ability_id, attacker_id, parse_duration)
-        
+
     return ability_target, ability_target.data
 
-def get_outgoing_heal_target_row(tree_model: TreeModel, line: LogLine, player_attacks: bool,
+
+def get_outgoing_heal_target_row(
+        tree_model: TreeModel, line: LogLine, player_attacks: bool,
         parse_duration: int) -> tuple[TreeItem, HealTableRow]:
     '''
-    Adds the needed parents to the tree model and returns the newly created or already existing data row.
-    Also updates combat time of the actor.
+    Adds the needed parents to the tree model and returns the newly created or already existing
+    data row. Also updates combat time of the actor.
 
     Parameters:
     - :param tree_model: model to work on
     - :param line: log line that contains the ability
     - :param player_attacks: True when player attacks, False otherwise
     - :param parse_duration: seconds between the first and last line of the combat, rounded up
 
@@ -215,40 +223,44 @@
     else:
         attacker_name = line.owner_name
         attacker_id = (line.owner_id,)
         attacker_handle = get_handle_from_id(line.owner_id)
     if attacker_id in tree_model.actor_index:
         attacker = tree_model.actor_index[attacker_id]
     else:
-        attacker = tree_model.add_actor(attacker_name, attacker_handle, attacker_id, 
-                HealTableRow, player_attacks)
+        attacker = tree_model.add_actor(
+                attacker_name, attacker_handle, attacker_id, HealTableRow, player_attacks)
         attacker.data.combat_start = line.timestamp
     attacker.data.combat_end = line.timestamp
 
     ability_id = line.event_name
     if ability_id in tree_model.ability_index[attacker_id]:
         ability = tree_model.ability_index[attacker_id][ability_id]
     else:
         ability = tree_model.add_ability(line.event_name, ability_id, attacker, attacker_id)
 
     ability_target_id = line.target_id
     if ability_target_id in tree_model.target_index[attacker_id][ability_id]:
         ability_target = tree_model.target_index[attacker_id][ability_id][ability_target_id]
     else:
-        ability_target = tree_model.add_target(HealTableRow(line.target_name, 
+        ability_target = tree_model.add_target(HealTableRow(
+                line.target_name,
                 get_handle_from_id(ability_target_id), ability_target_id), ability_target_id,
                 ability, ability_id, attacker_id, parse_duration)
-        
+
     return ability_target, ability_target.data
 
-def get_incoming_target_row(tree_model: TreeModel, line: LogLine, player_attacked: bool,
-        row_constructor: AnalysisTableRow, parse_duration: int) -> tuple[TreeItem, AnalysisTableRow]:
+
+def get_incoming_target_row(
+        tree_model: TreeModel, line: LogLine, player_attacked: bool,
+        row_constructor: AnalysisTableRow,
+        parse_duration: int) -> tuple[TreeItem, AnalysisTableRow]:
     '''
-    Adds the needed parents to the tree model and returns the newly created or already existing data row.
-    Also updates combat time of the actor.
+    Adds the needed parents to the tree model and returns the newly created or already existing
+    data row. Also updates combat time of the actor.
 
     Parameters:
     - :param tree_model: model to work on
     - :param line: log line that contains the ability
     - :param player_attacked: True when player is attacked, False otherwise
     - :param row_constructor: a new object returned by this constructor will hold the row data
     - :param parse_duration: seconds between the first and last line of the combat, rounded up
@@ -256,67 +268,72 @@
     :return: reference to newly created or existing TreItem and data row
     '''
     target_id = (line.target_id,)
     target_handle = get_handle_from_id(line.target_id)
     if target_id in tree_model.actor_index:
         target = tree_model.actor_index[target_id]
     else:
-        target = tree_model.add_actor(line.target_name, target_handle, target_id, row_constructor, 
-                player_attacked)
+        target = tree_model.add_actor(
+                line.target_name, target_handle, target_id, row_constructor, player_attacked)
         target.data.combat_start = line.timestamp
     target.data.combat_end = line.timestamp
 
     if line.source_name:
         source_id = line.source_id
         source_name = line.source_name
     else:
         source_id = line.owner_id
         source_name = line.owner_name
 
     if source_id in tree_model.source_index[target_id]:
         ability_source = tree_model.source_index[target_id][source_id]
     else:
-        ability_source = tree_model.add_source_actor((source_name, get_handle_from_id(source_id)), source_id, 
-                target, target_id)
+        ability_source = tree_model.add_source_actor(
+                (source_name, get_handle_from_id(source_id)), source_id, target, target_id)
 
     source_ability_id = line.source_id + line.event_id
     if source_ability_id in tree_model.ability_index[target_id][source_id]:
         source_ability = tree_model.ability_index[target_id][source_id][source_ability_id]
     else:
-        source_ability = tree_model.add_source_ability(row_constructor(line.event_name, '', 
-                source_ability_id), source_ability_id, ability_source, source_id, target_id, parse_duration)
-        
+        source_ability = tree_model.add_source_ability(
+                row_constructor(line.event_name, '', source_ability_id), source_ability_id,
+                ability_source, source_id, target_id, parse_duration)
+
     return source_ability, source_ability.data
 
-def get_flags(flag_str:str) -> tuple[bool]:
+
+def get_flags(flag_str: str) -> tuple[bool]:
     '''
     Returns flags from flag field of log line.
 
     Return: (critical_hit, miss, flank, kill, shield_break)
     '''
     critical_hit = 'Critical' in flag_str
     miss = 'Miss' in flag_str
     flank = 'Flank' in flag_str
     kill = 'Kill' in flag_str
     shield_break = 'ShieldBreak' in flag_str
     return (critical_hit, miss, flank, kill, shield_break)
 
+
 def calculate_damage_row_stats(raw_row_data: DamageTableRow, combat_time: float) -> tuple:
     '''
-    Calculates combat stats from raw stats taken from the parse, for example DPS from damage and combat time.
+    Calculates combat stats from raw stats taken from the parse, for example DPS from damage and
+    combat time.
 
     Parameters:
     - :param raw_row_data: contains the raw data of a row
     - :param combat_time: combat time of the parent entity in seconds
 
-    :return: complete row data according to TREE_HEADER (see __init__.py), plus a tuple containing name and 
-    handle as first element -> ((name, handle), DPS, Total Damage, ...)
+    :return: complete row data according to TREE_HEADER (see __init__.py), plus a tuple containing
+    name and handle as first element -> ((name, handle), DPS, Total Damage, ...)
     '''
-    (name, handle, total_damage, max_one_hit, kills, total_attacks, misses, crit_num, flank_num, 
-    total_shield_damage, total_hull_damage, total_base_damage, _, hull_attacks, shield_attacks) = raw_row_data
+    (name, handle, total_damage, max_one_hit, kills, total_attacks, misses, crit_num, flank_num,
+        total_shield_damage, total_hull_damage, total_base_damage, _, hull_attacks,
+        shield_attacks) = raw_row_data
     successful_attacks = hull_attacks - misses
     try:
         dps = total_damage / combat_time
         shield_dps = total_shield_damage / combat_time
         hull_dps = total_hull_damage / combat_time
         base_dps = total_base_damage / combat_time
     except ZeroDivisionError:
@@ -336,55 +353,60 @@
         accuracy = successful_attacks / hull_attacks
     except ZeroDivisionError:
         accuracy = 0.0
     try:
         flank_rate = flank_num / successful_attacks
     except ZeroDivisionError:
         flank_rate = 0.0
-    return ((name, handle), dps, total_damage, debuff, max_one_hit, crit_chance, accuracy, flank_rate,
-            kills, total_attacks, misses, crit_num, flank_num, total_shield_damage, shield_dps, 
-            total_hull_damage, hull_dps, total_base_damage, base_dps, combat_time, hull_attacks, 
-            shield_attacks)
+    return ((name, handle), dps, total_damage, debuff, max_one_hit, crit_chance, accuracy,
+            flank_rate, kills, total_attacks, misses, crit_num, flank_num, total_shield_damage,
+            shield_dps, total_hull_damage, hull_dps, total_base_damage, base_dps, combat_time,
+            hull_attacks, shield_attacks)
+
 
 def calculate_heal_row_stats(raw_row_data: HealTableRow, combat_time: float) -> tuple:
     '''
-    Calculates combat stats from raw stats taken from the parse, for example HPS from Heal and combat time.
+    Calculates combat stats from raw stats taken from the parse, for example HPS from Heal and
+    combat time.
 
     Parameters:
     - :param raw_row_data: contains the raw data of a row
     - :param combat_time: combat time of the parent entity in seconds
 
-    :return: complete row data according to HEAL_TREE_HEADER (see __init__.py), plus a tuple containing name 
-    and handle as first element -> ((name, handle), HPS, Total Heal, ...)
+    :return: complete row data according to HEAL_TREE_HEADER (see __init__.py), plus a tuple
+    containing name and handle as first element -> ((name, handle), HPS, Total Heal, ...)
     '''
-    (name, handle, total_heal, hull_heal, shield_heal, max_one_heal, heal_ticks, critical_heals, _, 
-            hull_heal_ticks, shield_heal_ticks) = raw_row_data
+    (name, handle, total_heal, hull_heal, shield_heal, max_one_heal, heal_ticks, critical_heals, _,
+        hull_heal_ticks, shield_heal_ticks) = raw_row_data
     try:
         hps = total_heal / combat_time
         shield_hps = shield_heal / combat_time
         hull_hps = hull_heal / combat_time
     except ZeroDivisionError:
         hps = 0.0
         shield_hps = 0.0
         hull_hps = 0.0
     try:
         crit_chance = critical_heals / heal_ticks
     except ZeroDivisionError:
         crit_chance = 0.0
 
-    return ((name, handle), hps, total_heal, hull_heal, hull_hps, shield_heal, shield_hps, max_one_heal, 
-            crit_chance, heal_ticks, critical_heals, combat_time, hull_heal_ticks, shield_heal_ticks)
+    return ((name, handle), hps, total_heal, hull_heal, hull_hps, shield_heal, shield_hps,
+            max_one_heal, crit_chance, heal_ticks, critical_heals, combat_time, hull_heal_ticks,
+            shield_heal_ticks)
+
 
 def combine_children_damage_stats(item: TreeItem) -> tuple:
     '''
-    Combines the stats of the children items intelligently. Absolute numbers are summed, percentages are
-    averaged.
+    Combines the stats of the children items intelligently. Absolute numbers are summed,
+    percentages are averaged.
 
     Parameters:
-    - :param item: item to retrieve children data from; item.data must be string containing the ability name
+    - :param item: item to retrieve children data from; item.data must be string containing the
+    ability name
     '''
     for index, column in enumerate(zip(*item._children)):
         if index == 0:
             if isinstance(item.data, (str, tuple)):
                 combined_data = [item.data]
             else:
                 combined_data = [(item.data.name, item.data.handle)]
@@ -395,21 +417,23 @@
             combined_data.append(max(column))
         elif index == 19:
             combined_data.append(column[0])
         else:
             combined_data.append(sum(column))
     item.data = tuple(combined_data)
 
+
 def combine_children_heal_stats(item: TreeItem) -> tuple:
     '''
-    Combines the stats of the children items intelligently. Absolute numbers are summed, percentages are
-    averaged.
+    Combines the stats of the children items intelligently. Absolute numbers are summed,
+    percentages are averaged.
 
     Parameters:
-    - :param item: item to retrieve children data from; item.data must be string containing the ability name
+    - :param item: item to retrieve children data from; item.data must be string containing the
+    ability name
     '''
     for index, column in enumerate(zip(*item._children)):
         if index == 0:
             if isinstance(item.data, (str, tuple)):
                 combined_data = [item.data]
             else:
                 combined_data = [(item.data.name, item.data.handle)]
@@ -420,20 +444,22 @@
             combined_data.append(max(column))
         elif index == 11:
             combined_data.append(column[0])
         else:
             combined_data.append(sum(column))
     item.data = tuple(combined_data)
 
+
 def merge_single_lines(tree_model: TreeModel):
     '''
-    Eliminates one level of depth if needed by merging lines that only have a single child. For example:
+    Eliminates one level of depth if needed by merging lines that only have a single child. For
+    example:
 
     v Quantum Mines
-        v Quantum Mine 34 
+        v Quantum Mine 34
             > Mine Explosion
         v Quantum Mine 25
             > Mine Explosion
 
     becomes:\n
     v Quantum Mines - Mine Explosion\n
        > Quantum Mine 34\n
@@ -443,15 +469,15 @@
     Parameters:
     - :param tree_model: tree model to analyze and improve
     '''
     for player in tree_model._player._children:
         new_pet_groups = dict()
 
         for ability_or_petgroup in player._children:
-            if ability_or_petgroup._children[0].child_count == 0:
+            if not ability_or_petgroup._children or ability_or_petgroup._children[0].child_count == 0:
                 continue
 
             for pet in reversed(ability_or_petgroup._children):
                 if pet.child_count == 1:
                     ability_name = pet._children[0].data
                     if ability_or_petgroup.data == ability_name:
                         new_pet_group_name = ability_name
@@ -472,14 +498,15 @@
 
             if ability_or_petgroup.child_count == 0:
                 ability_or_petgroup.parent._children.remove(ability_or_petgroup)
 
         for new_pet_group in new_pet_groups.values():
             player.append_child(new_pet_group)
 
+
 def complete_damage_sub_tree(item: TreeItem, combat_time):
     '''
     Recursive function merging data from the bottom up.
 
     Parameters:
     - :param item: item to complete
     '''
@@ -489,14 +516,15 @@
             child.data = calculate_damage_row_stats(child.data, combat_time)
         else:
             complete_damage_sub_tree(child, combat_time)
         graph_data.append(child.graph_data)
     combine_children_damage_stats(item)
     item.graph_data = numpy.sum(graph_data, axis=0, dtype=numpy.float64)
 
+
 def complete_heal_sub_tree(item: TreeItem, combat_time):
     '''
     Recursive function merging data from the bottom up.
 
     Parameters:
     - :param item: item to complete
     '''
@@ -506,32 +534,35 @@
             child.data = calculate_heal_row_stats(child.data, combat_time)
         else:
             complete_heal_sub_tree(child, combat_time)
         graph_data.append(child.graph_data)
     combine_children_heal_stats(item)
     item.graph_data = numpy.sum(graph_data, axis=0, dtype=numpy.float64)
 
-def complete_damage_tree(tree_model: TreeModel, combat_durations: dict):
+
+def complete_damage_tree(
+        tree_model: TreeModel, combat_durations: dict, total_combat_duration: float):
     '''
     Merges the data from the bottom up to fill all lines.
 
     Parameters:
     - :param tree_model: tree model to be completed
     - :param combat_durations: combat durations for all actors
     '''
     for actor in bundle(tree_model._player._children, tree_model._npc._children):
-        current_combat_time = combat_durations[actor.data.id[0]]
+        current_combat_time = combat_durations.get(actor.data.id[0], total_combat_duration)
         actor.data.combat_time = current_combat_time
         complete_damage_sub_tree(actor, current_combat_time)
 
-def complete_heal_tree(tree_model: TreeModel, combat_durations: dict):
+
+def complete_heal_tree(tree_model: TreeModel, combat_durations: dict, total_combat_duration: float):
     '''
     Merges the data from the bottom up to fill all lines.
 
     Parameters:
     - :param tree_model: tree model to be completed
     - :param combat_durations: combat durations for all actors
     '''
     for actor in bundle(tree_model._player._children, tree_model._npc._children):
-        current_combat_time = combat_durations[actor.data.id[0]]
+        current_combat_time = combat_durations.get(actor.data.id[0], total_combat_duration)
         actor.data.combat_time = current_combat_time
         complete_heal_sub_tree(actor, current_combat_time)
```

### Comparing `sto_oscr-2024.3b40/OSCR/utilities.py` & `sto_oscr-2024.4b20/OSCR/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 from datetime import datetime
 from re import search as re_search
 from typing import Generator, Iterable
 
-from .datamodels import LogLine
-
 PLAYER_HANDLE_REGEX = '^P\\[.+?@.+?(?P<handle>@.+?)\\]$'
 COMPUTER_HANDLE_REGEX = '^C\\[(?P<handle>\\d+).+?\\]$'
 
-def to_datetime(date_time:str) -> datetime:
+
+def to_datetime(date_time: str) -> datetime:
     '''
     returns datetime object from combatlog string containing date and time
     '''
     date_time_list = date_time.split(':')
     date_time_list += date_time_list.pop().split('.')
     date_time_list = list(map(int, date_time_list))
     date_time_list[0] += 2000
     date_time_list[6] *= 100000
     return datetime(*date_time_list)
 
-def datetime_to_str(date_time:datetime) -> str:
+
+def datetime_to_str(date_time: datetime) -> str:
     '''
     Converts datetime object to str timestamp. Truncates microseconds to tenth of seconds.
     '''
-    return (f'{str(date_time.year)[-2:]}:{date_time.month:02d}:{date_time.day:02d}:{date_time.hour:02d}:'
-            f'{date_time.minute:02d}:{date_time.second:02d}.{str(date_time.microsecond)[0]}')
+    return (f'{str(date_time.year)[-2:]}:{date_time.month:02d}:{date_time.day:02d}:'
+            f'{date_time.hour:02d}:{date_time.minute:02d}:{date_time.second:02d}.'
+            f'{str(date_time.microsecond)[0]}')
 
-def datetime_to_display(date_time:datetime) -> str:
+
+def datetime_to_display(date_time: datetime) -> str:
     '''
     Converts datetime object to formatted string.
     '''
     return (f'{date_time.year}-{date_time.month:02d}-{date_time.day:02d} {date_time.hour:02d}:'
             f'{date_time.minute:02d}:{date_time.second:02d}')
 
+
 def logline_to_str(line) -> str:
     '''
     Converts LogLine to str or returns str if argument is str.
     '''
     if isinstance(line, str):
         return line.strip() + '\n'
-    
+
     timestamp = datetime_to_str(line.timestamp)
     return f'{timestamp}::{",".join(line[1:11])},{line[11]},{line[12]}\n'
 
-def get_handle_from_id(id_str:str) -> str:
+
+def get_handle_from_id(id_str: str) -> str:
     '''
     returns player handle from is string
     '''
     if id_str.startswith('P'):
         handle = re_search(PLAYER_HANDLE_REGEX, id_str)
         if handle is None:
             return ''
@@ -76,26 +80,28 @@
     :return: (critical_hit, miss, kill)
     """
     critical_hit = "Critical" in flag_str
     miss = "Miss" in flag_str
     kill = "Kill" in flag_str
     return (critical_hit, miss, kill)
 
+
 def reversed_index(length: int) -> Generator[int, None, None]:
     '''
     Generator that yields the indices for an iterable with given length in reversed order.
 
     Parameters:
     - :param length: length of the iterable
     '''
     counter = length
     while counter > 0:
         counter -= 1
         yield counter
 
+
 def bundle(*iterables: Iterable) -> Generator:
     """
     Generator yielding the items of the given iterables in the order they were provided.
 
     Parameters:
     - :param iterables: iterables to be bundled
     """
```

### Comparing `sto_oscr-2024.3b40/LICENSE` & `sto_oscr-2024.4b20/LICENSE`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.3b40/pyproject.toml` & `sto_oscr-2024.4b20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.3b40/PKG-INFO` & `sto_oscr-2024.4b20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: STO-OSCR
-Version: 2024.3b40
+Version: 2024.4b20
 Summary: Open Source Combatlog Reader for Star Trek Online.
 Project-URL: Homepage, https://github.com/STOCD/OSCR
 Project-URL: Repository, https://github.com/STOCD/OSCR.git
 Project-URL: Bug Tracker, https://github.com/STOCD/OSCR/issues
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

