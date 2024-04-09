# Comparing `tmp/dcx-0.78.0.tar.gz` & `tmp/dcx-0.79.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcx-0.78.0.tar", last modified: Mon Apr  8 16:40:34 2024, max compression
+gzip compressed data, was "dcx-0.79.0.tar", last modified: Tue Apr  9 09:27:31 2024, max compression
```

## Comparing `dcx-0.78.0.tar` & `dcx-0.79.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.468639 dcx-0.78.0/
--rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.78.0/LICENSE
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:40:34.468436 dcx-0.78.0/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.78.0/README.md
--rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-08 16:40:32.000000 dcx-0.78.0/pyproject.toml
--rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-08 16:40:34.468682 dcx-0.78.0/setup.cfg
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.466132 dcx-0.78.0/src/
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.466904 dcx-0.78.0/src/dcx/
--rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.78.0/src/dcx/__init__.py
--rw-r--r--   0 robertdegen   (501) staff       (20)    65084 2024-04-08 16:40:29.000000 dcx-0.78.0/src/dcx/__main__.py
-drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-08 16:40:34.468259 dcx-0.78.0/src/dcx.egg-info/
--rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/PKG-INFO
--rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/SOURCES.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/dependency_links.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/requires.txt
--rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-08 16:40:34.000000 dcx-0.78.0/src/dcx.egg-info/top_level.txt
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.673124 dcx-0.79.0/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        5 2024-02-16 09:45:07.000000 dcx-0.79.0/LICENSE
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-09 09:27:31.672950 dcx-0.79.0/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      159 2024-02-25 22:16:23.000000 dcx-0.79.0/README.md
+-rw-r--r--   0 robertdegen   (501) staff       (20)      716 2024-04-09 09:27:29.000000 dcx-0.79.0/pyproject.toml
+-rw-r--r--   0 robertdegen   (501) staff       (20)       38 2024-04-09 09:27:31.673298 dcx-0.79.0/setup.cfg
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.670333 dcx-0.79.0/src/
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.671119 dcx-0.79.0/src/dcx/
+-rw-r--r--   0 robertdegen   (501) staff       (20)        0 2024-01-14 18:51:20.000000 dcx-0.79.0/src/dcx/__init__.py
+-rw-r--r--   0 robertdegen   (501) staff       (20)    66377 2024-04-09 09:27:20.000000 dcx-0.79.0/src/dcx/__main__.py
+drwxr-xr-x   0 robertdegen   (501) staff       (20)        0 2024-04-09 09:27:31.672650 dcx-0.79.0/src/dcx.egg-info/
+-rw-r--r--   0 robertdegen   (501) staff       (20)      850 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/PKG-INFO
+-rw-r--r--   0 robertdegen   (501) staff       (20)      226 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        1 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)       83 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/requires.txt
+-rw-r--r--   0 robertdegen   (501) staff       (20)        4 2024-04-09 09:27:31.000000 dcx-0.79.0/src/dcx.egg-info/top_level.txt
```

### Comparing `dcx-0.78.0/PKG-INFO` & `dcx-0.79.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.78.0
+Version: 0.79.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcx-0.78.0/pyproject.toml` & `dcx-0.79.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcx"
-version = "0.78.0"
+version = "0.79.0"
 authors = [
   { name="Robert Degen", email="turbodev@mailbox.org" },
 ]
 description = "Minimalistic selenium wrapper"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dcx-0.78.0/src/dcx/__main__.py` & `dcx-0.79.0/src/dcx/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -706,14 +706,38 @@
                 if play_part[1] == "save_profile": ###ntcommand
                     save_profile_name = play_part[2]
                     profiledir_actual = driver.caps["moz:profile"]
                     shutil.make_archive(save_profile_name, "zip", profiledir_actual)
                     #shutil.copyfile(os.path.join(profiledir_actual, "cookies.sqlite"), "cookies.sqlite")
                     #print(profiledir_actual)
                     unknown_command=False
+
+                if play_part[1] == "ready": ###ntcommand
+                    # wait for document.readyState === 'complete'
+                    ready_ttl_secs = default_wait
+
+                    logging.info("Waiting for document.readyState to be complete (max wait secs = %d)..." % ready_ttl_secs)
+
+                    while ready_ttl_secs > 0:
+                        the_document_readystate = driver.execute_script("return document.readyState === 'complete';")
+                        if type(the_document_readystate) is bool:
+                            if the_document_readystate == True:
+                                logging.info("READY")
+                                break
+                            else:
+                                ready_ttl_secs -= 1
+                                logging.info("Not yet ready, waiting 1 sec before re-check...")
+                                time.sleep(1)
+                        else:
+                            raise Exception("Error, document.readyState === 'complete' didn't return bool.")
+                    
+                    if ready_ttl_secs <= 0:                    
+                        raise Exception("document.readyState never reached complete state")
+                    
+                    unknown_command=False
                 
                 if play_part[1] == "save_cookies": ###ntcommand
                     cookies_dump_name = play_part[2]
                     pwd_cookies = None
                     try:
                         pwd_cookies = play_part[3]
                     except:
```

### Comparing `dcx-0.78.0/src/dcx.egg-info/PKG-INFO` & `dcx-0.79.0/src/dcx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcx
-Version: 0.78.0
+Version: 0.79.0
 Summary: Minimalistic selenium wrapper
 Author-email: Robert Degen <turbodev@mailbox.org>
 Project-URL: Homepage, https://github.com/turbo-bert/dcx
 Project-URL: Issues, https://github.com/turbo-bert/dcx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

