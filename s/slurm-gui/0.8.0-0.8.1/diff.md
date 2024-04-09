# Comparing `tmp/slurm-gui-0.8.0.tar.gz` & `tmp/slurm-gui-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm-gui-0.8.0.tar", last modified: Mon Apr  8 07:57:39 2024, max compression
+gzip compressed data, was "slurm-gui-0.8.1.tar", last modified: Tue Apr  9 03:41:51 2024, max compression
```

## Comparing `slurm-gui-0.8.0.tar` & `slurm-gui-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:57:39.261284 slurm-gui-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 07:57:34.000000 slurm-gui-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:57:39.261284 slurm-gui-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 07:57:34.000000 slurm-gui-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:57:39.261284 slurm-gui-0.8.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23275 2024-04-08 07:57:34.000000 slurm-gui-0.8.0/bin/tsqueue
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 07:57:39.261284 slurm-gui-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-08 07:57:34.000000 slurm-gui-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 07:57:39.261284 slurm-gui-0.8.0/slurm_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 07:57:39.000000 slurm-gui-0.8.0/slurm_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 07:57:39.000000 slurm-gui-0.8.0/slurm_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:57:39.000000 slurm-gui-0.8.0/slurm_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-08 07:57:39.000000 slurm-gui-0.8.0/slurm_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 07:57:39.000000 slurm-gui-0.8.0/slurm_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:41:51.737680 slurm-gui-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 03:41:47.000000 slurm-gui-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-09 03:41:51.737680 slurm-gui-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-09 03:41:47.000000 slurm-gui-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:41:51.733680 slurm-gui-0.8.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25585 2024-04-09 03:41:47.000000 slurm-gui-0.8.1/bin/tsqueue
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 03:41:51.737680 slurm-gui-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-09 03:41:47.000000 slurm-gui-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:41:51.733680 slurm-gui-0.8.1/slurm_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-09 03:41:51.000000 slurm-gui-0.8.1/slurm_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 03:41:51.000000 slurm-gui-0.8.1/slurm_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:41:51.000000 slurm-gui-0.8.1/slurm_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 03:41:51.000000 slurm-gui-0.8.1/slurm_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:41:51.000000 slurm-gui-0.8.1/slurm_gui.egg-info/top_level.txt
```

### Comparing `slurm-gui-0.8.0/LICENSE` & `slurm-gui-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slurm-gui-0.8.0/PKG-INFO` & `slurm-gui-0.8.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.8.0
+Version: 0.8.1
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual<0.60,>=0.50
 
 # Slurm made easy with slurm-gui ! 
 
 **GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework**
 
-![PyPI](https://img.shields.io/pypi/v/slurm-gui)
+[![PyPI](https://img.shields.io/pypi/v/slurm-gui)](https://pypi.org/project/slurm-gui/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slurm-gui)
-![PyPI - License](https://img.shields.io/pypi/l/slurm-gui)
+[![GH Action PyPI](https://github.com/dirkpetersen/slurm-gui/actions/workflows/python-publish.yml/badge.svg)](https://github.com/dirkpetersen/slurm-gui/actions/workflows/python-publish.yml)
+[![PyPI - License](https://img.shields.io/pypi/l/slurm-gui)](https://github.com/dirkpetersen/slurm-gui/blob/main/LICENSE)
+
 
 Install with `python3 -m pip install slurm-gui` and then run `tsqueue` on a node with Slurm installed to get a list of slurm jobs (tsbatch and tsrun are coming...)
 
 ![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/d56d9b88-0ff4-49cf-a563-b21d4aa2d9e0)
 
 use the mouse or keys to scroll up and down and hit enter to get more details (from squeue and sstat or sacct).
 
@@ -33,7 +43,12 @@
 
 Get a long list of information. squeue info comes first but if you scroll down, you will get also all the info provided by sstat
 
 if a job is running, it will offer you to cancel it plus an error message for jobs you cannot kill
 
 ![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/8c27c8c0-8a00-47e9-be9a-1346ff2cbab5)
 
+and if you have selected one of your own jobs, you can scoll down and get lots of details, for example about the maximum memory consumption (MaxRSS) of your job:
+
+![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/8037afd5-3a18-4adb-9f39-1578ff619ec8)
+
+
```

### Comparing `slurm-gui-0.8.0/README.md` & `slurm-gui-0.8.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Slurm made easy with slurm-gui ! 
 
 **GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework**
 
-![PyPI](https://img.shields.io/pypi/v/slurm-gui)
+[![PyPI](https://img.shields.io/pypi/v/slurm-gui)](https://pypi.org/project/slurm-gui/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slurm-gui)
-![PyPI - License](https://img.shields.io/pypi/l/slurm-gui)
+[![GH Action PyPI](https://github.com/dirkpetersen/slurm-gui/actions/workflows/python-publish.yml/badge.svg)](https://github.com/dirkpetersen/slurm-gui/actions/workflows/python-publish.yml)
+[![PyPI - License](https://img.shields.io/pypi/l/slurm-gui)](https://github.com/dirkpetersen/slurm-gui/blob/main/LICENSE)
+
 
 Install with `python3 -m pip install slurm-gui` and then run `tsqueue` on a node with Slurm installed to get a list of slurm jobs (tsbatch and tsrun are coming...)
 
 ![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/d56d9b88-0ff4-49cf-a563-b21d4aa2d9e0)
 
 use the mouse or keys to scroll up and down and hit enter to get more details (from squeue and sstat or sacct).
 
@@ -18,7 +20,12 @@
 
 Get a long list of information. squeue info comes first but if you scroll down, you will get also all the info provided by sstat
 
 if a job is running, it will offer you to cancel it plus an error message for jobs you cannot kill
 
 ![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/8c27c8c0-8a00-47e9-be9a-1346ff2cbab5)
 
+and if you have selected one of your own jobs, you can scoll down and get lots of details, for example about the maximum memory consumption (MaxRSS) of your job:
+
+![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/8037afd5-3a18-4adb-9f39-1578ff619ec8)
+
+
```

### Comparing `slurm-gui-0.8.0/bin/tsqueue` & `slurm-gui-0.8.1/bin/tsqueue`

 * *Files 4% similar despite different names*

```diff
@@ -3,60 +3,106 @@
 # puts a terminal interface on slurm squeue
 # to debug install package: textual-dev and run a console in a separate shell:
 # > textual console -x SYSTEM -x EVENT -x DEBUG -x INFO
 # Then launch tsqueue in dev mode
 # > textual run --dev ~/gh/slurm-gui/bin/tsqueue
 # This will show all print statements in the console
 
-import sys, os, re, subprocess as sp, asyncio
+import sys
 if sys.version_info < (3, 8):
     print("Error: This script requires Python 3.8 or higher.")
     print(f"You are using Python {sys.version}")
     sys.exit(1)
-from typing import List, Dict, Tuple
+import os, re, subprocess as sp, asyncio, getpass, shutil
+from typing import List, Dict, Tuple # Python 3.8 compatibility
+try:
+    import textual
+except:
+    print("Error: The 'textual' package is not installed. Please install it using 'python3 -m pip install textual'")
+    sys.exit(1)
 from textual import events
 from textual.app import App, ComposeResult
 from textual.widgets import DataTable, Button, Header, Footer, Label, ProgressBar, Static, Rule
 from textual.binding import Binding
-from textual.containers import Vertical, Horizontal
+from textual.containers import Vertical, Horizontal, Center, Middle
 from textual.screen import ModalScreen
 
+if not shutil.which('squeue'):
+    print("Error: The 'squeue' command is not available. Please make sure Slurm is installed and the command is in your PATH.")
+    sys.exit(1)
+
 class TSQueue(App):
     BINDINGS = [
         ("q", "request_quit", "Quit"),
     ]
 
     def compose(self) -> ComposeResult:
-        table = DataTable()
-        table.focus()
-        table.zebra_stripes = True
-        table.cursor_type = "row"
-        table.styles.max_height = "99vh"
-        yield table
+        with Center():
+            self.data_table = DataTable()
+            self.data_table.focus()
+            self.data_table.zebra_stripes = True
+            self.data_table.cursor_type = "row"
+            self.data_table.styles.max_height = "97vh"
+            self.data_table.styles.width = "99%"
+            yield self.data_table
+            self.progress_bar = ProgressBar(
+                total=100,
+                show_bar=True,
+                show_percentage=True,
+                show_eta=False
+            )
+            yield self.progress_bar
+        yield Footer()
+        self.progress_bar.advance(20)
 
     def on_mount(self) -> None:
-        self.data_table = self.query_one(DataTable)
-        self.update_data()
+        asyncio.create_task(self.update_data())
 
-    def update_data(self) -> None:
-        columns, data = self.get_squeue_data()
+    async def update_data(self) -> None:
+        columns, data = await self.get_squeue_data()
         #print('*** columns:', columns)
-        #print('*** data:', data)
+        #print('*** data:', data)     
+        self.progress_bar.advance(20)
         self.data_table.add_columns(*columns)
+        self.progress_bar.advance(30)
         self.data_table.add_rows(data)
+        self.progress_bar.total = 100              
+        self.data_table.focus
+        self.progress_bar.remove()
 
-    def get_squeue_data(self) -> Tuple[List[str], List[List[str]]]:
+    async def get_squeue_data(self) -> Tuple[List[str], List[List[str]]]:
         squeue_format = os.getenv('SQUEUE_FORMAT', '%.18i %.4P %.12j %.8u %.2t %.10M %.10L %.3D %.3C %.9b %.4m %R')
+        squeue_format = re.sub(r'\s+', '|', squeue_format) # replace multiple spaces with a single pipe
         cmd = f'squeue --format="{squeue_format}"'
-        output = sp.check_output(cmd, shell=True, text=True)
+        process = await asyncio.create_subprocess_shell(cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE)
+        stdout, stderr = await process.communicate()        
+        output = stdout.decode().strip()
         lines = output.strip().split('\n')
-        columns = re.split(r'\s+', lines[0].strip())
-        data = [re.split(r'\s+', line.strip()) for line in lines[1:]]
+        columns = [col.strip() for col in lines[0].split('|')]
+        data = [line.split('|') for line in lines[1:]] 
+     
+        # Get the current Linux user
+        current_user = getpass.getuser()
+
+        # Move all lines where the USER column matches the current user to the top
+        user_lines = []
+        other_lines = []
+        for line in data:
+            if line[columns.index('USER')] == current_user.strip():  # strip whitespace from user name
+                user_lines.append(line)
+            else:
+                other_lines.append(line)
+        data = user_lines + other_lines
         return columns, data
-    
+
+    async def delete_row_by_job_id(self, job_id: str) -> None:
+        if self.selected_row_key is not None:
+            self.data_table.remove_row(self.selected_row_key)
+            self.selected_row_key = None    
+
     async def get_job_details(self, job_id: str) -> Dict[str, List[str]]:
 
         user = os.getlogin()  # Get the current username
         if '[' in job_id:
             job_id = job_id.split('_')[0]        
         details = {}
 
@@ -87,29 +133,32 @@
         lines = stdout.decode().strip().split('\n')
         keys = lines[0].split('|')
         values = [line.split('|') for line in lines[1:2]]
         for i, key in enumerate(keys):
             sorted_details[key] = [value[i] for value in values]
         
         #print("Job Details:")
-        # print(sorted_details)
+        #print(sorted_details)
         return sorted_details
 
     async def on_data_table_row_selected(self, event: DataTable.RowSelected) -> None:
-        job_id = self.data_table.get_row(event.row_key)[0]
+        self.selected_row_key = event.row_key    
+        job_id = self.data_table.get_row(event.row_key)[0].strip()
         details = await self.get_job_details(job_id)
         screen = JobDetailsScreen(job_id, details)
         await self.push_screen(screen)
 
     def action_request_quit(self) -> None:
         self.app.exit()
 
 class JobDetailsScreen(ModalScreen):
     BINDINGS = [
         ("q", "request_quit", "Quit"),
+        ("c", "request_cancel", "Cancel")
+
     ]    
     DEFAULT_CSS = """
     JobDetailsScreen {
         align: center middle;
     }
     JobDetailsScreen > Vertical {
         width: 90%;
@@ -147,33 +196,31 @@
         if len(job_states) > 0:
             job_state = job_states[0]
 
         with Vertical():
             # Scrollable DataTable for details
             with Horizontal():
                 yield Button("(q)uit", id="close", variant="primary")
-
-                if job_state.lower() == 'running':
-                    yield Button("Cancel Job", id="cancel_job", variant="error")
-
+                #if job_state.lower() == 'running': # Only show cancel button if job is running
+                yield Button("(c)ancel job", id="cancel_job", variant="error")
                 self.status_label = Label(f"  Details for job {self.job_id}", id="title")
                 if reason != 'None':
                     self.status_label.update(f"Job {self.job_id} is pending, reason: {self.explain_reason_code(reason)}")
                 yield self.status_label
                
             details_table = DataTable()
             details_table.focus()
             details_table.zebra_stripes = True
             details_table.cursor_type = "none"
             details_table.styles.max_height = "99vh"
             details_table.add_column("Setting", width=20)
             details_table.add_column("Value")
             for key, values in self.details.items():
                 for value in values:
-                    if value not in [None, '', 'Unknown', '(null)', 'N/A', '*', 'None', '0', '00:00:00']:
+                    if value not in [None, '', 'Unknown', '(null)', 'N/A', 'n/a',  '*', 'None', '0', '00:00:00']:
                         details_table.add_row(key, value)
             yield details_table
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         if event.button.id == "close":
             self.dismiss()
         elif event.button.id == "cancel_job":
@@ -181,24 +228,28 @@
 
     async def cancel_job(self) -> None:
         cmd = f'scancel {self.job_id}'
         process = await asyncio.create_subprocess_shell(cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE)
         stdout, stderr = await process.communicate()
 
         if process.returncode == 0:
+            await self.app.delete_row_by_job_id(self.job_id)            
             self.dismiss()
         else:
             error_message = stderr.decode().strip()
             # Display an error message or handle the cancellation failure appropriately
             self.status_label.update(f"Failed to cancel job {self.job_id}: {error_message}")
             print(f"Failed to cancel job {self.job_id}: {error_message}")    
 
     def action_request_quit(self) -> None:
         self.dismiss()
 
+    def action_request_cancel(self) -> None:
+        asyncio.create_task(self.cancel_job())
+
     def explain_reason_code(self, reason_code: str) -> str:
         reason_explanations = {
             'Resources': 'The resources for the job are not yet available. This could be due to other jobs running on the system or resource limits being reached. The job will start once the required resources become available. If this is a job array, some of your array jobs may already be running. You can check the job status using the squeue command or job management interface.',
             'DependencyNeverSatisfied': 'The job you submitted has dependencies that were never satisfied. This means that the job was waiting for other jobs to complete before it could start, but those jobs did not finish successfully. To resolve this, review the dependencies of your job and ensure that the dependent jobs are able to complete successfully. You may need to resubmit the dependent jobs or adjust their requirements.',
             'PartitionTimeLimit': 'The job exceeded the time limit set for the partition it was submitted to. Each partition has a maximum time limit, and if your job runs longer than this limit, it will be terminated. To resolve this, you can either request a partition with a longer time limit or adjust your job to complete within the given time limit. If you need more time, consider breaking your job into smaller tasks or optimizing your code.',
             'TimeLimit': 'The job exceeded the time limit specified in your job submission. You can set a time limit for your job using the --time option when submitting the job. If your job exceeds this limit, it will be terminated. To resolve this, you can either increase the time limit for your job or optimize your code to complete within the specified time limit.',            
             'NodeFail': 'The job was terminated because one or more of the nodes assigned to it failed during the execution. This could be due to hardware issues, network problems, or other system failures. If you encounter this issue, it is recommended to report it to the system administrator for further investigation. In the meantime, you can try resubmitting your job to see if it runs successfully on different nodes.',
```

### Comparing `slurm-gui-0.8.0/setup.py` & `slurm-gui-0.8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,15 +42,23 @@
     author_email="no-email@no-domain.com",
     description=appdesc,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{gitrepos}",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Topic :: System :: Distributed Computing",
+        "Topic :: Utilities",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: 3.13",
     ],
     python_requires=pyreq,
     install_requires=read_requirements(),
     scripts=myscripts,
 )
```

### Comparing `slurm-gui-0.8.0/slurm_gui.egg-info/PKG-INFO` & `slurm-gui-0.8.1/slurm_gui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: slurm-gui
-Version: 0.8.0
+Version: 0.8.1
 Summary: GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework
 Home-page: https://github.com/dirkpetersen/slurm-gui
 Author: Dirk Petersen
 Author-email: no-email@no-domain.com
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Topic :: System :: Distributed Computing
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: textual<0.60,>=0.50
 
 # Slurm made easy with slurm-gui ! 
 
 **GUI/TUI frontends to squeue, sbatch and srun using the fabulous textual TUI framework**
 
-![PyPI](https://img.shields.io/pypi/v/slurm-gui)
+[![PyPI](https://img.shields.io/pypi/v/slurm-gui)](https://pypi.org/project/slurm-gui/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/slurm-gui)
-![PyPI - License](https://img.shields.io/pypi/l/slurm-gui)
+[![GH Action PyPI](https://github.com/dirkpetersen/slurm-gui/actions/workflows/python-publish.yml/badge.svg)](https://github.com/dirkpetersen/slurm-gui/actions/workflows/python-publish.yml)
+[![PyPI - License](https://img.shields.io/pypi/l/slurm-gui)](https://github.com/dirkpetersen/slurm-gui/blob/main/LICENSE)
+
 
 Install with `python3 -m pip install slurm-gui` and then run `tsqueue` on a node with Slurm installed to get a list of slurm jobs (tsbatch and tsrun are coming...)
 
 ![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/d56d9b88-0ff4-49cf-a563-b21d4aa2d9e0)
 
 use the mouse or keys to scroll up and down and hit enter to get more details (from squeue and sstat or sacct).
 
@@ -33,7 +43,12 @@
 
 Get a long list of information. squeue info comes first but if you scroll down, you will get also all the info provided by sstat
 
 if a job is running, it will offer you to cancel it plus an error message for jobs you cannot kill
 
 ![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/8c27c8c0-8a00-47e9-be9a-1346ff2cbab5)
 
+and if you have selected one of your own jobs, you can scoll down and get lots of details, for example about the maximum memory consumption (MaxRSS) of your job:
+
+![image](https://github.com/dirkpetersen/slurm-gui/assets/1427719/8037afd5-3a18-4adb-9f39-1578ff619ec8)
+
+
```

