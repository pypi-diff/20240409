# Comparing `tmp/neon_speech-4.3.1a2.tar.gz` & `tmp/neon_speech-4.3.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_speech-4.3.1a2.tar", last modified: Tue Jan 30 20:28:41 2024, max compression
+gzip compressed data, was "neon_speech-4.3.1a3.tar", last modified: Tue Apr  9 01:06:02 2024, max compression
```

## Comparing `neon_speech-4.3.1a2.tar` & `neon_speech-4.3.1a3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 20:28:41.184906 neon_speech-4.3.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-01-30 20:28:41.184906 neon_speech-4.3.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 20:28:41.184906 neon_speech-4.3.1a2/neon_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/neon_speech/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 20:28:41.184906 neon_speech-4.3.1a2/neon_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-01-30 20:28:41.000000 neon_speech-4.3.1a2/neon_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-30 20:28:41.000000 neon_speech-4.3.1a2/neon_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 20:28:41.000000 neon_speech-4.3.1a2/neon_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-30 20:28:41.000000 neon_speech-4.3.1a2/neon_speech.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-30 20:28:41.000000 neon_speech-4.3.1a2/neon_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 20:28:41.000000 neon_speech-4.3.1a2/neon_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 20:28:41.184906 neon_speech-4.3.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-01-30 20:28:35.000000 neon_speech-4.3.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:06:02.335735 neon_speech-4.3.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 01:06:02.335735 neon_speech-4.3.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:06:02.335735 neon_speech-4.3.1a3/neon_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27197 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/neon_speech/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 01:06:02.335735 neon_speech-4.3.1a3/neon_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 01:06:02.000000 neon_speech-4.3.1a3/neon_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 01:06:02.000000 neon_speech-4.3.1a3/neon_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 01:06:02.000000 neon_speech-4.3.1a3/neon_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 01:06:02.000000 neon_speech-4.3.1a3/neon_speech.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 01:06:02.000000 neon_speech-4.3.1a3/neon_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 01:06:02.000000 neon_speech-4.3.1a3/neon_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 01:06:02.335735 neon_speech-4.3.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-09 01:05:56.000000 neon_speech-4.3.1a3/setup.py
```

### Comparing `neon_speech-4.3.1a2/LICENSE.md` & `neon_speech-4.3.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/PKG-INFO` & `neon_speech-4.3.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_speech
-Version: 4.3.1a2
+Version: 4.3.1a3
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.3.1a2/README.md` & `neon_speech-4.3.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/neon_speech/__init__.py` & `neon_speech-4.3.1a3/neon_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/neon_speech/__main__.py` & `neon_speech-4.3.1a3/neon_speech/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/neon_speech/cli.py` & `neon_speech-4.3.1a3/neon_speech/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,18 +23,22 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import click
+import sys
+from typing import List
 
 from click_default_group import DefaultGroup
 from neon_utils.packaging_utils import get_package_version_spec
 from neon_utils.configuration_utils import init_config_dir
+from ovos_config.config import Configuration
+from ovos_utils.log import LOG, log_deprecation
 
 
 @click.group("neon-speech", cls=DefaultGroup,
              no_args_is_help=True, invoke_without_command=True,
              help="Neon Core Commands\n\n"
                   "See also: neon COMMAND --help")
 @click.option("--version", "-v", is_flag=True, required=False,
@@ -79,28 +83,40 @@
 @click.option("--module", "-m", default=None,
               help="STT Plugin to configure")
 @click.option("--package", "-p", default=None,
               help="STT package spec to install")
 @click.option("--force-install", "-f", default=False, is_flag=True,
               help="Force pip installation of configured module")
 def install_plugin(module, package, force_install):
+    log_deprecation("`install-plugin` replaced by `install-dependencies`", "2.0.0")
     from neon_speech.utils import install_stt_plugin
     from ovos_config.config import Configuration
     speech_config = Configuration()
 
     if force_install and not (package or module):
         click.echo("Installing STT plugin from configuration")
         module = module or speech_config.get("stt", {}).get("module")
         package = package or speech_config.get("stt", {}).get("package_spec")
 
     if module:
         install_stt_plugin(package or module)
         if not module:
             click.echo("Plugin specified without module")
 
+@neon_speech_cli.command(help="Install neon-speech module dependencies from config & cli")
+@click.option("--package", "-p", default=[], multiple=True,
+              help="Additional package to install (can be repeated)")
+def install_dependencies(package: List[str]):
+    from neon_utils.packaging_utils import install_packages_from_pip
+    from neon_speech.utils import build_extra_dependency_list
+    config = Configuration()
+    dependencies = build_extra_dependency_list(config, list(package))
+    result = install_packages_from_pip("neon-speech", dependencies)
+    LOG.info(f"pip exit code: {result}")
+    sys.exit(result)
 
 @neon_speech_cli.command(help="Install a STT Plugin")
 @click.option("--plugin", "-p", default=None,
               help="STT module to init")
 def init_plugin(plugin):
     from neon_speech.utils import init_stt_plugin
     from ovos_config.config import Configuration
```

### Comparing `neon_speech-4.3.1a2/neon_speech/service.py` & `neon_speech-4.3.1a3/neon_speech/service.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/neon_speech/stt.py` & `neon_speech-4.3.1a3/neon_speech/stt.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/neon_speech/transformers.py` & `neon_speech-4.3.1a3/neon_speech/transformers.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.3.1a2/neon_speech/utils.py` & `neon_speech-4.3.1a3/neon_speech/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from tempfile import mkstemp
-from ovos_utils.log import LOG
+from ovos_utils.log import LOG, deprecated
 from neon_utils.packaging_utils import get_package_dependencies
+from ovos_config.config import Configuration
+from typing import List, Union
 
 
 def patch_config(config: dict = None):
     """
     Write the specified speech configuration to the global config file
     :param config: Mycroft-compatible configuration override
     """
@@ -54,15 +56,21 @@
     known_plugins = {
         "deepspeech_stream_local": "neon-stt-plugin-deepspeech-stream-local",
         "polyglot": "neon-stt-plugin-polyglot",
         "google_cloud_streaming": "neon-stt-plugin-google-cloud-streaming",
     }
     return known_plugins.get(plugin) or plugin
 
+def build_extra_dependency_list(config: Union[dict, Configuration], additional: List[str] = []) -> List[str]:
+    extra_dependencies = config.get("extra_dependencies", {})
+    dependencies = additional + extra_dependencies.get("global", []) + extra_dependencies.get("voice", [])
 
+    return dependencies
+
+@deprecated("Replaced by `neon_utils.packaging_utils.install_packages_from_pip`", "2.0.0")
 def install_stt_plugin(plugin: str) -> bool:
     """
     Install an stt plugin using pip
     :param plugin: entrypoint of plugin to install
     :returns: True if the plugin installation is successful
     """
     import pip
```

### Comparing `neon_speech-4.3.1a2/neon_speech.egg-info/PKG-INFO` & `neon_speech-4.3.1a3/neon_speech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 4.3.1a2
+Version: 4.3.1a3
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.3.1a2/setup.py` & `neon_speech-4.3.1a3/setup.py`

 * *Files identical despite different names*

