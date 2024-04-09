# Comparing `tmp/yo-1.5.0.tar.gz` & `tmp/yo-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yo-1.5.0.tar", last modified: Mon Feb  5 18:26:02 2024, max compression
+gzip compressed data, was "yo-1.5.1.tar", last modified: Tue Apr  9 20:41:46 2024, max compression
```

## Comparing `yo-1.5.0.tar` & `yo-1.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-02-05 18:26:02.402679 yo-1.5.0/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-08-25 14:24:53.000000 yo-1.5.0/LICENSE.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-02-05 18:26:02.402679 yo-1.5.0/PKG-INFO
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-08-25 14:24:53.000000 yo-1.5.0/README.md
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-08-25 14:24:53.000000 yo-1.5.0/THIRD_PARTY_LICENSES.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)      307 2024-02-05 18:26:02.403679 yo-1.5.0/setup.cfg
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3464 2024-02-05 18:25:03.000000 yo-1.5.0/setup.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-02-05 18:26:02.401679 yo-1.5.0/tests/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-08-25 14:24:53.000000 yo-1.5.0/tests/test_api.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7576 2023-12-16 00:08:45.000000 yo-1.5.0/tests/test_cmds.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-02-05 18:26:02.402679 yo-1.5.0/yo/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)        0 2023-08-25 14:24:53.000000 yo-1.5.0/yo/__init__.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-08-25 14:24:53.000000 yo-1.5.0/yo/__main__.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)    86546 2024-02-05 18:25:03.000000 yo-1.5.0/yo/api.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-02-05 18:26:02.402679 yo-1.5.0/yo/data/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     9194 2023-12-16 00:08:45.000000 yo-1.5.0/yo/data/sample.yo.ini
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-02-05 18:26:02.402679 yo-1.5.0/yo/data/yo-tasks/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo-tasks/drgn
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo-tasks/ocid
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo-tasks/test-deps
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)       23 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo-tasks/test-existing-task
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo-tasks/test-run-many
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo-tasks/test-task
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-08-25 14:24:53.000000 yo-1.5.0/yo/data/yo_tasklib.sh
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)   134796 2024-02-05 18:25:03.000000 yo-1.5.0/yo/main.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     6384 2023-12-16 00:08:45.000000 yo-1.5.0/yo/oci.py
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)    10415 2023-09-01 17:04:54.000000 yo-1.5.0/yo/util.py
-drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-02-05 18:26:02.402679 yo-1.5.0/yo.egg-info/
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-02-05 18:26:02.000000 yo-1.5.0/yo.egg-info/PKG-INFO
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)      541 2024-02-05 18:26:02.000000 yo-1.5.0/yo.egg-info/SOURCES.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)        1 2024-02-05 18:26:02.000000 yo-1.5.0/yo.egg-info/dependency_links.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)       37 2024-02-05 18:26:02.000000 yo-1.5.0/yo.egg-info/entry_points.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)       72 2024-02-05 18:26:02.000000 yo-1.5.0/yo.egg-info/requires.txt
--rw-r--r--   0 stepbren  (1000) stepbren  (1000)        3 2024-02-05 18:26:02.000000 yo-1.5.0/yo.egg-info/top_level.txt
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.978702 yo-1.5.1/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1848 2023-08-25 14:24:53.000000 yo-1.5.1/LICENSE.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-04-09 20:41:46.978702 yo-1.5.1/PKG-INFO
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2532 2023-08-25 14:24:53.000000 yo-1.5.1/README.md
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)   156525 2023-08-25 14:24:53.000000 yo-1.5.1/THIRD_PARTY_LICENSES.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)      307 2024-04-09 20:41:46.978702 yo-1.5.1/setup.cfg
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3464 2024-04-09 20:41:38.000000 yo-1.5.1/setup.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/tests/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7971 2023-08-25 14:24:53.000000 yo-1.5.1/tests/test_api.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     7576 2023-12-16 00:08:45.000000 yo-1.5.1/tests/test_cmds.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/yo/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)        0 2023-08-25 14:24:53.000000 yo-1.5.1/yo/__init__.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1998 2023-08-25 14:24:53.000000 yo-1.5.1/yo/__main__.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)    86546 2024-02-05 18:25:03.000000 yo-1.5.1/yo/api.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/yo/data/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     9194 2023-12-16 00:08:45.000000 yo-1.5.1/yo/data/sample.yo.ini
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.978702 yo-1.5.1/yo/data/yo-tasks/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2396 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/drgn
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1956 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/ocid
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2032 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-deps
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)       23 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-existing-task
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1957 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-run-many
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     2008 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo-tasks/test-task
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     1277 2023-08-25 14:24:53.000000 yo-1.5.1/yo/data/yo_tasklib.sh
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)   135139 2024-04-09 20:41:38.000000 yo-1.5.1/yo/main.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     6384 2023-12-16 00:08:45.000000 yo-1.5.1/yo/oci.py
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)    10415 2023-09-01 17:04:54.000000 yo-1.5.1/yo/util.py
+drwxr-xr-x   0 stepbren  (1000) stepbren  (1000)        0 2024-04-09 20:41:46.977702 yo-1.5.1/yo.egg-info/
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)     3770 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/PKG-INFO
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)      541 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/SOURCES.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)        1 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/dependency_links.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)       37 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/entry_points.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)       72 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/requires.txt
+-rw-r--r--   0 stepbren  (1000) stepbren  (1000)        3 2024-04-09 20:41:46.000000 yo-1.5.1/yo.egg-info/top_level.txt
```

### Comparing `yo-1.5.0/LICENSE.txt` & `yo-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/PKG-INFO` & `yo-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.5.0
+Version: 1.5.1
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Description: # yo - fast and simple OCI client
```

### Comparing `yo-1.5.0/README.md` & `yo-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/THIRD_PARTY_LICENSES.txt` & `yo-1.5.1/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/setup.py` & `yo-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md").read()
 
-VERSION = "1.5.0"
+VERSION = "1.5.1"
 
 setup(
     name="yo",
     version=VERSION,
     description="A fast and simple CLI client for managing OCI instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `yo-1.5.0/tests/test_api.py` & `yo-1.5.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/tests/test_cmds.py` & `yo-1.5.1/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/__main__.py` & `yo-1.5.1/yo/__main__.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/api.py` & `yo-1.5.1/yo/api.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/sample.yo.ini` & `yo-1.5.1/yo/data/sample.yo.ini`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/yo-tasks/drgn` & `yo-1.5.1/yo/data/yo-tasks/drgn`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/yo-tasks/ocid` & `yo-1.5.1/yo/data/yo-tasks/ocid`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/yo-tasks/test-deps` & `yo-1.5.1/yo/data/yo-tasks/test-deps`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/yo-tasks/test-run-many` & `yo-1.5.1/yo/data/yo-tasks/test-run-many`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/yo-tasks/test-task` & `yo-1.5.1/yo/data/yo-tasks/test-task`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/data/yo_tasklib.sh` & `yo-1.5.1/yo/data/yo_tasklib.sh`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/main.py` & `yo-1.5.1/yo/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2088,14 +2088,20 @@
         parser.add_argument(
             "--cpu",
             type=float,
             default=None,
             help="Specify the amount of CPUs",
         )
         parser.add_argument(
+            "--ad",
+            type=str,
+            default=None,
+            help="Specify the availability domain (overrides instance profile)",
+        )
+        parser.add_argument(
             "--wait",
             "-w",
             action="store_true",
             help="Wait for the instance to start running",
         )
         parser.add_argument(
             "--wait-ssh",
@@ -2400,14 +2406,17 @@
         ).decode()
         return user_spec, user_data
 
     def run(self) -> None:
         profile = self.c.instance_profiles[self.args.profile]
         create_args = profile.create_arg_dict()
 
+        if self.args.ad:
+            create_args["availability_domain"] = self.args.ad
+
         if self.args.shape is not None:
             # override configured shape from "create_arg_dict()"
             create_args["shape"] = self.args.shape
         shape = self.c.get_shape_by_name(create_args["shape"])
         create_args["compartment_id"] = self.c.config.instance_compartment_id
         subnet = self.c.pick_subnet(profile.availability_domain)
         create_args["subnet_id"] = subnet.id
@@ -2635,15 +2644,19 @@
             action = self.force_action
         if self.args.dry_run:
             progress.log(f"DRY RUN: Would {action} {inst.id}")
             return
         self.do_action(inst, action)
 
     def post_for_instance(self, inst: YoInstance) -> None:
-        if self.args.wait and self.target_state and not self.args.dry_run:
+        if (
+            getattr(self.args, "wait", False)
+            and self.target_state
+            and not self.args.dry_run
+        ):
             inst = self.c.wait_instance_state(
                 inst.id,
                 self.target_state,
                 max_interval_seconds=1,
                 max_wait_seconds=600,
             )
             send_notification(
```

### Comparing `yo-1.5.0/yo/oci.py` & `yo-1.5.1/yo/oci.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo/util.py` & `yo-1.5.1/yo/util.py`

 * *Files identical despite different names*

### Comparing `yo-1.5.0/yo.egg-info/PKG-INFO` & `yo-1.5.1/yo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yo
-Version: 1.5.0
+Version: 1.5.1
 Summary: A fast and simple CLI client for managing OCI instances
 Home-page: https://github.com/oracle/yo
 Author: Oracle
 Author-email: stephen.s.brennan@oracle.com
 License: UPL
 Description: # yo - fast and simple OCI client
```

### Comparing `yo-1.5.0/yo.egg-info/SOURCES.txt` & `yo-1.5.1/yo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

