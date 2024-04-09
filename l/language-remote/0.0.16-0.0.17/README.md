# Comparing `tmp/language-remote-0.0.16.tar.gz` & `tmp/language-remote-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language-remote-0.0.16.tar", last modified: Sat Apr  6 07:57:08 2024, max compression
+gzip compressed data, was "language-remote-0.0.17.tar", last modified: Tue Apr  9 18:09:00 2024, max compression
```

## Comparing `language-remote-0.0.16.tar` & `language-remote-0.0.17.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 07:57:07.995146 language-remote-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-06 07:56:49.000000 language-remote-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/language_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/language_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 07:56:49.000000 language-remote-0.0.16/language_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-06 07:56:49.000000 language-remote-0.0.16/language_remote/src/lang_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-06 07:56:49.000000 language-remote-0.0.16/language_remote/src/language_code_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/language_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-06 07:56:49.000000 language-remote-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:57:07.999146 language-remote-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-06 07:56:49.000000 language-remote-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:09:00.221515 language-remote-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 18:09:00.221515 language-remote-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-09 18:08:46.000000 language-remote-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:09:00.217514 language-remote-0.0.17/language_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:09:00.217514 language-remote-0.0.17/language_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 18:08:46.000000 language-remote-0.0.17/language_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-09 18:08:46.000000 language-remote-0.0.17/language_remote/src/lang_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-09 18:08:46.000000 language-remote-0.0.17/language_remote/src/language_code_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:09:00.217514 language-remote-0.0.17/language_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 18:09:00.000000 language-remote-0.0.17/language_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-09 18:09:00.000000 language-remote-0.0.17/language_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:09:00.000000 language-remote-0.0.17/language_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:09:00.000000 language-remote-0.0.17/language_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 18:09:00.000000 language-remote-0.0.17/language_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 18:08:46.000000 language-remote-0.0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:09:00.221515 language-remote-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 18:08:46.000000 language-remote-0.0.17/setup.py
```

### Comparing `language-remote-0.0.16/README.md` & `language-remote-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `language-remote-0.0.16/language_remote/src/lang_code.py` & `language-remote-0.0.17/language_remote/src/lang_code.py`

 * *Files 13% similar despite different names*

```diff
@@ -294,7 +294,33 @@
         MiniLogger.start(message=DETECT_LANG_CODE_METHOD_NAME, object={"text": text, "attempts": attempts})
         lang_code_str = LangCode.detect_lang_code_str(text, attempts)
         if lang_code_str is None:
             MiniLogger.end(message=DETECT_LANG_CODE_METHOD_NAME, object={"result": None})
             return None
         MiniLogger.end(message=DETECT_LANG_CODE_METHOD_NAME, object={"result": lang_code_str})
         return LangCode(lang_code_str)
+
+    @staticmethod
+    def detect_lang_code_restricted(text: str, allowed_lang_codes: list[str], attempts=3, 
+                                    default_lang_code: 'LangCode' = None) -> 'LangCode':
+        DETECT_LANG_CODE_RESTRICTED_METHOD_NAME = 'detect_lang_code_restricted'
+        MiniLogger.start(message=DETECT_LANG_CODE_RESTRICTED_METHOD_NAME,
+                         object={"text": text, "allowed_lang_codes": allowed_lang_codes, "attempts": attempts})
+        lang_code_str = LangCode.detect_lang_code_str(text, attempts)
+        if lang_code_str in allowed_lang_codes:
+            MiniLogger.end(message=DETECT_LANG_CODE_RESTRICTED_METHOD_NAME, object={"result": lang_code_str})
+            return LangCode(lang_code_str)
+        MiniLogger.end(message=DETECT_LANG_CODE_RESTRICTED_METHOD_NAME, object={"result": None})
+        return default_lang_code
+
+    @staticmethod
+    def detect_lang_code_str_restricted(text: str, allowed_lang_codes: list[str], attempts=3,
+                                        default_lang_code: str = None) -> str:
+        DETECT_LANG_CODE_STR_RESTRICTED_METHOD_NAME = 'detect_lang_code_str_restricted'
+        MiniLogger.start(message=DETECT_LANG_CODE_STR_RESTRICTED_METHOD_NAME,
+                         object={"text": text, "allowed_lang_codes": allowed_lang_codes, "attempts": attempts})
+        lang_code_str = LangCode.detect_lang_code_str(text, attempts)
+        if lang_code_str in allowed_lang_codes:
+            MiniLogger.end(message=DETECT_LANG_CODE_STR_RESTRICTED_METHOD_NAME, object={"result": lang_code_str})
+            return lang_code_str
+        MiniLogger.end(message=DETECT_LANG_CODE_STR_RESTRICTED_METHOD_NAME, object={"result": default_lang_code})
+        return default_lang_code
```

### Comparing `language-remote-0.0.16/language_remote/src/language_code_constants.py` & `language-remote-0.0.17/language_remote/src/language_code_constants.py`

 * *Files identical despite different names*

### Comparing `language-remote-0.0.16/setup.py` & `language-remote-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "language-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/language-remote
-    version='0.0.16',
+    version='0.0.17',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     #long_description=readme,
```

