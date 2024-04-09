# Comparing `tmp/cosmix_launcher-1.0.0.tar.gz` & `tmp/cosmix_launcher-1.0.1.tar.gz`

## Comparing `cosmix_launcher-1.0.0.tar` & `cosmix_launcher-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/license.txt
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/requirements.txt
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/scripts/test.sh
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     4869 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/net.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/.gitignore
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/readme.md
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/license.txt
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/scripts/test.sh
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/.gitignore
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/readme.md
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.1/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.0/license.txt` & `cosmix_launcher-1.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.0/src/cosmix/__main__.py` & `cosmix_launcher-1.0.1/src/cosmix/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from . import api
 from .api.instance import Instance
 from .api import paths
 from .api import logger
 from .api import net
 from .api import versions
+from .api import config
+from typing import Optional
 import sys
 import click
 import os
 import send2trash
 import shutil
 
 
@@ -33,20 +35,23 @@
     logger.info("  Cosmic Reach: " + versions.get_latest_of("reach"))
     logger.info("  Cosmic Quilt: " + versions.get_latest_of("quilt"))
 
 
 @cosmix.command()
 @click.option("--version", "-v", default="latest", type=str, help="The version of Cosmic Reach to use. Defaults to 'latest'")
 @click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to use.")
+@click.option("--display-name", "-n", default=None, type=str, help="An optional display name to use for the instance.")
 @click.argument("name")
-def add(version: str, quilt_version: str, name: str):
+def add(version: str, quilt_version: str, display_name: Optional[str], name: str):
     if Instance.exists(name):
         logger.error("Instance already exists.")
         exit(1)
-    Instance.make_instance(name, version, None if quilt_version == "none" else quilt_version).download()
+    instance = Instance.make_instance(name, version, None if quilt_version == "none" else quilt_version)
+    instance.display_name = display_name
+    instance.download()
     logger.info("Made instance " + name)
 
 
 @cosmix.command()
 @click.option("--version", "-v", default="none", type=str, help="The version of Cosmic Reach to update to. Defaults to 'none'")
 @click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to update to. Defaults to 'none'")
 @click.argument("name")
@@ -61,28 +66,29 @@
     instance.save()
     instance.download(is_updating = True)
 
     logger.info("Updated instance " + name)
 
 
 @cosmix.command()
+@click.option("--args", "-a", default="none", type=str, help="A list of JVM args to pass to Cosmic Reach when launched.")
 @click.argument("name")
-def launch(name: str):
-    Instance.from_config_file(name).launch()
+def launch(args: str, name: str):
+    Instance.from_config_file(name).launch(args.split())
 
 
 @cosmix.command()
 def instances():
     if not os.path.exists(paths.INSTANCES) or len(os.listdir(paths.INSTANCES)) <= 0:
         logger.error("No instances found.")
         exit(0)
 
     for instance_name in os.listdir(paths.INSTANCES):
         instance = Instance.get_or_throw(instance_name)
-        s = f" - {instance.name} ({instance.version})"
+        s = f" - {instance.display_name} ({instance.version})"
         if instance.quilt_version is not None:
             s += f" (Quilt: {instance.quilt_version})"
         print(s)
 
 
 @cosmix.command()
 @click.argument("name")
@@ -91,14 +97,15 @@
     send2trash.send2trash(instance.path)
 
 
 @cosmix.command()
 @click.argument("name")
 def info(name: str):
     i = Instance.get_or_throw(name)
+    print(i.display_name + ":")
     print("Instance: " + i.name + (" (modded)" if i.is_modded() else ""))
     print("Path:     " + i.path.replace(os.path.expanduser("~"), "~", 1))
     print("Version:  " + i.version)
     if i.is_modded():
         print("Quilt:    " + i.quilt_version)
         mods = i.get_mods()
         if (l := len(mods)) > 0:
@@ -112,28 +119,29 @@
 @click.argument("mod", type=click.Path(exists = True))
 def add_mod(name: str, mod):
     i = Instance.get_or_throw(name)
     if not i.is_modded():
         logger.error("Instance is not modded")
         exit(1)
 
-    os.makedirs(i.path + "/mods/", exist_ok = True)
-    shutil.copyfile(mod, i.path + "/mods/" + mod.split("/")[-1])
+    path = os.path.join(i.path, "mods/")
+    os.makedirs(path, exist_ok = True)
+    shutil.copyfile(mod, os.path.join(path, mod.split("/")[-1]))
 
 
 @cosmix.command("add-crm1-mod")
 @click.argument("name")
-@click.argument("repo")
 @click.argument("mod")
-def add_crm1_mod(name: str, repo: str, mod: str):
+def add_crm1_mod(name: str, mod: str):
     i = Instance.get_or_throw(name)
 
     if not i.is_modded():
         logger.error("Instance is not modded")
         exit(1)
 
-    os.makedirs(i.path + "/mods/", exist_ok = True)
-    net.download_crm1_mod(repo, mod, i.path + "/mods/")
+    path = os.path.join(i.path, "mods/")
+    os.makedirs(path, exist_ok = True)
+    net.download_crm1_mod(mod, path)
 
 
 if __name__ == "__main__":
     cosmix()
```

### Comparing `cosmix_launcher-1.0.0/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.1/src/cosmix/api/instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,39 +26,48 @@
     "-classpath",
     "./deps/*",
     "org.quiltmc.loader.impl.launch.knot.KnotClient"
 ]
 
 
 class Instance:
-    def __init__(self, instance_name: str, cosmic_reach_version: str, args: list[str], quilt_version: Optional[str] = None):
+    def __init__(
+        self,
+        instance_name: str,
+        cosmic_reach_version: str,
+        args: list[str],
+        quilt_version: Optional[str] = None,
+        display_name: Optional[str] = None
+    ):
         self.name = instance_name
         self.version = cosmic_reach_version
         self.args = args
         self.quilt_version = quilt_version
+        self.display_name = instance_name if display_name is None else display_name
         self.path = os.path.join(paths.INSTANCES, self.name)
 
     def is_modded(self) -> bool:
         return self.quilt_version is not None
 
     def path_to(self, path: str) -> str:
         return os.path.join(self.path, path)
 
-    def launch(self):
+    def launch(self, launch_args: Optional[list[str]] = None):
         os.chdir(self.path)
 
         args = ["java"]
         if not self.is_modded():
             args.extend(["-jar", paths.path_to_cr(self.version)])
         else:
             args.append("-Dloader.gameJarPath=" + paths.path_to_cr(self.version))
             args.extend(COSMIC_QUILT_ARGS)
         args.extend(self.args)
+        args.extend(launch_args)
 
-        logger.info(f"Launching \"{self.name}\" with args {args} in folder {self.path}")
+        logger.info(f"Launching \"{self.display_name}\" ({self.name}) with args {args} in folder {self.path}")
         os.execvp("java", args)
 
     def download(self, is_updating: bool = False):
         cr_path = paths.path_to_cr(self.version)
         if not os.path.isfile(cr_path):
             net.download(f"{COSMIC_ARCHIVE_RAW_URL}/Cosmic Reach-{self.version}.jar", cr_path)
 
@@ -103,14 +112,16 @@
         if data is None:
             logger.error(f"Failed to load config at {path}")
             exit(1)
 
         ins = Instance(data["name"], data["version"], data["args"])
         if "quilt-version" in data:
             ins.quilt_version = data["quilt-version"]
+        if "display-name" in data:
+            ins.display_name = data["display-name"]
 
         return ins
 
     @staticmethod
     def make_instance(instance_name: str, cosmic_reach_version: str, quilt_version: Optional[str] = None) -> "Instance":
         if not VALID_INSTANCE_NAME.match(instance_name):
             logger.error("Instance name must match `[a-zA-Z0-9_-]*`")
@@ -127,18 +138,20 @@
         return instance
 
     @staticmethod
     def get_hjson(instance: "Instance") -> dict:
         d = {
             "name": instance.name,
             "version": instance.version,
-            "args": instance.args
+            "args": instance.args,
         }
         if instance.is_modded():
             d["quilt-version"] = instance.quilt_version
+        if instance.display_name != instance.name:
+            d["display-name"] = instance.display_name
         return d
 
     @staticmethod
     def exists(instance_name: str) -> bool:
         return os.path.exists(os.path.join(paths.INSTANCES, instance_name))
 
     @staticmethod
```

### Comparing `cosmix_launcher-1.0.0/src/cosmix/api/logger.py` & `cosmix_launcher-1.0.1/src/cosmix/api/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,66 @@
+from . import config
 import getpass
 import os
 
 
 __all__ = (
-    "COLORIZE",
     "LEVELS",
-    "SANATIZED_USERNAME",
-    "SANATIZATION_MODE"
     "sanatize_username",
     "log",
     "error",
     "warn",
     "info",
     "debug",
 )
 
 
-COLORIZE = True
 LEVELS = {
-    "error": "\u001b[33m",
+    "error": "\u001b[31m",
     "warn":  "\u001b[33m",
     "info":  "\u001b[36m",
     "debug": "\u001b[34m",
 }
 
-# https://www.youtube.com/watch?v=dQw4w9WgXcQ
-SANITIZED_USERNAME = "dQw4w9WgXcQ"
-# "sanatize" - Replace username with SANATIZED_USERNAME
-# "replace" - Replace path to home with ~
-# "none" - No sanatization
-SANATIZATION_MODE = "replace"
+_sanatize_mode = _sanatize_username = _colored_logs = None
+
 
 # Sadly there is no easy way for me to sanatize logging from the game's process because
 # the Python process is replaced with the Java one when CR is launched.
 def sanitize_username(string: str | list[str]) -> str:
-    if SANATIZATION_MODE == "none":
+    global _sanatize_mode, _sanatize_username
+
+    if _sanatize_mode is None:
+        _sanatize_mode = config.get_config()["logging"]["sanatize_mode"]
+
+    if _sanatize_mode == "none":
         return string
 
     if type(string) == list:
         return [sanatize_username(s) for s in string]
 
-    if SANATIZATION_MODE == "sanatize":
+    if _sanatize_mode == "sanatize":
+        if _sanatize_username is None:
+            _sanatize_username = config.get_config()["logging"]["sanatize_username"]
+
         replace = getpass.getuser()
-        replace_with = SANITIZED_USERNAME
-    elif SANATIZATION_MODE == "replace":
+        replace_with = _sanatize_username
+    elif _sanatize_mode == "replace":
         replace = os.path.expanduser("~")
         replace_with = "~"
 
     return string.replace(replace, replace_with)
 
 
 def log(text: str, level: str):
-    if COLORIZE:
-        print(sanitize_username(f"[{LEVELS[level]}{level}\u001b[0m]: {text}"))
-    else:
-        print(sanitize_username(f"[{level}]: {text}"))
+    global _colored_logs
+    if _colored_logs is None:
+        _colored_logs = config.get_config()["logging"]["colored_logs"]
+
+    level_text = (LEVELS[level] + level + "\u001b[0m") if _colored_logs else level
+    print(f"[{level_text}]: {text}")
 
 
 def error(text: str): log(text, "error")
 def warn(text: str):  log(text, "warn")
 def info(text: str):  log(text, "info")
 def debug(text: str): log(text, "debug")
```

### Comparing `cosmix_launcher-1.0.0/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.1/src/cosmix/api/maven.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,64 +10,65 @@
 
 
 QUILT_POM = """\
 <?xml version="1.0" encoding="UTF-8"?>
 <project
     xmlns="http://maven.apache.org/POM/4.0.0"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
-    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
-  <modelVersion>4.0.0</modelVersion>
-
-  <groupId>com.foo</groupId>
-  <artifactId>bar</artifactId>
-  <version>0.0.1-SNAPSHOT</version>
-
-  <repositories>
-    <repository>
-      <id>jitpack</id>
-      <name>Jitpack</name>
-      <url>https://jitpack.io</url>
-    </repository>
-    <repository>
-      <id>quilt</id>
-      <name>Quilt</name>
-      <url>https://maven.quiltmc.org/repository/release/</url>
-    </repository>
-    <repository>
-      <id>fabric</id>
-      <name>Fabric</name>
-      <url>https://maven.fabricmc.net/</url>
-    </repository>
-    <repository>
-      <id>sponge</id>
-      <name>Sponge</name>
-      <url>https://repo.spongepowered.org/maven/</url>
-    </repository>
-  </repositories>
-
-  <dependencies>
-    <dependency>
-      <groupId>org.codeberg.CRModders</groupId>
-      <artifactId>cosmic-quilt</artifactId>
-      <version>%s</version>
-    </dependency>
-  </dependencies>
-
-  <build>
-    <directory>lib</directory>
-    <plugins>
-      <plugin>
-        <groupId>org.apache.maven.plugins</groupId>
-        <artifactId>maven-dependency-plugin</artifactId>
-        <configuration>
-          <excludeGroupIds>finalforeach</excludeGroupIds>
-        </configuration>
-      </plugin>
-    </plugins>
-  </build>
+    xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd"
+>
+    <modelVersion>4.0.0</modelVersion>
+
+    <groupId>com.foo</groupId>
+    <artifactId>bar</artifactId>
+    <version>0.0.1-SNAPSHOT</version>
+
+    <repositories>
+        <repository>
+            <id>jitpack</id>
+            <name>Jitpack</name>
+            <url>https://jitpack.io</url>
+        </repository>
+        <repository>
+            <id>quilt</id>
+            <name>Quilt</name>
+            <url>https://maven.quiltmc.org/repository/release/</url>
+        </repository>
+        <repository>
+            <id>fabric</id>
+            <name>Fabric</name>
+            <url>https://maven.fabricmc.net/</url>
+        </repository>
+        <repository>
+            <id>sponge</id>
+            <name>Sponge</name>
+            <url>https://repo.spongepowered.org/maven/</url>
+        </repository>
+    </repositories>
+
+    <dependencies>
+        <dependency>
+            <groupId>org.codeberg.CRModders</groupId>
+            <artifactId>cosmic-quilt</artifactId>
+            <version>%s</version>
+        </dependency>
+    </dependencies>
+
+    <build>
+        <directory>lib</directory>
+        <plugins>
+            <plugin>
+                <groupId>org.apache.maven.plugins</groupId>
+                <artifactId>maven-dependency-plugin</artifactId>
+                <configuration>
+                    <excludeGroupIds>finalforeach</excludeGroupIds>
+                </configuration>
+            </plugin>
+        </plugins>
+    </build>
 </project>
 """
 
 
 def copy_deps(of: str, dest: str):
     old = os.getcwd()
     os.chdir(of)
```

### Comparing `cosmix_launcher-1.0.0/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.1/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.0/src/cosmix/api/net.py` & `cosmix_launcher-1.0.1/src/cosmix/api/net.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from . import logger
+from . import config
 import requests
 import tqdm
 import os
 import crm1
 
 
 __all__ = (
@@ -41,18 +42,23 @@
     return requests.get(url).text
 
 
 def get_json(url: str) -> dict:
     return requests.get(url).json()
 
 
-def download_crm1_mod(repo: str, mod: str, dest_folder: str):
-    # TODO: When/if https://github.com/CRModders/CRM-1/pull/3 is pulled the get_all_repos call should not be required.
-    pool = crm1.make_pool(crm1.autorepotools.get_all_repos())
-    pool.add_repository(repo)
+def download_crm1_mod(mod: str, dest_folder: str):
+    pool = crm1.make_pool()
+
+    for repo in config.get_config()["crm1"]["default_repos"]:
+        pool.add_repository(repo)
+
+    if config.get_config()["crm1"]["use_autorepo_mapping"]:
+        for mapping in crm1.autorepotools.get_all_repos():
+            pool.add_repository(mapping)
 
     mod = pool.get_mod(mod)
 
     if mod is None:
         logger.error(f"Failed to find mod '{mod}' in repo '{repo}'")
         return
```

### Comparing `cosmix_launcher-1.0.0/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.1/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.0/pyproject.toml` & `cosmix_launcher-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmix_launcher-1.0.0/readme.md` & `cosmix_launcher-1.0.1/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,103 @@
 # Cosmix
 
 A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt.
 
 ## Installation
 
 ```sh
-git clone https://codeberg.org/emmathemartian/cosmix && cd cosmix
+# Install from PyPI (recommended)
+python3 -m pip install cosmix-launcher
 
+# Install from source
+git clone https://codeberg.org/emmathemartian/cosmix && cd cosmix
 python3 -m pip install -r requirements.txt
 python3 -m build
 python3 -m pip install ./dist/*.whl
 
+# Test to make sure it's downloaded
 python3 -m cosmix version
 ```
 
 I recommend making an alias to `python3 -m cosmix`. In Zsh you can do this by adding the following to your `.zshrc`:
 ```zsh
 alias cosmix="python3 -m cosmix"
 ```
 
 **Arch Linux:**
 > Arch Linux and it's derivatives may complain with this `error: externally-managed-environment`
 >
-> To get around this, use `python3 -m pip install --user --break-system-packages ./dist/*.whl`
+> To get around this, use the `--user --break-system-packages` options with `pip install`
 >
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
 You may also need to install Maven. On Arch Linux this is just `pacman -S maven`.
 
 ## Usage
 
 ```
 cosmix version
     prints the current installed cosmix version
 
 cosmix debug
     prints a lot of debug information related to cosmix
 
-cosmix add [name]
+cosmix add [instance]
     adds and downloads a new instance
     options:
     --version -v VERSION        specify a Cosmic Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
 
-cosmix update [name]
+cosmix update [instance]
     updates an existing version
     options:
     --version -v VERSION        specify a Cosimc Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
 
 cosmix instances
     lists all instances
 
-cosmix launch [name]
+cosmix launch [instance]
     launches an instance
 
-cosmix info [name]
+cosmix info [instance]
     prints info about an instance
 
 cosmix add-mod [instance] [path to mod jar]
     adds a mod jar to an instance
 
-cosmix add-crm1-mod [instance] [CRM-1 repo] [mod id]
-    adds a mod to an instance via CRM-1
+cosmix add-crm1-mod [instance] [mod id]
+    adds a mod to an instance via CRM-1. To add repos, see ~/.local/share/cosmix/config.hjson
 
-cosmix trash [name]
+cosmix trash [instance]
     moves an instance to the system's trash folder
 ```
 
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
     cosmix add vanilla
 # Create a Cosmic Quilt instance named `my-quilt` on the latest CR version with Cosmic Quilt 1.2.7
     cosmix add my-quilt --quilt-version 1.2.7
 # Create a vanilla instance named `old-version` on CR 0.0.1
     cosmix add old-version -v 0.0.1
 # Install the latest version of Flux API available on JoJoJux's autorepo to the instance `test`
-    cosmix add-crm1-mod test https://crm-repo.jojojux.de/repo.hjson dev.crmodders.flux
+    cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
     cosmix update latest -v latest -q latest
 ```
 
 ## Folder Structure
 
 Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `APPDATA` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
     deps/
         cosmic-reach/
-            JARs for each downloaded Cosmic Reach version.
+            Contains JARs for each downloaded Cosmic Reach version.
     instances/
-        Folders containing each downloaded instance.
+        example-instance/
+            config.json  - Configs for the instance.
+    config.hjson - Configs for Cosmix
 ```
```

### Comparing `cosmix_launcher-1.0.0/PKG-INFO` & `cosmix_launcher-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.0
+Version: 1.0.1
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -13,97 +13,103 @@
 # Cosmix
 
 A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt.
 
 ## Installation
 
 ```sh
-git clone https://codeberg.org/emmathemartian/cosmix && cd cosmix
+# Install from PyPI (recommended)
+python3 -m pip install cosmix-launcher
 
+# Install from source
+git clone https://codeberg.org/emmathemartian/cosmix && cd cosmix
 python3 -m pip install -r requirements.txt
 python3 -m build
 python3 -m pip install ./dist/*.whl
 
+# Test to make sure it's downloaded
 python3 -m cosmix version
 ```
 
 I recommend making an alias to `python3 -m cosmix`. In Zsh you can do this by adding the following to your `.zshrc`:
 ```zsh
 alias cosmix="python3 -m cosmix"
 ```
 
 **Arch Linux:**
 > Arch Linux and it's derivatives may complain with this `error: externally-managed-environment`
 >
-> To get around this, use `python3 -m pip install --user --break-system-packages ./dist/*.whl`
+> To get around this, use the `--user --break-system-packages` options with `pip install`
 >
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
 You may also need to install Maven. On Arch Linux this is just `pacman -S maven`.
 
 ## Usage
 
 ```
 cosmix version
     prints the current installed cosmix version
 
 cosmix debug
     prints a lot of debug information related to cosmix
 
-cosmix add [name]
+cosmix add [instance]
     adds and downloads a new instance
     options:
     --version -v VERSION        specify a Cosmic Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
 
-cosmix update [name]
+cosmix update [instance]
     updates an existing version
     options:
     --version -v VERSION        specify a Cosimc Reach version to use. defaults to "latest"
     --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
 
 cosmix instances
     lists all instances
 
-cosmix launch [name]
+cosmix launch [instance]
     launches an instance
 
-cosmix info [name]
+cosmix info [instance]
     prints info about an instance
 
 cosmix add-mod [instance] [path to mod jar]
     adds a mod jar to an instance
 
-cosmix add-crm1-mod [instance] [CRM-1 repo] [mod id]
-    adds a mod to an instance via CRM-1
+cosmix add-crm1-mod [instance] [mod id]
+    adds a mod to an instance via CRM-1. To add repos, see ~/.local/share/cosmix/config.hjson
 
-cosmix trash [name]
+cosmix trash [instance]
     moves an instance to the system's trash folder
 ```
 
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
     cosmix add vanilla
 # Create a Cosmic Quilt instance named `my-quilt` on the latest CR version with Cosmic Quilt 1.2.7
     cosmix add my-quilt --quilt-version 1.2.7
 # Create a vanilla instance named `old-version` on CR 0.0.1
     cosmix add old-version -v 0.0.1
 # Install the latest version of Flux API available on JoJoJux's autorepo to the instance `test`
-    cosmix add-crm1-mod test https://crm-repo.jojojux.de/repo.hjson dev.crmodders.flux
+    cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
     cosmix update latest -v latest -q latest
 ```
 
 ## Folder Structure
 
 Cosmix stores all of its data in your `XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `APPDATA` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
     deps/
         cosmic-reach/
-            JARs for each downloaded Cosmic Reach version.
+            Contains JARs for each downloaded Cosmic Reach version.
     instances/
-        Folders containing each downloaded instance.
+        example-instance/
+            config.json  - Configs for the instance.
+    config.hjson - Configs for Cosmix
 ```
```

