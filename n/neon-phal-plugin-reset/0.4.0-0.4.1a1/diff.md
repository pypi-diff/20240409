# Comparing `tmp/neon-phal-plugin-reset-0.4.0.tar.gz` & `tmp/neon-phal-plugin-reset-0.4.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-reset-0.4.0.tar", last modified: Tue Sep  5 22:31:33 2023, max compression
+gzip compressed data, was "neon-phal-plugin-reset-0.4.1a1.tar", last modified: Mon Apr  8 23:14:49 2024, max compression
```

## Comparing `neon-phal-plugin-reset-0.4.0.tar` & `neon-phal-plugin-reset-0.4.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:31:33.597987 neon-phal-plugin-reset-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1634 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (999)       33 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     1038 2023-09-05 22:31:33.597987 neon-phal-plugin-reset-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      741 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:31:33.593987 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/
--rw-r--r--   0 runner    (1001) docker     (999)    15332 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2687 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     4062 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/create_media.py
--rw-r--r--   0 runner    (1001) docker     (999)     1854 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:31:33.597987 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1038 2023-09-05 22:31:33.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      490 2023-09-05 22:31:33.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 22:31:33.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       85 2023-09-05 22:31:33.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      107 2023-09-05 22:31:33.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-09-05 22:31:33.000000 neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 22:31:33.597987 neon-phal-plugin-reset-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (999)      106 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-05 22:31:33.597987 neon-phal-plugin-reset-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     3719 2023-09-05 22:31:29.000000 neon-phal-plugin-reset-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:14:49.016882 neon-phal-plugin-reset-0.4.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 23:14:49.016882 neon-phal-plugin-reset-0.4.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:14:49.012882 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/create_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:14:49.012882 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 23:14:48.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-08 23:14:49.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:14:48.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 23:14:48.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 23:14:48.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 23:14:48.000000 neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:14:49.016882 neon-phal-plugin-reset-0.4.1a1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:14:49.016882 neon-phal-plugin-reset-0.4.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-04-08 23:14:44.000000 neon-phal-plugin-reset-0.4.1a1/setup.py
```

### Comparing `neon-phal-plugin-reset-0.4.0/LICENSE.md` & `neon-phal-plugin-reset-0.4.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.4.0/PKG-INFO` & `neon-phal-plugin-reset-0.4.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.4.0
+Version: 0.4.1a1
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-reset-0.4.0/README.md` & `neon-phal-plugin-reset-0.4.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/__init__.py` & `neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/config.py` & `neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/config.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/create_media.py` & `neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/create_media.py`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset/version.py` & `neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.4.0"
+__version__ = "0.4.1a1"
```

### Comparing `neon-phal-plugin-reset-0.4.0/neon_phal_plugin_reset.egg-info/PKG-INFO` & `neon-phal-plugin-reset-0.4.1a1/neon_phal_plugin_reset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.4.0
+Version: 0.4.1a1
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-reset-0.4.0/setup.py` & `neon-phal-plugin-reset-0.4.1a1/setup.py`

 * *Files identical despite different names*

