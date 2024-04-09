# Comparing `tmp/python_sysinformer-1.2.5.tar.gz` & `tmp/python_sysinformer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sysinformer-1.2.5.tar", max compression
+gzip compressed data, was "python_sysinformer-1.3.0.tar", max compression
```

## Comparing `python_sysinformer-1.2.5.tar` & `python_sysinformer-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-08-21 22:18:33.402691 python_sysinformer-1.2.5/LICENSE
--rw-r--r--   0        0        0     5690 2023-08-21 22:18:33.402691 python_sysinformer-1.2.5/README.md
--rw-r--r--   0        0        0     1529 2023-08-21 22:19:05.331196 python_sysinformer-1.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/config/__init__.py
--rw-r--r--   0        0        0     1102 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/config/config_parser.py
--rw-r--r--   0        0        0      221 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/config/constants.py
--rw-r--r--   0        0        0     1225 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/config/default_config.py
--rw-r--r--   0        0        0        0 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/__init__.py
--rw-r--r--   0        0        0     4349 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/containers.py
--rw-r--r--   0        0        0     5012 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/cpu.py
--rw-r--r--   0        0        0     2041 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/disks.py
--rw-r--r--   0        0        0     3745 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/latency.py
--rw-r--r--   0        0        0     2721 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/memory.py
--rw-r--r--   0        0        0     2604 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/networking.py
--rw-r--r--   0        0        0     2764 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/processes.py
--rw-r--r--   0        0        0     2605 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/services.py
--rw-r--r--   0        0        0     2851 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/core/system.py
--rw-r--r--   0        0        0     3974 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/main.py
--rw-r--r--   0        0        0        0 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/utilities/__init__.py
--rw-r--r--   0        0        0      442 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/utilities/exceptions.py
--rw-r--r--   0        0        0      560 2023-08-21 22:18:33.406691 python_sysinformer-1.2.5/src/utilities/utils.py
--rw-r--r--   0        0        0     6277 1970-01-01 00:00:00.000000 python_sysinformer-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 06:33:11.325074 python_sysinformer-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5296 2024-04-09 06:33:11.325074 python_sysinformer-1.3.0/README.md
+-rw-r--r--   0        0        0     1593 2024-04-09 06:33:38.345000 python_sysinformer-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/config/__init__.py
+-rw-r--r--   0        0        0     1102 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/config/config_parser.py
+-rw-r--r--   0        0        0     1233 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/config/default_config.py
+-rw-r--r--   0        0        0      221 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/constants.py
+-rw-r--r--   0        0        0        0 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/containers.py
+-rw-r--r--   0        0        0     5666 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/cpu.py
+-rw-r--r--   0        0        0     2041 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/disks.py
+-rw-r--r--   0        0        0     3745 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/latency.py
+-rw-r--r--   0        0        0     2739 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/memory.py
+-rw-r--r--   0        0        0     2597 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/networking.py
+-rw-r--r--   0        0        0     2764 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/processes.py
+-rw-r--r--   0        0        0     2605 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/services.py
+-rw-r--r--   0        0        0     4035 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/core/system.py
+-rw-r--r--   0        0        0     3985 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/utilities/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/utilities/exceptions.py
+-rw-r--r--   0        0        0      560 2024-04-09 06:33:11.329074 python_sysinformer-1.3.0/src/utilities/utils.py
+-rw-r--r--   0        0        0     6016 1970-01-01 00:00:00.000000 python_sysinformer-1.3.0/PKG-INFO
```

### Comparing `python_sysinformer-1.2.5/LICENSE` & `python_sysinformer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/README.md` & `python_sysinformer-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -77,28 +77,14 @@
 
 The most basic usage to retrieve all information is:
 
 ```bash
 psi run -a
 ```
 
-If you prefer to only retrieve specific information, you can use the following flags:
-
-
-```bash
-Usage: psi config [OPTIONS]
-
-  The config command is used to create a default config file.
-
-Options:
-  --create            Creates a new configuration file
-  --config-path TEXT  The path to the config file (default: ~/.config/psi/config.yaml)
-  --help              Show this message and exit.
-```
-
 If you prefer to only retrieve specific information, you can use the following options:
 
 ```bash
 Options:
   -a, --all           Show all information
   -s, --system        Show only system information
   -c, --cpu           Show only CPU information
```

### Comparing `python_sysinformer-1.2.5/pyproject.toml` & `python_sysinformer-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "python-SysInformer"
-version = "1.2.5"
+version = "1.3.0"
 description = "A simple system information tool for Linux"
 authors = ["Timothy Bryant <timothybryant3@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src", from = "."}]
 # classifiers = ["Private :: Do not Upload"]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.9"
 distro = "^1.8.0"
 netifaces = "^0.11.0"
 psutil = "^5.9.5"
 tabulate = "^0.9.0"
 ping3 = "^4.0.4"
 pyyaml = "^6.0.1"
+click = "^8.1.7"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
-sourcery = "^1.0.9"
 pytest = "^7.2.2"
 black = "^23.3.0"
 pre-commit = "^3.3.3"
 pytest-mock = "^3.11.1"
 coverage = "^7.2.7"
 isort = "^5.12.0"
+sourcery = "^1.11.0"
 
 [tool.poetry.group.tooling.dependencies]
 pip-tools = "^7.1.0"
 doit = "^0.36.0"
 python-semantic-release = "^8.0.7"
 
 [build-system]
@@ -43,33 +44,34 @@
 [tool.poetry.scripts]
 psi = "src.main:cli"
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = [
     "build",
     "chore",
-    "ci",
-    "docs",
-    "feat",
+    "refactor",
     "fix",
     "perf",
     "style",
-    "refactor",
+    "docs",
+    "ci",
     "test",
+    "feat",
     ":boom:",
+    "BREAKING_CHANGE",
 ]
-major_tags = [":boom:"]
+major_tags = [":boom:", "BREAKING_CHANGE"]
 minor_tags = ["feat"]
 patch_tags = ["fix", "perf", "style", "docs", "ci", "test"]
 
 [tool.semantic_release]
 version_toml = [
     "pyproject.toml:tool.poetry.version",
 ]
 branch = "main"
 changelog_file = "CHANGELOG.md"
 build_command = "poetry build"
 dist_path = "dist/"
-upload_to_release = true
+upload_to_vcs_release = true
 upload_to_pypi = false
 remove_dist = false
 patch_without_tag = true
```

### Comparing `python_sysinformer-1.2.5/src/config/config_parser.py` & `python_sysinformer-1.3.0/src/config/config_parser.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/src/config/default_config.py` & `python_sysinformer-1.3.0/src/config/default_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 
 import yaml
 
 
 def write_default_config(config_path=None) -> None:
-    # Use the default path if none provided
     if config_path is None:
         config_dir = os.path.join(os.path.expanduser("~"), ".config", "psi")
         config_path = os.path.join(config_dir, "config.yaml")
+    else:
+        config_dir = os.path.dirname(config_path)
 
-        # Ensure the directory exists
-        os.makedirs(config_dir, exist_ok=True)
+    # Ensure the directory exists
+    os.makedirs(config_dir, exist_ok=True)
 
     # Default configuration
     default_config = {
         "services": [
             {"name": "FTP Server", "port": 21, "host": "localhost"},
             {"name": "SSH", "port": 22, "host": "localhost"},
             {"name": "HTTP", "port": 80, "host": "localhost"},
```

### Comparing `python_sysinformer-1.2.5/src/core/containers.py` & `python_sysinformer-1.3.0/src/core/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,20 +113,22 @@
 def print_running_containers() -> None:
     """
     Prints the running Docker or Podman containers on the system.
     """
     print_title("Container Information")
     if container_tool := check_docker_or_podman():
         containers = get_running_containers(container_tool)
-        if containers is not None:
+        if containers == []:
+            print(f"No {container_tool} containers are running on your system.")
+        elif containers:
             print(f"{container_tool.capitalize()} containers running on your system:")
             print(
                 tabulate(
                     containers,
-                    headers=["ID", "Names", "PortMappings", "Status"],
+                    headers=["ID", "Name", "PortMappings", "Status"],
                     tablefmt="simple_grid",
                 )
             )
         else:
             print("Error retrieving running containers.")
     else:
         print("Neither Docker nor Podman is installed on your system.")
```

### Comparing `python_sysinformer-1.2.5/src/core/cpu.py` & `python_sysinformer-1.3.0/src/core/cpu.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 import os
 import platform
 from typing import Literal, Union
+import subprocess
 
 import psutil
 
 from src.utilities.utils import print_bold_kv, print_title
 
 
 def get_cpu_cache_and_bogomips() -> tuple[str, str]:
     """
-    Tries to get cpu_cache and cpu_bogomips from /proc/cpuinfo and
-    if it fails, then return 'UNKNOWN'.
+    Tries to get cpu_cache from sysctl command on macOS and cpu_bogomips from /proc/cpuinfo on Linux,
+    if it fails, then return a clear message indicating the status.
 
     Returns:
-    tuple: A tuple containing cpu_cache and cpu_bogomips.
+    tuple: A tuple containing cpu_cache and a message for cpu_bogomips.
     """
-    try:
-        with open("/proc/cpuinfo", encoding="UTF-8", mode="r") as f:
-            cpuinfo = f.readlines()
+    cpu_cache = "UNKNOWN"
+    cpu_bogomips = "N/A (No macOS Equivalent)"
 
-        cpu_cache = next(
-            line.split(": ")[1].strip()
-            for line in cpuinfo
-            if line.startswith("cache size")
-        )
-        cpu_bogomips = next(
-            line.split(": ")[1].strip()
-            for line in cpuinfo
-            if line.startswith("bogomips")
-        )
+    os_type = platform.system()
+    if os_type == "Linux":
+        try:
+            with open("/proc/cpuinfo", encoding="UTF-8", mode="r") as f:
+                cpuinfo = f.readlines()
+
+            cpu_cache = next(
+                line.split(": ")[1].strip()
+                for line in cpuinfo
+                if line.startswith("cache size")
+            )
+            cpu_bogomips = next(
+                line.split(": ")[1].strip()
+                for line in cpuinfo
+                if line.startswith("bogomips")
+            )
+        except (IOError, StopIteration):
+            cpu_cache = "UNKNOWN"
+            cpu_bogomips = "UNKNOWN"
+    elif os_type == "Darwin":  # Darwin is the system name for macOS
+        try:
+            # Retrieve the L2 cache size
+            result = subprocess.run(
+                ["sysctl", "-n", "hw.l2cachesize"], capture_output=True, check=True, text=True
+            )
+            if result.returncode == 0 and result.stdout:
+                cpu_cache = f"{int(result.stdout.strip()) // 1024} KB"
+        except subprocess.SubprocessError:
+            cpu_cache = "UNKNOWN"
 
-        return cpu_cache, cpu_bogomips
-    except IOError:
-        # print(f"Error reading CPU cache size and bogomips: {exception}")
-        return "UNKNOWN", "UNKNOWN"
-    except Exception:
-        # print(f"Error reading CPU cache size and bogomips: {exception}")
-        return "UNKNOWN", "UNKNOWN"
+    return cpu_cache, cpu_bogomips
 
 
 def get_cpu_info() -> tuple[int, str, Union[float, Literal["Unknown"]], str, str]:
     """
     Gets CPU information.
 
     Returns:
@@ -116,15 +129,15 @@
     if os_type != "Linux":
         return (
             f"Temperature check only supported on Linux. Current OS: {os_type}",
             False,
         )
 
     try:
-        temps = psutil.sensors_temperatures()
+        temps = psutil.sensors_temperatures() # type: ignore
         if "coretemp" in temps:
             cputemp = temps["coretemp"]
             for item in cputemp:
                 if item.label == "Package id 0":
                     return f"{item.current}°C", True
         return "Unable to get system temperature.", False
     except psutil.Error:
@@ -134,25 +147,27 @@
         return "Unable to get system temperature.", False
 
 
 def print_cpu_info() -> None:
     """
     Prints the CPU information, CPU usage, load average, and system temperature.
     """
+    os_type = platform.system()
     cpu_nb, cpu_info, cpu_freq, cpu_cache, cpu_bogomips = get_cpu_info()
     print_title("CPU Information")
     print_bold_kv("Number", str(cpu_nb))
     print_bold_kv("Model", cpu_info)
     print_bold_kv("Frequency", f"{cpu_freq} MHz")
     print_bold_kv("Cache L2", cpu_cache)
     print_bold_kv("Bogomips", cpu_bogomips)
     print_bold_kv("CPU Usage", f"{get_cpu_usage()}%")
 
-    cpu_temp, _ = get_system_temperature()  # replaced status with _
-    print_bold_kv("CPU Temperature", cpu_temp)
+    if os_type == "Linux":
+        cpu_temp, _ = get_system_temperature()
+        print_bold_kv("CPU Temperature", cpu_temp)
 
     process_count = get_process_count()
     print_bold_kv("Process Count", f"{process_count}")
 
     load_1, load_5, load_15 = get_load_average()
     print_bold_kv("Load average (1m)", f"{round(load_1, 2)}")
     print_bold_kv("Load average (5m)", f"{round(load_5, 2)}")
```

### Comparing `python_sysinformer-1.2.5/src/core/disks.py` & `python_sysinformer-1.3.0/src/core/disks.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/src/core/latency.py` & `python_sysinformer-1.3.0/src/core/latency.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/src/core/memory.py` & `python_sysinformer-1.3.0/src/core/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Returns:
         tuple: containing total memory, free memory, memory usage percentage,
                total swap, free swap, swap usage percentage
     """
     try:
         mem_info = {
             i.split()[0].rstrip(":"): int(i.split()[1])
-            for i in open("/proc/meminfo").readlines()
+            for i in open("/proc/meminfo", encoding="UTF-8").readlines()
         }
     except (FileNotFoundError, PermissionError):
         # print(f"Error reading file '/proc/meminfo': {exception}")
         return (0, 0, 0, 0, 0, 0)
 
     keys = ["MemTotal", "MemFree", "Buffers", "Cached", "SwapTotal", "SwapFree"]
     if any(key not in mem_info for key in keys):
```

### Comparing `python_sysinformer-1.2.5/src/core/networking.py` & `python_sysinformer-1.3.0/src/core/networking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import urllib.request
 
 import netifaces
 import psutil
 from tabulate import tabulate
 
-from src.config.constants import GET_WAN_IP
+from src.constants import GET_WAN_IP
 from src.utilities.utils import print_title
 
 
 def get_network_info() -> tuple[dict[str, str], tuple[str, str]]:
     """
     Gets LAN and WAN network information of the system.
```

### Comparing `python_sysinformer-1.2.5/src/core/processes.py` & `python_sysinformer-1.3.0/src/core/processes.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/src/core/services.py` & `python_sysinformer-1.3.0/src/core/services.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/src/main.py` & `python_sysinformer-1.3.0/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 import time
 
 import click
 
-from src.config.constants import CONFIG_PATH_DEFAULT
+from src.constants import CONFIG_PATH_DEFAULT
 from src.config.default_config import write_default_config
 from src.core.containers import print_running_containers
 from src.core.cpu import print_cpu_info
 from src.core.disks import print_disk_info
 from src.core.latency import print_latency_info
 from src.core.memory import print_memory_info
 from src.core.networking import print_network_info
@@ -24,22 +24,22 @@
     "disk": lambda _: print_disk_info(),
     "network": lambda config: (print_network_info(), print_latency_info(config)),
     "processes": lambda config: print_process_info(config),
     "containers": lambda _: print_running_containers(),
 }
 
 
-def check_os() -> None:
-    """Checks if the OS is supported."""
-    current_os = platform.system()
-    if current_os in ("Windows", "Darwin"):
-        print_title_red(
-            f"{current_os} OS is not fully supported yet. Results may vary."
-        )
-        time.sleep(2)
+# def check_os() -> None:
+#     """Checks if the OS is supported."""
+#     current_os = platform.system()
+#     if current_os in ("Windows", "Darwin"):
+#         print_title_red(
+#             f"{current_os} OS is not fully supported yet. Results may vary."
+#         )
+#         time.sleep(2)
 
 
 # The main group for the CLI
 @click.group()
 def cli():
     """System information tool."""
 
@@ -78,15 +78,15 @@
 
 
 @cli.command(name="config")
 @click.option("--create", is_flag=True, help="Creates a new configuration file")
 @click.option(
     "--config-path",
     default=CONFIG_PATH_DEFAULT,
-    help="The path to the config file (default: ~/.config/p/confsiig.yaml)",
+    help="The path to the config file (default: ~/.config/psi/config.yaml)",
 )
 def create_config(create, config_path):
     """The config command is used to create a default config file."""
     try:
         if create:
             write_default_config(config_path)
         else:
@@ -100,15 +100,15 @@
 def print_all_info(config_path: str) -> None:
     """
     Prints all system-related information.
 
     Args:
         config_file (str): The path to the config file.
     """
-    check_os()
+    # check_os()
     print_system_info()
     print_cpu_info()
     print_cpu_usage_info()
     print_memory_info()
     print_memory_usage_info()
     print_disk_info()
     print_network_info()
```

### Comparing `python_sysinformer-1.2.5/src/utilities/utils.py` & `python_sysinformer-1.3.0/src/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.2.5/PKG-INFO` & `python_sysinformer-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: python-sysinformer
-Version: 1.2.5
+Version: 1.3.0
 Summary: A simple system information tool for Linux
 Author: Timothy Bryant
 Author-email: timothybryant3@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: distro (>=1.8.0,<2.0.0)
 Requires-Dist: netifaces (>=0.11.0,<0.12.0)
 Requires-Dist: ping3 (>=4.0.4,<5.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
@@ -94,28 +97,14 @@
 
 The most basic usage to retrieve all information is:
 
 ```bash
 psi run -a
 ```
 
-If you prefer to only retrieve specific information, you can use the following flags:
-
-
-```bash
-Usage: psi config [OPTIONS]
-
-  The config command is used to create a default config file.
-
-Options:
-  --create            Creates a new configuration file
-  --config-path TEXT  The path to the config file (default: ~/.config/psi/config.yaml)
-  --help              Show this message and exit.
-```
-
 If you prefer to only retrieve specific information, you can use the following options:
 
 ```bash
 Options:
   -a, --all           Show all information
   -s, --system        Show only system information
   -c, --cpu           Show only CPU information
```

