# Comparing `tmp/mysqld-integration-test-0.0.8.tar.gz` & `tmp/mysqld-integration-test-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqld-integration-test-0.0.8.tar", last modified: Sat Mar  4 17:59:38 2023, max compression
+gzip compressed data, was "mysqld-integration-test-0.0.9.tar", last modified: Sat Mar  4 19:33:44 2023, max compression
```

## Comparing `mysqld-integration-test-0.0.8.tar` & `mysqld-integration-test-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 17:59:38.892059 mysqld-integration-test-0.0.8/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)    11358 2023-03-03 04:08:29.000000 mysqld-integration-test-0.0.8/LICENSE
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3804 2023-03-04 17:59:38.892059 mysqld-integration-test-0.0.8/PKG-INFO
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3006 2023-03-04 17:52:10.000000 mysqld-integration-test-0.0.8/README.md
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 17:59:38.890059 mysqld-integration-test-0.0.8/mysqld_integration_test/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       50 2023-03-03 04:08:29.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/__init__.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       43 2023-03-04 12:50:15.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/exceptions.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      715 2023-03-04 17:56:56.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/helpers.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1571 2023-03-04 12:50:15.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/log.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     7049 2023-03-04 17:57:19.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/mysqld.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3013 2023-03-04 17:28:20.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/settings.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       22 2023-03-04 16:18:07.000000 mysqld-integration-test-0.0.8/mysqld_integration_test/version.py
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 17:59:38.891059 mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3804 2023-03-04 17:59:38.000000 mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/PKG-INFO
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      532 2023-03-04 17:59:38.000000 mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/SOURCES.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)        1 2023-03-04 17:59:38.000000 mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/dependency_links.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      120 2023-03-04 17:59:38.000000 mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/requires.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       24 2023-03-04 17:59:38.000000 mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/top_level.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1068 2023-03-04 17:52:35.000000 mysqld-integration-test-0.0.8/pyproject.toml
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       38 2023-03-04 17:59:38.892059 mysqld-integration-test-0.0.8/setup.cfg
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 17:59:38.892059 mysqld-integration-test-0.0.8/tests/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)       93 2023-03-03 04:08:29.000000 mysqld-integration-test-0.0.8/tests/test_sample.py
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 19:33:44.764833 mysqld-integration-test-0.0.9/
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)    11358 2023-03-03 04:08:29.000000 mysqld-integration-test-0.0.9/LICENSE
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3804 2023-03-04 19:33:44.764833 mysqld-integration-test-0.0.9/PKG-INFO
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3006 2023-03-04 17:52:10.000000 mysqld-integration-test-0.0.9/README.md
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 19:33:44.763833 mysqld-integration-test-0.0.9/mysqld_integration_test/
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       50 2023-03-03 04:08:29.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/__init__.py
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       43 2023-03-04 12:50:15.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/exceptions.py
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1157 2023-03-04 18:28:34.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/helpers.py
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1403 2023-03-04 18:27:17.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/log.py
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     7186 2023-03-04 19:30:35.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/mysqld.py
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3075 2023-03-04 19:31:29.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/settings.py
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       22 2023-03-04 18:48:03.000000 mysqld-integration-test-0.0.9/mysqld_integration_test/version.py
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 19:33:44.764833 mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3804 2023-03-04 19:33:44.000000 mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/PKG-INFO
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)      532 2023-03-04 19:33:44.000000 mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)        1 2023-03-04 19:33:44.000000 mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)      120 2023-03-04 19:33:44.000000 mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/requires.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       24 2023-03-04 19:33:44.000000 mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/top_level.txt
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1068 2023-03-04 18:48:08.000000 mysqld-integration-test-0.0.9/pyproject.toml
+-rw-r--r--   0 jcamp     (1000) jcamp     (1000)       38 2023-03-04 19:33:44.764833 mysqld-integration-test-0.0.9/setup.cfg
+drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2023-03-04 19:33:44.764833 mysqld-integration-test-0.0.9/tests/
+-rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)       93 2023-03-03 04:08:29.000000 mysqld-integration-test-0.0.9/tests/test_sample.py
```

### Comparing `mysqld-integration-test-0.0.8/LICENSE` & `mysqld-integration-test-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqld-integration-test-0.0.8/PKG-INFO` & `mysqld-integration-test-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqld-integration-test
-Version: 0.0.8
+Version: 0.0.9
 Summary: mysqld-integration-test is a python module that creates a temporary mysqld instance to use for testing your application.
 Author-email: Jason Camp <me@jason.camp>
 License: Apache
 Project-URL: Homepage, https://github.com/jasondcamp/mysqld-integration-test
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mysqld-integration-test-0.0.8/README.md` & `mysqld-integration-test-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mysqld-integration-test-0.0.8/mysqld_integration_test/log.py` & `mysqld-integration-test-0.0.9/mysqld_integration_test/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,51 @@
-import os
-import sys
 import logging
-from datetime import date
-
 from mysqld_integration_test.exceptions import InvalidLogLevel
 
-class bcolors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
+COLOR_OKBLUE = '\033[94m'
+COLOR_OKGREEN = '\033[92m'
+COLOR_WARNING = '\033[93m'
+COLOR_FAIL = '\033[91m'
+COLOR_ENDC = '\033[0m'
 
 class _Log():
     def __init__(self):
         logging.debug("magic")
         self.logger = logging.getLogger('mysqld-integration-test')
         self.logger.setLevel(logging.ERROR)
 
     def debug(self, msg):
         if self.logger:
             self.logger.debug(msg)
 
     def info(self, msg):
         if self.logger:
-            self.logger.info(self._colored(msg, bcolors.OKBLUE))
+            self.logger.info(_colored(msg, COLOR_OKBLUE))
 
     def error(self, msg):
         if self.logger:
-            self.logger.error(self._colored(msg, bcolors.FAIL))
+            self.logger.error(_colored(msg, COLOR_FAIL))
 
     def warn(self, msg):
         if self.logger:
-            self.logger.warn(self._colored(msg, bcolors.WARNING))
-
-    def _colored(self, msg, color):
-        return f"{color}{msg}{bcolors.ENDC}"
+            self.logger.warn(_colored(msg, COLOR_WARNING))
 
     def success(self, msg):
         if self.logger:
-            self.logger.info(self._colored(msg, bcolors.OKGREEN))
+            self.logger.info(_colored(msg, COLOR_OKGREEN))
 
     def setlevel(self, log_level):
         if log_level == "INFO":
             self.logger.setLevel(logging.INFO)
         elif log_level == "DEBUG":
             self.logger.setLevel(logging.DEBUG)
         elif log_level == 'ERROR':
             self.logger.setLevel(logging.ERROR)
         elif log_level == 'WARN':
             self.logger.setLevel(logging.WARN)
         else:
             raise InvalidLogLevel
 
+def _colored(msg, color):
+    return f"{color}{msg}{COLOR_ENDC}"
+
 logger = _Log()
```

### Comparing `mysqld-integration-test-0.0.8/mysqld_integration_test/mysqld.py` & `mysqld-integration-test-0.0.9/mysqld_integration_test/mysqld.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import atexit
 import tempfile
 import shutil
 import time
 import os
-import re
 import signal
 import subprocess
-import mysql.connector
-import tempfile
 from datetime import datetime
+import mysql.connector
 
 from mysqld_integration_test.log import logger
-from mysqld_integration_test.settings import Settings
+from mysqld_integration_test.helpers import Utils
+from mysqld_integration_test import settings
 from mysqld_integration_test.settings import ConfigFile
 from mysqld_integration_test.settings import ConfigInstance
 from mysqld_integration_test.version import __version__
 
 class Mysqld:
     def __init__(self, **kwargs):
         logger.debug(f"mysqd-integration-test {__version__}")
 
         self.child_process = None
+        self.terminate_signal = signal.SIGTERM
+        self.owner_pid = None
         self.base_dir = tempfile.mkdtemp()
         self.config = ConfigFile(base_dir=self.base_dir)
 
         if 'config_file' in kwargs:
             self.config.general.config_file = kwargs['config_file']
 
-        self.config = Settings.parse_config(self.config, kwargs)
+        self.config = settings.parse_config(self.config, kwargs)
         logger.setlevel(self.config.general.log_level)
 
         atexit.register(self.stop)
 
 
     def __del__(self):
         logger.debug(f"Cleaning up temp dir {self.config.dirs.base_dir}")
@@ -39,19 +40,20 @@
         time.sleep(0.5)
         shutil.rmtree(self.base_dir)
 
 
     def run(self):
         if self.child_process:
             logger.error("Error, database already running!")
-            return  # already started
+            return False  # already started
 
         # Get the mysql variant and version
-        (variant, version, version_minor) = self.parse_version(subprocess.check_output([self.config.database.mysqld_binary, '--version']).decode("utf-8"))
-        logger.debug(f"VERSION: {variant} {version} {version_minor}")
+        (variant, version_major, version_minor) = Utils.parse_version(
+                subprocess.check_output([self.config.database.mysqld_binary, '--version']).decode("utf-8"))
+        logger.debug(f"VERSION: {variant} {version_major} {version_minor}")
 
         # Set the owner pid
         self.owner_pid = os.getpid()
 
         # Build the mysql base fileset
         # Make base directories
         logger.debug("Creating application directories")
@@ -61,61 +63,79 @@
 
         # Write my.cnf
         logger.debug("Writing my.cnf")
         self.write_mycnf()
 
         # Initialize database files
         logger.debug("Initializing databases with mysql_install_db")
-        subprocess.Popen([self.config.database.mysql_install_db_binary, f"--defaults-file={os.path.join(self.config.dirs.etc_dir, 'my.cnf')}", f"--datadir={self.config.dirs.data_dir}"] , stdout=subprocess.PIPE, stderr=subprocess.STDOUT).communicate()
+        subprocess.Popen([self.config.database.mysql_install_db_binary,
+            f"--defaults-file={os.path.join(self.config.dirs.etc_dir, 'my.cnf')}",
+            f"--datadir={self.config.dirs.data_dir}"] ,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT).communicate()
 
         # Start up the database
         try:
             logger.debug("Starting mysql")
-            self.mysql_command_line = [self.config.database.mysqld_binary, f"--defaults-file={os.path.join(self.config.dirs.etc_dir, 'my.cnf')}"]
-            self.child_process = subprocess.Popen(self.mysql_command_line, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-        except Exception as e:
-            raise RuntimeError('failed to start %s: %r' % (self.name, e))
+            mysql_command_line = [self.config.database.mysqld_binary, f"--defaults-file={os.path.join(self.config.dirs.etc_dir, 'my.cnf')}"]
+            self.child_process = subprocess.Popen(mysql_command_line, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        except Exception as exc:
+            raise RuntimeError(f"Failed to start mysqld: {exc}")
         else:
             try:
                 self.wait_booting()
             except Exception:
                 self.stop()
                 raise
 
         # MariaDB 10 requires that you log in as the user that is running the mysql instance and reset the root pw
         # Set password
         # Get the current user
-        if variant == "mariadb" and version >= 10:
+        if variant == "mariadb" and version_major >= 10:
             logger.debug("Detected MariaDB >= 10: Resetting password")
-            current_user = os.getlogin()
-            cnx = mysql.connector.connect(user=current_user, unix_socket=self.config.database.socket_file,
-                                  host=self.config.database.host, port=self.config.database.port)
-            cursor = cnx.cursor()
-            cursor.execute(f"ALTER USER '{self.config.database.username}'@'localhost' IDENTIFIED BY '{self.config.database.password}';")
-            cursor.execute("FLUSH PRIVILEGES;")
-            cnx.commit()
-            cursor.close()
-            cnx.close()
+            self.reset_password_current_user()
 
         # create test database
-        cnx = mysql.connector.connect(user=current_user, unix_socket=self.config.database.socket_file,
-                              host=self.config.database.host, port=self.config.database.port)
+        self.create_test_database()
+
+        # Return specifics the user can use to connect to the test instance
+        instance_config = ConfigInstance({
+                'host': self.config.database.host,
+                'port': self.config.database.port,
+                'username': self.config.database.username,
+                'password': self.config.database.password,
+                'socket_file': self.config.database.socket_file})
+
+        return instance_config
+
+
+    def reset_password_current_user(self):
+        current_user = os.getlogin()
+        cnx = mysql.connector.connect(user=current_user,
+                                      unix_socket=self.config.database.socket_file,
+                                      host=self.config.database.host,
+                                      port=self.config.database.port)
         cursor = cnx.cursor()
-        cursor.execute('CREATE DATABASE IF NOT EXISTS test')
+        cursor.execute(f"ALTER USER '{self.config.database.username}'@'localhost' IDENTIFIED BY '{self.config.database.password}';")
+        cursor.execute("FLUSH PRIVILEGES;")
         cnx.commit()
         cursor.close()
         cnx.close()
 
-        # Return specifics the user can use to connect to the test instance
-        instance_config = ConfigInstance()
-        instance_config.host = self.config.database.host
-        instance_config.port = self.config.database.port
-        instance_config.username = self.config.database.username
-        instance_config.password = self.config.database.password
-        return(instance_config)
+
+    def create_test_database(self):
+        cnx = mysql.connector.connect(user=self.config.database.username,
+                                      password=self.config.database.password,
+                                      host=self.config.database.host,
+                                      port=self.config.database.port)
+        cursor = cnx.cursor()
+        cursor.execute('CREATE DATABASE IF NOT EXISTS test')
+        cnx.commit()
+        cursor.close()
+        cnx.close()
 
 
     def stop(self, _signal=signal.SIGTERM):
         self.terminate(_signal)
 
 
     def terminate(self, _signal=None):
@@ -141,15 +161,15 @@
         except OSError:
             pass
 
         self.child_process = None
 
 
     def write_mycnf(self):
-        with open(os.path.join(self.config.dirs.etc_dir, 'my.cnf'), 'wt') as my_cnf:
+        with open(os.path.join(self.config.dirs.etc_dir, 'my.cnf'), 'wt', encoding='utf-8') as my_cnf:
             my_cnf.write("[mysqld]" + "\n")
             my_cnf.write(f"bind-address={self.config.database.host}" + "\n")
             my_cnf.write(f"port={self.config.database.port}" + "\n")
             my_cnf.write(f"datadir={self.config.dirs.data_dir}" + "\n")
             my_cnf.write(f"tmpdir={self.config.dirs.tmp_dir}" + "\n")
             my_cnf.write(f"socket={self.config.database.socket_file}" + "\n")
             my_cnf.write(f"pid-file={self.config.database.pid_file}" + "\n")
@@ -167,21 +187,7 @@
             if (datetime.now() - exec_at).seconds > self.config.general.timeout_start:
                 raise RuntimeError("Failed to launch mysql binary (timeout)")
 
             time.sleep(0.5)
 
     def is_server_available(self):
         return os.path.exists(self.config.database.pid_file)
-
-
-    def parse_version(self, version):
-        version_info = (re.findall(r"Ver (\d+)\.([0-9.]+)\-(\w+)", version))
-        version_major = int(version_info[0][0])
-        version_minor = version_info[0][1]
-        version_variant = version_info[0][2].lower()
-
-        if version_major == 8:
-            version_variant = "mysql"
-
-        return (version_variant, version_major, version_minor)
-
-
```

### Comparing `mysqld-integration-test-0.0.8/mysqld_integration_test/settings.py` & `mysqld-integration-test-0.0.9/mysqld_integration_test/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 import os
-import yaml
-import sys
-import tempfile
 import functools
+import yaml
 
 from mysqld_integration_test.version import __version__
 from mysqld_integration_test.helpers import Utils
 
+#ARGS_DATABASE = [ 'username', 'password', 'host', 'port', 'mysql_install_db_binary', 'mysqld_binary' ]
+#ARGS_GENERAL = [ 'timeout_start', 'timeout_stop', 'log_level', 'config_file']
+config_settings = {}
+config_settings['database'] = [ 'username', 'password', 'host', 'port', 'mysql_install_db_binary', 'mysqld_binary' ]
+config_settings['general'] = [ 'timeout_start', 'timeout_stop', 'log_level', 'config_file' ]
+
 def rgetattr(obj, attr, *args):
     def _getattr(obj, attr):
         return getattr(obj, attr, *args)
     return functools.reduce(_getattr, [obj] + attr.split('.'))
 
 
 def rsetattr(obj, attr, val):
     pre, _, post = attr.rpartition('.')
     return setattr(rgetattr(obj, pre) if pre else obj, post, val)
 
 
-class Settings():
-    def __init__(self, args):
-        self.args = args
+def merge_configs(config, section, section_cfg):
+    for arg in config_settings[section]:
+        if arg in section_cfg:
+            rsetattr(config, f"{section}.{arg}", section_cfg[arg])
+
+    return config
 
-    @classmethod
-    def parse_config(cls, config, config_args):
-        args = {}
-        args['database'] = [ 'username', 'password', 'host', 'port', 'mysql_install_db_binary', 'mysqld_binary' ]
-        args['general'] = [ 'timeout_start', 'timeout_stop', 'log_level', 'config_file' ]
-
-        # See if there is a config file
-        if os.path.exists(config.general.config_file):
-            with open(config.general.config_file, "r", encoding='utf-8') as ymlfile:
-                cfg = yaml.load(ymlfile, Loader=yaml.FullLoader)
-
-            # Merge config together with args
-            for section in args:
-                for arg in args[section]:
-                    if arg in cfg[section]:
-                        # Set the value from the config file
-                        rsetattr(config, f"{section}.{arg}", cfg[section][arg])
-
-        # Merge in any class arguments
-        for section in args:
-            for arg in args[section]:
-                if arg in config_args:
-                    rsetattr(config, f"{section}.{arg}", config_args[arg])
 
-        return config
+def parse_config(config, config_args):
+    # See if there is a config file
+    if os.path.exists(config.general.config_file):
+        with open(config.general.config_file, "r", encoding='utf-8') as ymlfile:
+            cfg = yaml.load(ymlfile, Loader=yaml.FullLoader)
 
+        # Merge config together with args
+        for section in config_settings:
+            config = merge_configs(config, section, cfg[section])
 
-class ConfigAttribute(object):
+    # Merge in any class arguments
+    for section in config_settings:
+        config = merge_configs(config, section, config_args)
+
+    return config
+
+
+class ConfigAttribute():
     pass
 
 
 class ConfigFile():
     def __init__(self, base_dir):
         self.dirs = ConfigAttribute()
         self.dirs.base_dir = base_dir
@@ -75,14 +73,13 @@
         self.general.timeout_start = 30
         self.general.timeout_stop = 30
         self.general.log_level = "INFO"
         self.general.config_file = 'mysqld-integration-test.cfg'
 
 
 class ConfigInstance():
-    def __init__(self):
-        self.host = None
-        self.port = None
-        self.username = None
-        self.password = None
-        self.socket_file = None
-
+    def __init__(self, args):
+        self.host = args['host']
+        self.port = args['port']
+        self.username = args['username']
+        self.password = args['password']
+        self.socket_file = args['socket_file']
```

### Comparing `mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/PKG-INFO` & `mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqld-integration-test
-Version: 0.0.8
+Version: 0.0.9
 Summary: mysqld-integration-test is a python module that creates a temporary mysqld instance to use for testing your application.
 Author-email: Jason Camp <me@jason.camp>
 License: Apache
 Project-URL: Homepage, https://github.com/jasondcamp/mysqld-integration-test
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mysqld-integration-test-0.0.8/mysqld_integration_test.egg-info/SOURCES.txt` & `mysqld-integration-test-0.0.9/mysqld_integration_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysqld-integration-test-0.0.8/pyproject.toml` & `mysqld-integration-test-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mysqld-integration-test"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{name = "Jason Camp", email = "me@jason.camp"}]
 license = {text = "Apache"}
 description = "mysqld-integration-test is a python module that creates a temporary mysqld instance to use for testing your application."
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
```

