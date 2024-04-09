# Comparing `tmp/kas-4.3.1.tar.gz` & `tmp/kas-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kas-4.3.1.tar", last modified: Wed Mar 13 07:05:39 2024, max compression
+gzip compressed data, was "dist/kas-4.3.2.tar", last modified: Tue Apr  9 17:26:02 2024, max compression
```

## Comparing `kas-4.3.1.tar` & `kas-4.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-03-13 07:05:39.000000 kas-4.3.1/
--rw-r--r--   0 jan       (1000) users      (100)     2941 2024-03-13 07:05:39.000000 kas-4.3.1/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-4.3.1/README.rst
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-03-13 07:05:39.000000 kas-4.3.1/kas/
--rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-4.3.1/kas/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-4.3.1/kas/__main__.py
--rw-r--r--   0 jan       (1000) users      (100)     1422 2024-03-13 07:05:25.000000 kas-4.3.1/kas/__version__.py
--rw-r--r--   0 jan       (1000) users      (100)     7835 2024-02-13 09:50:23.000000 kas-4.3.1/kas/config.py
--rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-4.3.1/kas/configschema.py
--rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-4.3.1/kas/context.py
--rw-r--r--   0 jan       (1000) users      (100)    12489 2024-02-25 18:08:37.000000 kas-4.3.1/kas/includehandler.py
--rw-r--r--   0 jan       (1000) users      (100)     6532 2023-12-18 09:28:13.000000 kas-4.3.1/kas/kas.py
--rw-r--r--   0 jan       (1000) users      (100)     2794 2023-12-18 09:28:13.000000 kas-4.3.1/kas/kasusererror.py
--rw-r--r--   0 jan       (1000) users      (100)    14485 2024-02-25 18:08:37.000000 kas-4.3.1/kas/libcmds.py
--rw-r--r--   0 jan       (1000) users      (100)    13868 2024-03-13 06:22:05.000000 kas-4.3.1/kas/libkas.py
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-03-13 07:05:39.000000 kas-4.3.1/kas/plugins/
--rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-4.3.1/kas/plugins/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     4293 2024-02-25 18:08:37.000000 kas-4.3.1/kas/plugins/build.py
--rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-4.3.1/kas/plugins/checkout.py
--rw-r--r--   0 jan       (1000) users      (100)     8739 2023-12-18 09:28:13.000000 kas-4.3.1/kas/plugins/dump.py
--rw-r--r--   0 jan       (1000) users      (100)     5333 2023-10-20 17:38:55.000000 kas-4.3.1/kas/plugins/for_all_repos.py
--rw-r--r--   0 jan       (1000) users      (100)    18592 2024-02-25 18:08:37.000000 kas-4.3.1/kas/plugins/menu.py
--rw-r--r--   0 jan       (1000) users      (100)     4451 2023-05-19 05:17:03.000000 kas-4.3.1/kas/plugins/shell.py
--rw-r--r--   0 jan       (1000) users      (100)    23418 2024-03-07 16:57:42.000000 kas-4.3.1/kas/repos.py
--rw-r--r--   0 jan       (1000) users      (100)    10018 2024-02-13 09:50:23.000000 kas-4.3.1/kas/schema-kas.json
--rwxr-xr-x   0 jan       (1000) users      (100)    17963 2024-03-13 07:05:25.000000 kas-4.3.1/kas-container
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/
--rw-r--r--   0 jan       (1000) users      (100)     2941 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)      586 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) users      (100)        1 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) users      (100)       38 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/entry_points.txt
--rw-r--r--   0 jan       (1000) users      (100)       96 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/requires.txt
--rw-r--r--   0 jan       (1000) users      (100)        4 2024-03-13 07:05:39.000000 kas-4.3.1/kas.egg-info/top_level.txt
--rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-4.3.1/pyproject.toml
--rw-r--r--   0 jan       (1000) users      (100)       38 2024-03-13 07:05:39.000000 kas-4.3.1/setup.cfg
--rw-r--r--   0 jan       (1000) users      (100)     3342 2024-03-02 08:32:56.000000 kas-4.3.1/setup.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/
+-rw-r--r--   0 jan       (1000) users      (100)     2941 2024-04-09 17:26:02.000000 kas-4.3.2/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-4.3.2/README.rst
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/kas/
+-rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-4.3.2/kas/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-4.3.2/kas/__main__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1422 2024-04-09 17:25:46.000000 kas-4.3.2/kas/__version__.py
+-rw-r--r--   0 jan       (1000) users      (100)     7835 2024-02-13 09:50:23.000000 kas-4.3.2/kas/config.py
+-rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-4.3.2/kas/configschema.py
+-rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-4.3.2/kas/context.py
+-rw-r--r--   0 jan       (1000) users      (100)    12489 2024-02-25 18:08:37.000000 kas-4.3.2/kas/includehandler.py
+-rw-r--r--   0 jan       (1000) users      (100)     6532 2024-04-09 15:54:13.000000 kas-4.3.2/kas/kas.py
+-rw-r--r--   0 jan       (1000) users      (100)     2794 2023-12-18 09:28:13.000000 kas-4.3.2/kas/kasusererror.py
+-rw-r--r--   0 jan       (1000) users      (100)    14530 2024-04-09 15:54:13.000000 kas-4.3.2/kas/libcmds.py
+-rw-r--r--   0 jan       (1000) users      (100)    13868 2024-03-13 06:22:05.000000 kas-4.3.2/kas/libkas.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/kas/plugins/
+-rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-4.3.2/kas/plugins/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     4293 2024-02-25 18:08:37.000000 kas-4.3.2/kas/plugins/build.py
+-rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-4.3.2/kas/plugins/checkout.py
+-rw-r--r--   0 jan       (1000) users      (100)     8739 2023-12-18 09:28:13.000000 kas-4.3.2/kas/plugins/dump.py
+-rw-r--r--   0 jan       (1000) users      (100)     5333 2023-10-20 17:38:55.000000 kas-4.3.2/kas/plugins/for_all_repos.py
+-rw-r--r--   0 jan       (1000) users      (100)    18592 2024-02-25 18:08:37.000000 kas-4.3.2/kas/plugins/menu.py
+-rw-r--r--   0 jan       (1000) users      (100)     4451 2023-05-19 05:17:03.000000 kas-4.3.2/kas/plugins/shell.py
+-rw-r--r--   0 jan       (1000) users      (100)    23420 2024-04-09 15:54:13.000000 kas-4.3.2/kas/repos.py
+-rw-r--r--   0 jan       (1000) users      (100)    10018 2024-02-13 09:50:23.000000 kas-4.3.2/kas/schema-kas.json
+-rwxr-xr-x   0 jan       (1000) users      (100)    17993 2024-04-09 17:25:46.000000 kas-4.3.2/kas-container
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/
+-rw-r--r--   0 jan       (1000) users      (100)     2941 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)      586 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) users      (100)        1 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) users      (100)       38 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/entry_points.txt
+-rw-r--r--   0 jan       (1000) users      (100)       96 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/requires.txt
+-rw-r--r--   0 jan       (1000) users      (100)        4 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/top_level.txt
+-rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-4.3.2/pyproject.toml
+-rw-r--r--   0 jan       (1000) users      (100)       38 2024-04-09 17:26:02.000000 kas-4.3.2/setup.cfg
+-rw-r--r--   0 jan       (1000) users      (100)     3342 2024-03-02 08:32:56.000000 kas-4.3.2/setup.py
```

### Comparing `kas-4.3.1/PKG-INFO` & `kas-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 4.3.1
+Version: 4.3.2
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
 Download-URL: https://github.com/siemens/kas/archive/{__version__}.tar.gz
 Description: Setup tool for bitbake based projects
```

### Comparing `kas-4.3.1/README.rst` & `kas-4.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/__init__.py` & `kas-4.3.2/kas/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/__main__.py` & `kas-4.3.2/kas/__main__.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/__version__.py` & `kas-4.3.2/kas/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 # SOFTWARE.
 """
     This module contains the version of kas.
 """
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2020'
 
-__version__ = '4.3.1'
+__version__ = '4.3.2'
 
 # Please update docs/format-changelog.rst when changing the file version.
 __file_version__ = 16
 __compatible_file_version__ = 1
```

### Comparing `kas-4.3.1/kas/config.py` & `kas-4.3.2/kas/config.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/configschema.py` & `kas-4.3.2/kas/configschema.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/context.py` & `kas-4.3.2/kas/context.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/includehandler.py` & `kas-4.3.2/kas/includehandler.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/kas.py` & `kas-4.3.2/kas/kas.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
     This module is the main entry point for kas, setup tool for bitbake based
     projects. In case of user errors (e.g. invalid configuration, repo fetch
-    failure) KAS exits with error code 2, while exiting with 1 for internal
+    failure) kas exits with error code 2, while exiting with 1 for internal
     errors. For details on error handling, see :mod:`kas.kasusererror`.
 """
 
 import argparse
 import atexit
 import asyncio
 import traceback
```

### Comparing `kas-4.3.1/kas/kasusererror.py` & `kas-4.3.2/kas/kasusererror.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/libcmds.py` & `kas-4.3.2/kas/libcmds.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,25 @@
 
     def __del__(self):
         shutil.rmtree(self.tmpdirname)
 
     def __str__(self):
         return 'setup_home'
 
+    def _setup_netrc(self):
+        if os.environ.get('NETRC_FILE', False):
+            shutil.copy(os.environ['NETRC_FILE'],
+                        self.tmpdirname + "/.netrc")
+        if os.environ.get('CI_SERVER_HOST', False) \
+                and os.environ.get('CI_JOB_TOKEN', False):
+            with open(self.tmpdirname + '/.netrc', 'a') as fds:
+                fds.write('machine ' + os.environ['CI_SERVER_HOST'] + '\n'
+                          'login gitlab-ci-token\n'
+                          'password ' + os.environ['CI_JOB_TOKEN'] + '\n')
+
     def _setup_aws_creds(self):
         aws_dir = self.tmpdirname + "/.aws"
         conf_file = aws_dir + "/config"
         shared_creds_file = aws_dir + "/credentials"
         os.makedirs(aws_dir)
         if os.environ.get('AWS_CONFIG_FILE') \
                 and os.environ.get('AWS_SHARED_CREDENTIALS_FILE'):
@@ -219,39 +230,31 @@
         if gitconfig_host and os.path.exists(gitconfig_host):
             shutil.copy(gitconfig_host, gitconfig_kas)
 
         with GitConfigParser(gitconfig_kas, read_only=False) as config:
             # overwrite user as kas operates git
             config['user'] = {
                 'email': 'kas@example.com',
-                'name': 'Kas User'
+                'name': 'kas User'
             }
             if os.environ.get('GIT_CREDENTIAL_HELPER', False):
                 config['credential'] = {
                     'helper': os.environ.get('GIT_CREDENTIAL_HELPER')
                 }
                 if os.environ.get('GIT_CREDENTIAL_USEHTTPPATH', False):
                     config['credential']['useHttpPath'] = \
                         os.environ.get('GIT_CREDENTIAL_USEHTTPPATH')
             config.write()
 
     def execute(self, ctx):
-        if os.environ.get('NETRC_FILE', False):
-            shutil.copy(os.environ['NETRC_FILE'],
-                        self.tmpdirname + "/.netrc")
-        if os.environ.get('CI_SERVER_HOST', False) \
-                and os.environ.get('CI_JOB_TOKEN', False):
-            with open(self.tmpdirname + '/.netrc', 'a') as fds:
-                fds.write('\n# appended by kas, you have gitlab CI env\n')
-                fds.write('machine ' + os.environ['CI_SERVER_HOST'] + '\n'
-                          'login gitlab-ci-token\n'
-                          'password ' + os.environ['CI_JOB_TOKEN'] + '\n')
-
+        def_umask = os.umask(0o077)
+        self._setup_netrc()
         self._setup_gitconfig()
         self._setup_aws_creds()
+        os.umask(def_umask)
 
         ctx.environ['HOME'] = self.tmpdirname
 
 
 class SetupDir(Command):
     """
         Creates the build directory.
```

### Comparing `kas-4.3.1/kas/libkas.py` & `kas-4.3.2/kas/libkas.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/__init__.py` & `kas-4.3.2/kas/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/build.py` & `kas-4.3.2/kas/plugins/build.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/checkout.py` & `kas-4.3.2/kas/plugins/checkout.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/dump.py` & `kas-4.3.2/kas/plugins/dump.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/for_all_repos.py` & `kas-4.3.2/kas/plugins/for_all_repos.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/menu.py` & `kas-4.3.2/kas/plugins/menu.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/plugins/shell.py` & `kas-4.3.2/kas/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas/repos.py` & `kas-4.3.2/kas/repos.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
         return ['hg', 'log', '-r', self.commit or self.tag or self.branch
                 or self.refspec]
 
     def fetch_cmd(self):
         return ['hg', 'pull']
 
     def is_dirty_cmd(self):
-        return ['hg', 'diff']
+        return ['hg', 'status']
 
     def resolve_branch_cmd(self):
         if self.branch:
             return ['hg', 'identify', '--id', '-r',
                     f'limit(heads(branch({self.branch})))']
         else:
             return ['hg', 'identify', '--id', '-r', self.refspec]
```

### Comparing `kas-4.3.1/kas/schema-kas.json` & `kas-4.3.2/kas/schema-kas.json`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/kas-container` & `kas-4.3.2/kas-container`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 		if [ "$1" = "cleanall" ]; then
 			DL_DIR=${DL_DIR:-${KAS_BUILD_DIR}/downloads}
 			trace rm -rf "${DL_DIR}"
 		fi
 	fi
 }
 
-KAS_IMAGE_VERSION_DEFAULT="4.3.1"
+KAS_IMAGE_VERSION_DEFAULT="4.3.2"
 KAS_CONTAINER_IMAGE_PATH_DEFAULT="ghcr.io/siemens/kas"
 KAS_CONTAINER_IMAGE_NAME_DEFAULT="kas"
 KAS_CONTAINER_SELF_NAME="$(basename "$0")"
 
 set_container_image_var() {
 	KAS_IMAGE_VERSION="${KAS_IMAGE_VERSION:-${KAS_IMAGE_VERSION_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_NAME="${KAS_CONTAINER_IMAGE_NAME:-${KAS_CONTAINER_IMAGE_NAME_DEFAULT}}"
@@ -397,15 +397,15 @@
 	# on the host. This data is then added to the .config.yaml where it can
 	# be evaluated by the next invocation of kas-container.
 
 	if ! [ "$(realpath -qe "${KAS_REPO_DIR}")" = "$(realpath -qe "${KAS_WORK_DIR}")" ]; then
 		set -- "$@" -e _KAS_REPO_DIR_HOST="$(readlink -fv "${KAS_REPO_DIR}")"
 	fi
 
-	BUILD_SYSTEM=$(tr '\n' '\f' 2>/dev/null < ${KAS_FIRST_FILE} | \
+	BUILD_SYSTEM=$(tr '\n' '\f' 2>/dev/null < "${KAS_FIRST_FILE}" | \
 		sed -e 's/\(.*\fconfig KAS_BUILD_SYSTEM\f\(.*\)\|.*\)/\2/' \
 		    -e 's/\f\([[:alpha:]].*\|$\)//' \
 		    -e 's/.*default \"\(.*\)\".*/\1/')
 else
 	if [ -z "${KAS_FIRST_FILE}" ]; then
 		KAS_FIRST_FILE="${KAS_WORK_DIR}/.config.yaml"
 	fi
@@ -435,15 +435,15 @@
 
 if [ "$(id -u)" -eq 0 ] && [ "${KAS_ALLOW_ROOT}" != "yes" ] ; then
 	fatal_error "Running as root - may break certain recipes." \
 	            "Better give a regular user docker access. Set" \
 	            "KAS_ALLOW_ROOT=yes to override."
 fi
 
-set -- "$@" -v "${KAS_REPO_DIR}":/repo:${KAS_REPO_MOUNT_OPT} \
+set -- "$@" -v "${KAS_REPO_DIR}:/repo:${KAS_REPO_MOUNT_OPT}" \
 	-v "${KAS_WORK_DIR}":/work:rw -e KAS_WORK_DIR=/work \
 	-v "${KAS_BUILD_DIR}":/build:rw \
 	--workdir=/repo \
 	-e KAS_BUILD_DIR=/build \
 	-e USER_ID="$(id -u)" -e GROUP_ID="$(id -g)" --rm --init
 
 if [ -n "${KAS_SSH_DIR}" ] ; then
@@ -583,8 +583,9 @@
 while [ $KAS_EXTRA_BITBAKE_ARGS -gt 0 ]; do
 	arg="$1"
 	shift 1
 	set -- "$@" "$arg"
 	KAS_EXTRA_BITBAKE_ARGS=$((KAS_EXTRA_BITBAKE_ARGS - 1))
 done
 
+# shellcheck disable=SC2086
 trace ${KAS_CONTAINER_COMMAND} run "$@"
```

### Comparing `kas-4.3.1/kas.egg-info/PKG-INFO` & `kas-4.3.2/kas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 4.3.1
+Version: 4.3.2
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
 Download-URL: https://github.com/siemens/kas/archive/{__version__}.tar.gz
 Description: Setup tool for bitbake based projects
```

### Comparing `kas-4.3.1/kas.egg-info/SOURCES.txt` & `kas-4.3.2/kas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kas-4.3.1/setup.py` & `kas-4.3.2/setup.py`

 * *Files identical despite different names*

