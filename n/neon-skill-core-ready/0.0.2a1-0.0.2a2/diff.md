# Comparing `tmp/neon-skill-core_ready-0.0.2a1.tar.gz` & `tmp/neon-skill-core_ready-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-core_ready-0.0.2a1.tar", last modified: Tue Feb  6 01:52:43 2024, max compression
+gzip compressed data, was "neon-skill-core_ready-0.0.2a2.tar", last modified: Tue Apr  9 16:47:47 2024, max compression
```

## Comparing `neon-skill-core_ready-0.0.2a1.tar` & `neon-skill-core_ready-0.0.2a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.574614 neon-skill-core_ready-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-06 01:52:43.574614 neon-skill-core_ready-0.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.570614 neon-skill-core_ready-0.0.2a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.570614 neon-skill-core_ready-0.0.2a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.570614 neon-skill-core_ready-0.0.2a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/locale/en-us/dialog/confirm_no_speak_ready.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/locale/en-us/dialog/confirm_speak_ready.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/locale/en-us/dialog/ready.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.570614 neon-skill-core_ready-0.0.2a1/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/locale/en-us/intent/disable_ready_notification.intent
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/locale/en-us/intent/enable_ready_notification.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.574614 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-06 01:52:43.000000 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-06 01:52:43.000000 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:52:43.000000 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-06 01:52:43.000000 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-06 01:52:43.000000 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:52:43.000000 neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:52:43.574614 neon-skill-core_ready-0.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:52:43.574614 neon-skill-core_ready-0.0.2a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:52:34.000000 neon-skill-core_ready-0.0.2a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.925021 neon-skill-core_ready-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-09 16:47:47.925021 neon-skill-core_ready-0.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.921021 neon-skill-core_ready-0.0.2a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.921021 neon-skill-core_ready-0.0.2a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.921021 neon-skill-core_ready-0.0.2a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/locale/en-us/dialog/confirm_no_speak_ready.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/locale/en-us/dialog/confirm_speak_ready.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/locale/en-us/dialog/ready.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.921021 neon-skill-core_ready-0.0.2a2/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/locale/en-us/intent/disable_ready_notification.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/locale/en-us/intent/enable_ready_notification.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.925021 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-09 16:47:47.000000 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 16:47:47.000000 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:47:47.000000 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 16:47:47.000000 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 16:47:47.000000 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:47:47.000000 neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:47:47.925021 neon-skill-core_ready-0.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:47:47.925021 neon-skill-core_ready-0.0.2a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-09 16:47:40.000000 neon-skill-core_ready-0.0.2a2/version.py
```

### Comparing `neon-skill-core_ready-0.0.2a1/LICENSE.md` & `neon-skill-core_ready-0.0.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-core_ready-0.0.2a1/PKG-INFO` & `neon-skill-core_ready-0.0.2a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-core_ready
-Version: 0.0.2a1
+Version: 0.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-core_ready
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-core_ready-0.0.2a1/README.md` & `neon-skill-core_ready-0.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-core_ready-0.0.2a1/__init__.py` & `neon-skill-core_ready-0.0.2a2/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_bus_client import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
-from neon_utils.skills import NeonSkill
-from ovos_workshop import intent_handler
+from ovos_workshop.decorators import intent_handler
+from ovos_workshop.skills import OVOSSkill
 
 
-class CoreReadySkill(NeonSkill):
+class CoreReadySkill(OVOSSkill):
     def __init__(self, **kwargs):
-        NeonSkill.__init__(self, **kwargs)
+        OVOSSkill.__init__(self, **kwargs)
         self.add_event("mycroft.ready", self.handle_ready)
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
@@ -56,15 +56,15 @@
         """
         Speak `ready` dialog when ready unless disabled in settings
         """
         return self.settings.get("speak_ready") is not False
 
     def handle_ready(self, _: Message):
         """
-        Handle mycroft.ready event. Notify the user everything is ready if
+        Handle `mycroft.ready` event. Notify the user everything is ready if
         configured.
         """
         if self.speak_ready:
             self.speak_dialog("ready")
         else:
             LOG.info("Ready notification disabled in settings")
```

### Comparing `neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/PKG-INFO` & `neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-core-ready
-Version: 0.0.2a1
+Version: 0.0.2a2
 Home-page: https://github.com/NeonGeckoCom/skill-core_ready
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-core_ready-0.0.2a1/neon_skill_core_ready.egg-info/SOURCES.txt` & `neon-skill-core_ready-0.0.2a2/neon_skill_core_ready.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-core_ready-0.0.2a1/setup.py` & `neon-skill-core_ready-0.0.2a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-core_ready-0.0.2a1/skill.json` & `neon-skill-core_ready-0.0.2a2/skill.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990530303030302%*

 * *Differences: {"'requirements'": "{'python': {delete: [0]}}"}*

```diff
@@ -24,15 +24,14 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
-            "neon-utils~=1.2",
             "ovos-bus-client~=0.0.3",
             "ovos-utils~=0.0, >=0.0.28",
             "ovos-workshop~=0.0.12"
         ],
         "skill": [],
         "system": {}
     },
```

### Comparing `neon-skill-core_ready-0.0.2a1/test/test_skill.py` & `neon-skill-core_ready-0.0.2a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-core_ready-0.0.2a1/version.py` & `neon-skill-core_ready-0.0.2a2/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.0.2a1"
+__version__ = "0.0.2a2"
```

