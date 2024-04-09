# Comparing `tmp/bakabakabaka-0.8.1.tar.gz` & `tmp/bakabakabaka-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakabakabaka-0.8.1.tar", last modified: Tue Apr  9 06:28:34 2024, max compression
+gzip compressed data, was "bakabakabaka-0.8.3.tar", last modified: Tue Apr  9 15:21:24 2024, max compression
```

## Comparing `bakabakabaka-0.8.1.tar` & `bakabakabaka-0.8.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:28:34.290920 bakabakabaka-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 06:28:34.290920 bakabakabaka-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    32529 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/baka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:28:34.286920 bakabakabaka-0.8.1/bakabakabaka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 06:28:34.000000 bakabakabaka-0.8.1/bakabakabaka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 06:28:34.290920 bakabakabaka-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-09 06:28:21.000000 bakabakabaka-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:21:24.775472 bakabakabaka-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 15:21:16.000000 bakabakabaka-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 15:21:24.775472 bakabakabaka-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-09 15:21:16.000000 bakabakabaka-0.8.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32912 2024-04-09 15:21:16.000000 bakabakabaka-0.8.3/baka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:21:24.775472 bakabakabaka-0.8.3/bakabakabaka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-09 15:21:24.000000 bakabakabaka-0.8.3/bakabakabaka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 15:21:24.000000 bakabakabaka-0.8.3/bakabakabaka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:21:24.000000 bakabakabaka-0.8.3/bakabakabaka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 15:21:24.000000 bakabakabaka-0.8.3/bakabakabaka.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-09 15:21:24.000000 bakabakabaka-0.8.3/bakabakabaka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:21:24.775472 bakabakabaka-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-09 15:21:16.000000 bakabakabaka-0.8.3/setup.py
```

### Comparing `bakabakabaka-0.8.1/LICENSE` & `bakabakabaka-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.1/PKG-INFO` & `bakabakabaka-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.1
+Version: 0.8.3
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bakabakabaka-0.8.1/README.md` & `bakabakabaka-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `bakabakabaka-0.8.1/baka.py` & `bakabakabaka-0.8.3/baka.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,18 @@
 import shlex
 import shutil
 import smtplib
 import socket
 import subprocess
 import sys
 import time
+import typing
 
-VERSION = "0.8.1"
-BASE_PATH = os.path.expanduser("~/.baka")
+__version__: typing.Final[str] = "0.8.3"
+BASE_PATH: typing.Final[str] = os.path.expanduser("~/.baka")
 
 
 def init_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(description="the stupid configuration tracker using the stupid content tracker",
                                      usage="%(prog)s [--dry-run] <argument>")
     parser.add_argument("--version", action="version", version=VERSION)
     maingrp = parser.add_mutually_exclusive_group()
@@ -304,26 +305,33 @@
         smtp_server_instance.starttls()
         smtp_server_instance.login(config_email["smtp_username"], config_email["smtp_password"])
         smtp_server_instance.send_message(message)
     return 0
 
 
 def main() -> int:
+    # There are three main steps to baka:
+    # 1. Generate commands to be executed based on argument
+    # 2. Execute (or print if dry-run) commands
+    # 3. Append time and arguments to history.log, also log command output if job
     if sys.flags.optimize > 0:
         print("Warning: baka does not function properly with the -O (optimize) flag", file=sys.stderr)
     # parse arguments
     parser = init_parser()
     args = parser.parse_args()
     # init config
     config = Config()
     # change cwd to repo folder
     original_cwd = os.getcwd()
     os.chdir(BASE_PATH)
-    # select commands
+    # 1. Generate commands to be executed based on argument
+    # all arguments are mutually exclusive, except for dry-run or the job modifiers
+    # no commands are ever executed and nothing is ever written outside of ~/.baka if --dry-run
     if args.hash_and_copy_files:
+        # meant for internal use only
         hash_and_copy_files(config)
         return 0
     elif args.init:
         # option to edit then reload config
         _ = input("Press enter to open your config file with nano")
         if args.dry_run:
             print(shlex.join(["nano", os.path.join(BASE_PATH, "config.json")]))
@@ -508,110 +516,112 @@
             "--format=format:%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n%C(bold white)%s%C(reset)%C(dim white) - %an%C(reset)"
         ]]
     elif args.show:
         cmds = [["git", "show", "--color-words"]]
     else:
         parser.print_usage()
         return 2
-    # execute commands
+    # 2. Execute (or print if dry-run) commands
     command_output = []
     error_message = ""
     pending_stat = False
     return_code = 0
     try:
         for cmd in cmds:
-            if args.job and "shlex_split" in config.jobs[args.job] and config.jobs[args.job]["shlex_split"]:
+            if args.job and config.jobs[args.job].get("shlex_split", False):
                 if type(cmd) == list and len(cmd) == 1:
                     cmd = cmd[0]
                 cmd = shlex.split(cmd)
             if args.dry_run:
                 print(shlex.join(cmd))
                 command_output.append("dry-run")
                 command_output.append(">>> " + shlex.join(cmd))
-            else:
-                if args.job:
-                    # run command as part of job, otherwise run command normally
-                    capture_output = bool(
-                        ("write" in config.jobs[args.job] and config.jobs[args.job]["write"]) or
-                        ("email" in config.jobs[args.job] and config.jobs[args.job]["email"] and config.jobs[args.job]["email"]["to"])
-                    )
-                    verbosity = ""
-                    if "verbosity" in config.jobs[args.job] and config.jobs[args.job]["verbosity"]:
-                        verbosity = config.jobs[args.job]["verbosity"].lower()
-                    if verbosity not in ["debug", "info", "error", "silent"]:
-                        verbosity = "debug"
-                    if verbosity in ["debug"]:
-                        print("\033[94m%s\033[0m" % shlex.join(cmd))
-                    if "interactive" in config.jobs[args.job] and config.jobs[args.job]["interactive"]:
-                        response = input("\033[92mContinue (yes/no/skip)?\033[0m ")
-                        if response.strip().lower().startswith("y"):
-                            pass
-                        elif response.strip().lower().startswith("n"):
-                            break
-                        elif response.strip().lower().startswith("s"):
-                            continue
-                        else:
-                            print("\033[91mInvalid response, exiting\033[0m")
-                            break
-                    proc_input = "y\n" if args.yes else None
-                    proc_out = subprocess.PIPE
-                    proc_err = subprocess.PIPE
-                    if not capture_output:
-                        if verbosity in ["debug", "info"]:
-                            proc_out = sys.stdout
-                        if verbosity in ["debug", "info", "error"]:
-                            proc_err = sys.stderr
-                    proc = subprocess.run(cmd, stdout=proc_out, stderr=proc_err, input=proc_input)
-                    if proc.returncode != 0:
-                        if "exit_non_zero" in config.jobs[args.job] and config.jobs[args.job]["exit_non_zero"]:
-                            return_code = proc.returncode
-                            error_message = "Error: baka job encountered a non-zero return code for `%s`, exiting" % shlex.join(cmd)
-                            command_output.append(error_message)
-                            print(error_message, file=sys.stderr)
-                            break
-                        else:
-                            return_code += 1
-                    if capture_output:
-                        if verbosity in ["debug", "info"]:
-                            sys.stdout.buffer.write(proc.stdout)
-                        if verbosity in ["debug", "info", "error"]:
-                            sys.stderr.buffer.write(proc.stderr)
-                            print("\n")
-                        command_output.append(">>> " + shlex.join(cmd))
-                        command_output.append(proc.stdout.decode().strip())
-                        command_output.append(proc.stderr.decode().strip())
-                        command_output.append("\n")
-                    elif verbosity in ["debug", "info", "error"]:
-                        print("")
-                elif args.file:
-                    # save outputs of non-copy commands as files, otherwise run command normally
-                    if cmd[0] == "BAKA_DEST":
-                        dest = cmd[1]
-                        with open(dest, "w", encoding="utf-8", errors="surrogateescape") as f:
-                            proc = subprocess.run(cmd[2:], capture_output=True, text=True)
-                            f.write(proc.stdout)
+                continue
+            # execute command if not dry-run
+            if args.job:
+                # run command as part of job, otherwise run command normally
+                capture_output = bool(
+                    ("write" in config.jobs[args.job] and config.jobs[args.job]["write"]) or
+                    ("email" in config.jobs[args.job] and config.jobs[args.job]["email"] and config.jobs[args.job]["email"]["to"])
+                )
+                verbosity = ""
+                if "verbosity" in config.jobs[args.job] and config.jobs[args.job]["verbosity"]:
+                    verbosity = config.jobs[args.job]["verbosity"].lower()
+                if verbosity not in ["debug", "info", "error", "silent"]:
+                    verbosity = "debug"
+                if verbosity in ["debug"]:
+                    print("\033[94m%s\033[0m" % shlex.join(cmd))
+                if "interactive" in config.jobs[args.job] and config.jobs[args.job]["interactive"]:
+                    response = input("\033[92mContinue (yes/no/skip)?\033[0m ")
+                    if response.strip().lower().startswith("y"):
+                        pass
+                    elif response.strip().lower().startswith("n"):
+                        break
+                    elif response.strip().lower().startswith("s"):
+                        continue
+                    else:
+                        print("\033[91mInvalid response, exiting\033[0m")
+                        break
+                proc_input = "y\n" if args.yes else None
+                proc_out = subprocess.PIPE
+                proc_err = subprocess.PIPE
+                if not capture_output:
+                    if verbosity in ["debug", "info"]:
+                        proc_out = sys.stdout
+                    if verbosity in ["debug", "info", "error"]:
+                        proc_err = sys.stderr
+                proc = subprocess.run(cmd, stdout=proc_out, stderr=proc_err, input=proc_input)
+                if proc.returncode != 0:
+                    if "exit_non_zero" in config.jobs[args.job] and config.jobs[args.job]["exit_non_zero"]:
+                        return_code = proc.returncode
+                        error_message = "Error: baka job encountered a non-zero return code for `%s`, exiting" % shlex.join(cmd)
+                        command_output.append(error_message)
+                        print(error_message, file=sys.stderr)
+                        break
                     else:
-                        proc = subprocess.run(cmd)
-                    if proc.returncode != 0 and not (cmd[0] == "git" and cmd[1] == "commit"):
                         return_code += 1
+                if capture_output:
+                    if verbosity in ["debug", "info"]:
+                        sys.stdout.buffer.write(proc.stdout)
+                    if verbosity in ["debug", "info", "error"]:
+                        sys.stderr.buffer.write(proc.stderr)
+                        print("\n")
+                    command_output.append(">>> " + shlex.join(cmd))
+                    command_output.append(proc.stdout.decode().strip())
+                    command_output.append(proc.stderr.decode().strip())
+                    command_output.append("\n")
+                elif verbosity in ["debug", "info", "error"]:
+                    print("")
+            elif args.file:
+                # save outputs of non-copy commands as files, otherwise run command normally
+                if cmd[0] == "BAKA_DEST":
+                    dest = cmd[1]
+                    with open(dest, "w", encoding="utf-8", errors="surrogateescape") as f:
+                        proc = subprocess.run(cmd[2:], capture_output=True, text=True)
+                        f.write(proc.stdout)
                 else:
-                    # run command normally
-                    if cmd == [sys.executable, os.path.abspath(__file__), "--_hash_and_copy_files"]:
-                        pending_stat = True
-                    elif pending_stat:
-                        os_stat_tracked_files(config)
-                        pending_stat = False
                     proc = subprocess.run(cmd)
-                    if proc.returncode != 0 and not (cmd[0] == "git" and cmd[1] == "commit"):
-                        return_code += 1
+                if proc.returncode != 0 and not (cmd[0] == "git" and cmd[1] == "commit"):
+                    return_code += 1
+            else:
+                # run command normally
+                if cmd == [sys.executable, os.path.abspath(__file__), "--_hash_and_copy_files"]:
+                    pending_stat = True
+                elif pending_stat:
+                    os_stat_tracked_files(config)
+                    pending_stat = False
+                proc = subprocess.run(cmd)
+                if proc.returncode != 0 and not (cmd[0] == "git" and cmd[1] == "commit"):
+                    return_code += 1
     except Exception as e:
         error_message = "Error baka line: %s For: %s %s %s" % (sys.exc_info()[2].tb_lineno, shlex.join(cmd), type(e).__name__, e.args)
         command_output.append(error_message)
         print(error_message, file=sys.stderr)
-    # write log
+    # 3. Append time and arguments to history.log, also log command output if job
+    # append to history.log
     if not (args.dry_run or args.diff or args.log or args.show):
         log_entry = time.ctime()
         for key in vars(args):
             if vars(args)[key] or (key == "remove" and args.remove is not None):
                 log_entry += " " + key + " " + str(vars(args)[key])
         if error_message:
             log_entry += " " + error_message
```

### Comparing `bakabakabaka-0.8.1/bakabakabaka.egg-info/PKG-INFO` & `bakabakabaka-0.8.3/bakabakabaka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakabakabaka
-Version: 0.8.1
+Version: 0.8.3
 Summary: the stupid configuration tracker using the stupid content tracker
 Home-page: https://github.com/elesiuta/baka
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

