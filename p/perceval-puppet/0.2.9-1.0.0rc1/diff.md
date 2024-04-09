# Comparing `tmp/perceval_puppet-0.2.9.tar.gz` & `tmp/perceval_puppet-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_puppet-0.2.9.tar", max compression
+gzip compressed data, was "perceval_puppet-1.0.0rc1.tar", max compression
```

## Comparing `perceval_puppet-0.2.9.tar` & `perceval_puppet-1.0.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       50 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/LICENSE
--rw-r--r--   0        0        0      972 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/NEWS
--rw-r--r--   0        0        0     2197 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/README.md
--rw-r--r--   0        0        0        0 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/perceval/backends/puppet/__init__.py
--rw-r--r--   0        0        0       86 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/perceval/backends/puppet/_version.py
--rw-r--r--   0        0        0    10849 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/perceval/backends/puppet/puppetforge.py
--rw-r--r--   0        0        0     1397 2023-04-26 14:45:33.189992 perceval_puppet-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0     1888 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/base.py
--rw-r--r--   0        0        0      192 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_empty.json
--rw-r--r--   0        0        0    15963 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_modules.json
--rw-r--r--   0        0        0     1028 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_modules_next.json
--rw-r--r--   0        0        0    22968 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_releases_ceph.json
--rw-r--r--   0        0        0     1810 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_releases_nomad.json
--rw-r--r--   0        0        0      318 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_user_norisnetwork.json
--rw-r--r--   0        0        0      302 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_user_sshuyskiy.json
--rwxr-xr-x   0        0        0     1017 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/run_tests.py
--rw-r--r--   0        0        0    18656 2023-04-26 14:45:33.193992 perceval_puppet-0.2.9/tests/test_puppetforge.py
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 perceval_puppet-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      126 2024-04-09 16:15:19.396988 perceval_puppet-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2505 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0     2197 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/perceval/backends/puppet/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/perceval/backends/puppet/_version.py
+-rw-r--r--   0        0        0    10849 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/perceval/backends/puppet/puppetforge.py
+-rw-r--r--   0        0        0     1415 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1888 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/base.py
+-rw-r--r--   0        0        0      192 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_empty.json
+-rw-r--r--   0        0        0    15963 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_modules.json
+-rw-r--r--   0        0        0     1028 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_modules_next.json
+-rw-r--r--   0        0        0    22968 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_releases_ceph.json
+-rw-r--r--   0        0        0     1810 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_releases_nomad.json
+-rw-r--r--   0        0        0      318 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_user_norisnetwork.json
+-rw-r--r--   0        0        0      302 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_user_sshuyskiy.json
+-rwxr-xr-x   0        0        0     1017 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    18656 2024-04-09 16:15:19.400988 perceval_puppet-1.0.0rc1/tests/test_puppetforge.py
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 perceval_puppet-1.0.0rc1/PKG-INFO
```

### Comparing `perceval_puppet-0.2.9/LICENSE` & `perceval_puppet-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/NEWS` & `perceval_puppet-1.0.0rc1/NEWS`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,78 @@
 # Releases
 
+  ## perceval-puppet 0.2.25 - (2024-03-27)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.24 - (2024-03-12)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.23 - (2024-03-01)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.22 - (2024-02-08)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.21 - (2024-01-30)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.20 - (2023-12-19)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.19 - (2023-11-28)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.18 - (2023-11-14)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.17 - (2023-11-03)
+  
+  * Update Poetry's package dependencies
+
+## perceval-puppet 0.2.16 - (2023-10-20)
+
+**Dependencies updateds:**
+
+ * Add Python 3.10 and 3.11 and drop 3.7 support\
+   Python 3.7 reached the end of life phase on June 27 2023 and is no
+   longer supported.
+
+
+  ## perceval-puppet 0.2.15 - (2023-08-06)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.14 - (2023-07-23)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.13 - (2023-07-11)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.12 - (2023-06-28)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.11 - (2023-05-17)
+  
+  * Update Poetry's package dependencies
+
+  ## perceval-puppet 0.2.10 - (2023-04-27)
+  
+  * Update Poetry's package dependencies
+
   ## perceval-puppet 0.2.9 - (2023-04-26)
   
   * Update Poetry's package dependencies
 
   ## perceval-puppet 0.2.8 - (2023-04-21)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_puppet-0.2.9/README.md` & `perceval_puppet-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 The backends currently managed by this package support the next repositories:
 
 * Puppet Forge
 
 ## Requirements
 
- * Python >= 3.7
+ * Python >= 3.8
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 ## Installation
 
 There are several ways to install perceval-puppet on your system: packages or source
```

### Comparing `perceval_puppet-0.2.9/perceval/backends/puppet/puppetforge.py` & `perceval_puppet-1.0.0rc1/perceval/backends/puppet/puppetforge.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     the Puppet's forge.
 
     :param max_items: maximum number of items requested on the same query
     :param tag: label used to mark the data
     :param archive: archive to store/retrieve data
     :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.6.0'
+    version = '1.0.0'
 
     CATEGORIES = [CATEGORY_MODULE]
     EXTRA_SEARCH_FIELDS = {
         'module_group': ['module_group'],
         'slug': ['slug']
     }
```

### Comparing `perceval_puppet-0.2.9/pyproject.toml` & `perceval_puppet-1.0.0rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-puppet"
-version = "0.2.9"
+version = "1.0.0-rc.1"
 description = "Bundle of Perceval backends for Puppet, Inc. ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -25,27 +25,27 @@
 include = [
     { path = "AUTHORS", format = "sdist" },
     { path = "NEWS", format = "sdist" },
     { path = "README.md", format = "sdist" },
 ]
 
 classifiers = [
-   "Development Status :: 4 - Beta",
+   "Development Status :: 5 - Production/Stable",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Topic :: Software Development",
    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
    "Programming Language :: Python :: 3"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/chaoss/grimoirelab-perceval-puppet/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 requests = "^2.7.0"
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
 perceval = { version = ">=0.19", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 httpretty = "1.0.2"
```

### Comparing `perceval_puppet-0.2.9/tests/base.py` & `perceval_puppet-1.0.0rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_modules.json` & `perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_modules.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_modules_next.json` & `perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_modules_next.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_releases_ceph.json` & `perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_releases_ceph.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/tests/data/puppetforge/puppetforge_releases_nomad.json` & `perceval_puppet-1.0.0rc1/tests/data/puppetforge/puppetforge_releases_nomad.json`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/tests/run_tests.py` & `perceval_puppet-1.0.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/tests/test_puppetforge.py` & `perceval_puppet-1.0.0rc1/tests/test_puppetforge.py`

 * *Files identical despite different names*

### Comparing `perceval_puppet-0.2.9/PKG-INFO` & `perceval_puppet-1.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: perceval-puppet
-Version: 0.2.9
+Version: 1.0.0rc1
 Summary: Bundle of Perceval backends for Puppet, Inc. ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Requires-Dist: grimoirelab-toolkit (>=0.3)
 Requires-Dist: perceval (>=0.19)
 Requires-Dist: requests (>=2.7.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-perceval-puppet/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-perceval-puppet
 Description-Content-Type: text/markdown
@@ -34,15 +32,15 @@
 
 The backends currently managed by this package support the next repositories:
 
 * Puppet Forge
 
 ## Requirements
 
- * Python >= 3.7
+ * Python >= 3.8
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 ## Installation
 
 There are several ways to install perceval-puppet on your system: packages or source
```

