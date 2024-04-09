# Comparing `tmp/karabiner-config-helpers-0.0.1.tar.gz` & `tmp/karabiner-config-helpers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karabiner-config-helpers-0.0.1.tar", last modified: Sat Mar  2 19:48:38 2024, max compression
+gzip compressed data, was "karabiner-config-helpers-0.0.2.tar", last modified: Tue Apr  9 19:23:48 2024, max compression
```

## Comparing `karabiner-config-helpers-0.0.1.tar` & `karabiner-config-helpers-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-02 19:48:38.314371 karabiner-config-helpers-0.0.1/
--rw-r--r--   0 user      (1000) user      (1000)       18 2024-03-02 19:19:53.000000 karabiner-config-helpers-0.0.1/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)      623 2024-03-02 19:48:38.314371 karabiner-config-helpers-0.0.1/PKG-INFO
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-02 19:48:38.314371 karabiner-config-helpers-0.0.1/bin/
--rwxr-xr-x   0 user      (1000) user      (1000)     2803 2024-03-02 19:21:35.000000 karabiner-config-helpers-0.0.1/bin/karabiner-rules
--rwxr-xr-x   0 user      (1000) user      (1000)     3301 2024-03-02 19:28:12.000000 karabiner-config-helpers-0.0.1/bin/karabiner-type
--rw-r--r--   0 user      (1000) user      (1000)       85 2024-03-02 19:06:18.000000 karabiner-config-helpers-0.0.1/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      814 2024-03-02 19:48:38.314371 karabiner-config-helpers-0.0.1/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-02 19:48:38.311038 karabiner-config-helpers-0.0.1/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-02 19:48:38.314371 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/
--rw-r--r--   0 user      (1000) user      (1000)      670 2024-03-02 19:26:44.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2979 2024-03-02 19:04:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/keyboard_base.py
--rw-r--r--   0 user      (1000) user      (1000)     2414 2024-03-02 19:04:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/keyboard_us.py
--rwxr-xr-x   0 user      (1000) user      (1000)     5562 2024-03-02 19:04:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/rules.py
--rwxr-xr-x   0 user      (1000) user      (1000)     3546 2024-03-02 19:26:21.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/type_utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-03-02 19:48:38.314371 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      623 2024-03-02 19:48:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      495 2024-03-02 19:48:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-03-02 19:48:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       25 2024-03-02 19:48:38.000000 karabiner-config-helpers-0.0.1/src/karabiner_config_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-09 19:23:48.416657 karabiner-config-helpers-0.0.2/
+-rw-r--r--   0 user      (1000) user      (1000)       18 2024-03-02 19:19:53.000000 karabiner-config-helpers-0.0.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)      623 2024-04-09 19:23:48.416657 karabiner-config-helpers-0.0.2/PKG-INFO
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-09 19:23:48.416657 karabiner-config-helpers-0.0.2/bin/
+-rwxr-xr-x   0 user      (1000) user      (1000)     3154 2024-03-31 17:53:34.000000 karabiner-config-helpers-0.0.2/bin/karabiner-rules
+-rwxr-xr-x   0 user      (1000) user      (1000)     2280 2024-04-01 11:23:11.000000 karabiner-config-helpers-0.0.2/bin/karabiner-type
+-rw-r--r--   0 user      (1000) user      (1000)       85 2024-03-02 19:06:18.000000 karabiner-config-helpers-0.0.2/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      814 2024-04-09 19:23:48.419990 karabiner-config-helpers-0.0.2/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-09 19:23:48.416657 karabiner-config-helpers-0.0.2/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-09 19:23:48.416657 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/
+-rw-r--r--   0 user      (1000) user      (1000)      874 2024-04-01 10:58:49.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     4546 2024-04-09 19:14:38.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/app_layouts.py
+-rw-r--r--   0 user      (1000) user      (1000)     3592 2024-04-09 18:16:26.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/keyboard_base.py
+-rw-r--r--   0 user      (1000) user      (1000)     1999 2024-04-09 18:17:17.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/keyboard_de.py
+-rw-r--r--   0 user      (1000) user      (1000)     2475 2024-04-09 18:17:56.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/keyboard_us.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     6671 2024-03-31 17:49:38.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/rules.py
+-rw-r--r--   0 user      (1000) user      (1000)     1211 2024-03-02 20:27:43.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/script_utils.py
+-rwxr-xr-x   0 user      (1000) user      (1000)     4872 2024-04-01 11:27:38.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/type_utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-09 19:23:48.416657 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      623 2024-04-09 19:23:48.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      628 2024-04-09 19:23:48.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-09 19:23:48.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       25 2024-04-09 19:23:48.000000 karabiner-config-helpers-0.0.2/src/karabiner_config_helpers.egg-info/top_level.txt
```

### Comparing `karabiner-config-helpers-0.0.1/PKG-INFO` & `karabiner-config-helpers-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karabiner-config-helpers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful functions and tools for custom karabiner element rules.
 Home-page: https://gitlab.com/six-two/karabiner-config
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `karabiner-config-helpers-0.0.1/bin/karabiner-rules` & `karabiner-config-helpers-0.0.2/bin/karabiner-rules`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import argparse
 import json
 import sys
 # local
+from karabiner_config_helpers import KarabinerConfigFileError
 from karabiner_config_helpers.rules import load_config, store_config, replace_or_insert_rule, sort_rules, delete_rule_by_description, delete_rule_by_name, debug_main, CONFIG_PATH
 
 
 if __name__ == "__main__":
     ap = argparse.ArgumentParser(description="Reads a complex modification JSON from stdin and insert it into the targeted profile. If a rule with the same description already exists, it will be replaced")
     ap.add_argument("-p", "--profile", default="Default profile", help="the profile to modify")
     sp = ap.add_subparsers(dest="cmd")
@@ -21,45 +22,48 @@
     remove_parser = sp.add_parser("remove", description="remove a rule")
     remove_selector_group = remove_parser.add_mutually_exclusive_group()
     remove_selector_group.add_argument("-d", "--description", help="delete all rules with this description")
     remove_selector_group.add_argument("-i", "--id", help="remove the rule with this it (without the # character)")
 
     args = ap.parse_args()
 
+    try:
+        config_json = load_config(CONFIG_PATH)
 
-    config_json = load_config(CONFIG_PATH)
-
-    if not args.cmd:
-        ap.print_help()
-        exit(1)
-    elif args.cmd == "insert":
-        try:
-            new_rule_json = load_config(args.file) if args.file else json.load(sys.stdin)
-        except Exception as ex:
-            print("Failed to parse new rule's JSON:", ex)
-
-        if "description" not in new_rule_json:
-            print("The following JSON (for the new rule to insert) is missing a top level 'description' attribute:")
-            json.dump(new_rule_json, indent=4)
-            sys.exit(1)
-
-        replace_or_insert_rule(config_json, args.profile, new_rule_json)
-    elif args.cmd == "sort":
-        sort_rules(config_json, args.profile)
-    elif args.cmd == "debug":
-        debug_main(config_json, args.profile)
-    elif args.cmd == "remove":
-        if args.description != None:
-            delete_rule_by_description(config_json, args.profile, args.description)
-        elif args.id:
-            delete_rule_by_name(config_json, args.profile, "#"+args.id)
+        if not args.cmd:
+            ap.print_help()
+            exit(1)
+        elif args.cmd == "insert":
+            try:
+                new_rule_json = load_config(args.file) if args.file else json.load(sys.stdin)
+            except Exception as ex:
+                print("Failed to parse new rule's JSON:", ex)
+
+            if "description" not in new_rule_json:
+                print("The following JSON (for the new rule to insert) is missing a top level 'description' attribute:")
+                json.dump(new_rule_json, indent=4)
+                sys.exit(1)
+
+            replace_or_insert_rule(config_json, args.profile, new_rule_json)
+        elif args.cmd == "sort":
+            sort_rules(config_json, args.profile)
+        elif args.cmd == "debug":
+            debug_main(config_json, args.profile)
+        elif args.cmd == "remove":
+            if args.description != None:
+                delete_rule_by_description(config_json, args.profile, args.description)
+            elif args.id:
+                delete_rule_by_name(config_json, args.profile, "#"+args.id)
+            else:
+                print("Rule needs to be selected by id (like #NAME) or description")
         else:
-            print("Rule needs to be selected by id (like #NAME) or description")
-    else:
-        print(f"[!] Unknown command: {args.cmd}")
-        ap.print_usage()
-        exit(1)
-
-    store_config(config_json)
+            print(f"[!] Unknown command: {args.cmd}")
+            ap.print_usage()
+            exit(1)
+
+        store_config(config_json)
+    except KarabinerConfigFileError as e:
+        print(f"[!] Could not parse karabiner config file {CONFIG_PATH} due to the following error:")
+        print(e)
```

### Comparing `karabiner-config-helpers-0.0.1/bin/karabiner-type` & `karabiner-config-helpers-0.0.2/bin/karabiner-type`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 #!/usr/bin/env python3
 import argparse
 import json
 import string
 import sys
 # local
-from karabiner_config_helpers import get_resolver
+from karabiner_config_helpers import get_resolver, helper_default_argument_parser_action_handler
 from karabiner_config_helpers.type_utils import type_text_main
-from karabiner_config_helpers.rules import helper_insert_rule_into_config
+from karabiner_config_helpers.app_layouts import load_app_resolver_map_json
+
+
+def generate_config_json(args) -> dict:
+    if args.stdin:
+        string_to_type = sys.stdin.read()
+    elif args.test:
+        string_to_type = string.printable
+    else:
+        string_to_type = args.type
+
+    keybinding_list = list(sorted([x.lower() for x in args.keybindings]))
+    app_resolver_map = load_app_resolver_map_json()
+    if args.description != None:
+        description = args.description
+    else:
+        description = f"-1 | #{','.join(keybinding_list)} | {' or '.join(keybinding_list)} -> Type the string '{string_to_type}'"
+        if args.back:
+            description += f" and go back {args.back} characters"
+
+    return type_text_main(string_to_type, description, args.back, keybinding_list, app_resolver_map)
 
 
 if __name__ == "__main__":
     default_layout = "us_mac"
 
     ap = argparse.ArgumentParser()
     input_group = ap.add_mutually_exclusive_group(required=True)
     input_group.add_argument("--stdin", action="store_true", help="read input from standard input stream, so that you can pipe it into this program without needing to worry about escaping")
     input_group.add_argument("--type", metavar="TEXT_TO_TYPE", help="this is the string that should be typed")
     input_group.add_argument("--test", action="store_true", help="replace string_to_type with all printable ASCII characters")  
 
     ap.add_argument("keybindings", nargs="+", help="what key combinations need to be pressed to type the text. Format: <modifier1>+<modifier2...>+<key>. If you specify multiple, only one of them needs to be pressed (example: 'right_command+right_meta+t', 'button4')")
-    ap.add_argument("--resolver", default=default_layout, help=f"the name of the resolver/keyboard layout (Default: {default_layout})")
-    ap.add_argument("--parallels-resolver", default=None, help="the resolver to use if Parallels Desktop is receiving the keys. Defaults to using the value specified with --resolver")
     ap.add_argument("-b", "--back", type=int, default=0, help="move the cursor backwards by X characters, so that it is within the just typed text (default: 0)")
     ap.add_argument("-d", "--description", help="use this value as a description instead of automatically generating one")
-    ap.add_argument("--print", action="store_true", help="instead of inserting the rule just print it to stdout")
-    args = ap.parse_args()
-
-    if args.stdin:
-        string_to_type = sys.stdin.read()
-    elif args.test:
-        string_to_type = string.printable
-    else:
-        string_to_type = args.type
 
-    try:
-        keybinding_list = list(sorted([x.lower() for x in args.keybindings]))
-        default_resolver = get_resolver(args.resolver)
-        parallels_resolver = get_resolver(args.parallels_resolver) if args.parallels_resolver else None
-        if args.description != None:
-            description = args.description
-        else:
-            if parallels_resolver:
-                description = f"-1 | #{','.join(keybinding_list)} | {' or '.join(keybinding_list)} -> Type the string '{string_to_type}'. Host layout: {default_resolver.layout_name}. Parallels layout: {parallels_resolver.layout_name}"
-            else:
-                description = f"-1 | #{','.join(keybinding_list)} | {' or '.join(keybinding_list)} -> Type the string '{string_to_type}'. Layout: {default_resolver.layout_name}"
-            if args.back:
-                description += f" and go back {args.back} characters"
-
-        full_json = type_text_main(string_to_type, description, args.back, keybinding_list, default_resolver, parallels_resolver)
-        if args.print:
-            json.dump(full_json, sys.stdout, indent=4)
-        else:
-            helper_insert_rule_into_config(full_json)
-    except NoResolverWithName as e:
-        print("[!]", e)
-        exit(1)
+    helper_default_argument_parser_action_handler(ap, generate_config_json)
```

### Comparing `karabiner-config-helpers-0.0.1/setup.cfg` & `karabiner-config-helpers-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = karabiner-config-helpers
-version = 0.0.1
+version = 0.0.2
 author = six-two
 author_email = pip@six-two.dev
 description = Useful functions and tools for custom karabiner element rules.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/six-two/karabiner-config
 license = MIT License
```

### Comparing `karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/__init__.py` & `karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+class KarabinerConfigFileError(Exception):
+    pass
+
+
 # Import everything that someone else may want to use
 from .keyboard_base import KeyResolver, NoKeyMappingFoundError, CharRequiresMultipleKeys
 from .keyboard_us import RESOLVER_US_MAC, RESOLVER_US_LINUX
+from .keyboard_de import RESOLVER_DE_LINUX
 from .rules import helper_insert_rule_into_config
+from .script_utils import helper_default_argument_parser_action_handler
 
 
 _RESOLVERS: dict[str,KeyResolver] = {
     "us_mac": RESOLVER_US_MAC,
     "us_linux": RESOLVER_US_LINUX,
+    "de_linux": RESOLVER_DE_LINUX,
 }
 
 class NoResolverWithName(Exception):
     pass
 
 def get_resolver(name: str) -> KeyResolver:
     if result := _RESOLVERS.get(name):
```

### Comparing `karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/keyboard_base.py` & `karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/keyboard_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any
+from enum import Enum
 
 ####### Convenience functions for better readability #############
 
 def normal(key):
    return {"key_code": key}
 
 def shift(key):
@@ -24,25 +25,45 @@
    def __init__(self, character: str) -> None:
       super().__init__(f"Can not type character '{character}' ({hex(ord(character))})")
 
 
 class CharRequiresMultipleKeys(Exception):
    pass
 
+
+class OperatingSystem(Enum):
+    LINUX = 1
+    MAC = 2
+    WINDOWS = 3
+
+
 class KeyResolver:
     """
     Resolve characters to the keystrokes that are required for them.
     Might return multiple keystrokes if that is required.
     If the key can not be typed a NoKeyMappingFoundError will be thrown.
     """
 
-    def __init__(self, layout_name: str,  *list_of_lookup_tables: dict) -> None:
+    def __init__(self, layout_name: str, os: OperatingSystem, *list_of_lookup_tables: dict) -> None:
         self.layout_name = layout_name
+        self.os = os
         self._list_of_lookup_tables = list_of_lookup_tables
 
+    def get_default_modifier_for_os(self) -> str:
+        """
+        Returns the default modifier for key bindings like copy, paste, select all, etc.
+        Command on MacOS, Control on Linux and Windows
+        """
+        if self.os == OperatingSystem.MAC:
+            return "command"
+        elif self.os in [OperatingSystem.LINUX, OperatingSystem.WINDOWS]:
+            return "control"
+        else:
+            raise Exception(f"Unknown operating system: {self.os}")
+
     def get_to_keys_for_char(self, character: str) -> list[dict[str,Any]]:
         """
         Maps a character to the keystrokes needed to type it. You can directly put the result into the "to" field of a manipulator.
         """
         if len(character) != 1:
             raise Exception(f"String '{character}' should have length 1")
```

### Comparing `karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/keyboard_us.py` & `karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/keyboard_us.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import string
 # local
 from . import KeyResolver
-from .keyboard_base import normal, shift, option, alt_gr, shift_alt_gr
+from .keyboard_base import normal, shift, option, alt_gr, shift_alt_gr, OperatingSystem
 
 KEYMAP_LETTERS_NUMBERS_UNMODIFIED = {}
 for character in string.ascii_lowercase + string.digits:
     KEYMAP_LETTERS_NUMBERS_UNMODIFIED[character] = normal(character)
 for character in string.ascii_uppercase:
     KEYMAP_LETTERS_NUMBERS_UNMODIFIED[character] = shift(character.lower())
 
@@ -76,10 +76,10 @@
     "ö": alt_gr("o"),
     "Ö": shift_alt_gr("o"),
     "ü": alt_gr("u"),
     "Ü": shift_alt_gr("u"),
     "ß": alt_gr("s"),
 }
 
-RESOLVER_US_MAC = KeyResolver("US (Mac)", KEYMAP_LETTERS_NUMBERS_UNMODIFIED, KEYMAP_SPECIAL_US_LAYOUT, KEYMAP_MAC_UMLAUTS)
-RESOLVER_US_LINUX = KeyResolver("US (Linux, de_se_fi)", KEYMAP_LETTERS_NUMBERS_UNMODIFIED, KEYMAP_SPECIAL_US_LAYOUT, KEYMAP_LINUX_US_DE_SE_FI_UMLAUTS)
+RESOLVER_US_MAC = KeyResolver("US (Mac)", OperatingSystem.MAC, KEYMAP_LETTERS_NUMBERS_UNMODIFIED, KEYMAP_SPECIAL_US_LAYOUT, KEYMAP_MAC_UMLAUTS)
+RESOLVER_US_LINUX = KeyResolver("US (Linux, de_se_fi)", OperatingSystem.LINUX, KEYMAP_LETTERS_NUMBERS_UNMODIFIED, KEYMAP_SPECIAL_US_LAYOUT, KEYMAP_LINUX_US_DE_SE_FI_UMLAUTS)
```

### Comparing `karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/rules.py` & `karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 import json
 import re
 import os
 from typing import Optional, Any
+# local
+from . import KarabinerConfigFileError
 
 # General expected rule description:
 # [PRIORITY] [#NAME] [DESCRIPTION]
 # PRIORITY needs to be at the beginning of the line, the rest is your choice. You can also insert separators between elements to make them visually stand out. Example:
 # "+50 | #MOD-FN | fn -> left_control"
 
 # PRIORITY controls in which order rules are executed
@@ -38,19 +40,31 @@
     if match := NAME_REGEX.search(description):
         return match.group(1)
     else:
         return None
 
 
 def get_rules_of_profile(config_json: dict, target_profile: str) -> list[dict]:
-    for profile in config_json["profiles"]:
-        if profile["name"] == target_profile:
-            return profile["complex_modifications"]["rules"]
+    profile_list = config_json.get("profiles")
+    if profile_list:
+        for index, profile in enumerate(profile_list):
+            name = profile.get("name")
+            if name:
+                if name == target_profile:
+                    result = profile.get("complex_modifications", {}).get("rules")
+                    if type(result) == list:
+                        return result
+                    else:
+                        raise KarabinerConfigFileError(f"Expected a list as value of 'profiles[{index}].complex_modifications.rules' in karabiner configuration file")
+            else:
+                raise KarabinerConfigFileError(f"Expected non-empty key 'profiles[{index}].name' in karabiner configuration file")
 
-    return []
+        raise KarabinerConfigFileError(f"Found not profile with the name '{target_profile}' in karabiner configuration file")
+    else:
+        raise KarabinerConfigFileError("Expected non-empty key 'profiles' in karabiner configuration file")
 
 
 def debug_main(config_json: dict, target_profile: str) -> None:
     for rule_json in get_rules_of_profile(config_json, target_profile):
         description = rule_json.get("description", "")
         print("\n", f'"{description}"')
         prio = get_rule_priority_from_description(rule_json)
@@ -64,20 +78,25 @@
     # We use the index to guarantee that the sorting is stable
     rules_with_weights = [(-get_rule_priority_from_description(rule_json), index, rule_json) for index, rule_json in enumerate(rule_json_list)]
     rules_with_weights.sort()
     return [rule_json for _, _, rule_json in rules_with_weights]
 
 
 def sort_rules(config_json: dict, target_profile: str) -> None:
-    for profile in config_json["profiles"]:
-        if profile["name"] == target_profile:
-            unsorted_rules = profile["complex_modifications"]["rules"]
-            sorted_rules = stable_sort_rules_by_priority(unsorted_rules)
-            profile["complex_modifications"]["rules"] = sorted_rules
-            return
+    # Lets try it this way, so that we do not need to implement the error handling twice:
+    rules = get_rules_of_profile(config_json, target_profile)
+    sorted_rules = stable_sort_rules_by_priority(rules)
+    rules[:] = sorted_rules
+
+    # for profile in config_json["profiles"]:
+    #     if profile["name"] == target_profile:
+    #         unsorted_rules = profile["complex_modifications"]["rules"]
+    #         sorted_rules = stable_sort_rules_by_priority(unsorted_rules)
+    #         profile["complex_modifications"]["rules"] = sorted_rules
+    #         return
 
 
 def replace_or_insert_rule(config_json: dict, target_profile: str, new_rule_json: dict) -> None:
     new_name = get_rule_name_from_description(new_rule_json)
     # IMPORTANT CHECK: If you remove it, all rules without names will be removed if you add a rule without a name :/
     if new_name:
         delete_rule_by_name(config_json, target_profile, new_name)
```

### Comparing `karabiner-config-helpers-0.0.1/src/karabiner_config_helpers/type_utils.py` & `karabiner-config-helpers-0.0.2/src/karabiner_config_helpers/type_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 import sys
 from typing import Optional, Union
 # local
+from . import get_resolver
 from .keyboard_base import KeyResolver, NoKeyMappingFoundError, shift, normal
+from .app_layouts import AppResolverMap
 
 def string_to_keymap_json(string_to_type: str, move_cursor_backwards: int, key_resolver: KeyResolver) -> list[dict]:
     list_of_keystrokes: list[dict] = []
     for character in string_to_type:
         try:
             list_of_keystrokes += key_resolver.get_to_keys_for_char(character)
         except NoKeyMappingFoundError as ex:
@@ -21,14 +23,17 @@
         raise Exception(f"Cursor backwards count can not be a negative number, but is {move_cursor_backwards}")
     elif move_cursor_backwards > 0:
         list_of_keystrokes += [normal("left_arrow")] * move_cursor_backwards
     return list_of_keystrokes
 
 
 def create_manipulators(string_to_type: str, move_cursor_backwards: int, from_key: str, from_modifiers: list[str], key_resolver: KeyResolver, parallels_key_resolver: Optional[KeyResolver]) -> list[dict]:
+    """
+    DEPRECATED, because it does not handle multiple layouts for multiple different applications. Use create_manipulators_for_all_layouts(...) instead
+    """
     from_dict: dict[str,Union[list,dict,str]] = {
         "modifiers": {
             "mandatory": from_modifiers,
             "optional": [
                 "caps_lock"
             ]
         }
@@ -72,21 +77,53 @@
             {
                 "type": "basic",
             "from": from_dict,
             "to": string_to_keymap_json(string_to_type, move_cursor_backwards, key_resolver)
           }
         ]
 
-def type_text_main(string_to_type: str, description: str, move_cursor_backwards: int, from_key_combos: list[str], key_resolver: KeyResolver, parallels_key_resolver: Optional[KeyResolver]) -> dict:
+def create_manipulators_for_all_layouts(string_to_type: str, move_cursor_backwards: int, from_key: str, from_modifiers: list[str], app_resolver_map: AppResolverMap) -> list[dict]:
+    from_dict: dict[str,Union[list,dict,str]] = {
+        "modifiers": {
+            "mandatory": from_modifiers,
+            "optional": [
+                "caps_lock"
+            ]
+        }
+    }
+    if from_key.startswith("button"):
+        # This is a mouse button, use the correct key
+        from_dict = {
+            "pointing_button": from_key
+        }
+    else:
+        # Will probably be a normal key
+        from_dict["key_code"] = from_key
+
+    manipulators = []
+    for resolver_name, condition_list in app_resolver_map.get_resolver_names_and_conditions():
+        key_resolver = get_resolver(resolver_name)
+        manipulators.append({
+            "description": f"Type text in {resolver_name} layout",
+            "type": "basic",
+            "from": from_dict,
+            "to": string_to_keymap_json(string_to_type, move_cursor_backwards, key_resolver),
+            "conditions": condition_list,
+        })
+    
+    return manipulators
+
+
+def type_text_main(string_to_type: str, description: str, move_cursor_backwards: int, from_key_combos: list[str], app_resolver_map: AppResolverMap) -> dict:
     manipulators = []
 
     for key_combo in from_key_combos:
         parts = key_combo.split("+")
         from_key = parts[-1]
         from_modifiers = parts[:-1]
-        manipulators += create_manipulators(string_to_type, move_cursor_backwards, from_key, from_modifiers, key_resolver, parallels_key_resolver)
+        manipulators += create_manipulators_for_all_layouts(string_to_type, move_cursor_backwards, from_key, from_modifiers, app_resolver_map)
 
     return {
         "description": description,
         "manipulators": manipulators,
     }
```

### Comparing `karabiner-config-helpers-0.0.1/src/karabiner_config_helpers.egg-info/PKG-INFO` & `karabiner-config-helpers-0.0.2/src/karabiner_config_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karabiner-config-helpers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Useful functions and tools for custom karabiner element rules.
 Home-page: https://gitlab.com/six-two/karabiner-config
 Author: six-two
 Author-email: pip@six-two.dev
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

