# Comparing `tmp/py400-0.1.tar.gz` & `tmp/py400-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py400-0.1.tar", last modified: Mon Mar  4 14:52:58 2024, max compression
+gzip compressed data, was "py400-0.2.0.tar", last modified: Tue Apr  9 08:57:47 2024, max compression
```

## Comparing `py400-0.1.tar` & `py400-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 14:52:58.525361 py400-0.1/
--rw-rw-rw-   0        0        0      190 2024-03-04 14:52:58.521245 py400-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-01 13:34:43.000000 py400-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-04 14:52:58.508012 py400-0.1/py400/
--rw-rw-rw-   0        0        0    21661 2024-03-04 14:39:54.000000 py400-0.1/py400/AS400.py
--rw-rw-rw-   0        0        0       19 2024-03-04 14:41:05.000000 py400-0.1/py400/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 14:52:58.520746 py400-0.1/py400.egg-info/
--rw-rw-rw-   0        0        0      190 2024-03-04 14:52:58.000000 py400-0.1/py400.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-03-04 14:52:58.000000 py400-0.1/py400.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 14:52:58.000000 py400-0.1/py400.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-03-04 14:52:58.000000 py400-0.1/py400.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-04 14:52:58.000000 py400-0.1/py400.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-04 14:52:58.525361 py400-0.1/setup.cfg
--rw-rw-rw-   0        0        0      403 2024-03-04 14:41:53.000000 py400-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:57:47.889886 py400-0.2.0/
+-rw-rw-rw-   0        0        0      192 2024-04-09 08:57:47.889280 py400-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-01 13:34:43.000000 py400-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 08:57:47.862305 py400-0.2.0/py400/
+-rw-rw-rw-   0        0        0    21735 2024-04-09 08:51:14.000000 py400-0.2.0/py400/AS400.py
+-rw-rw-rw-   0        0        0       19 2024-03-04 15:09:28.000000 py400-0.2.0/py400/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 08:57:47.888286 py400-0.2.0/py400.egg-info/
+-rw-rw-rw-   0        0        0      192 2024-04-09 08:57:47.000000 py400-0.2.0/py400.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-09 08:57:47.000000 py400-0.2.0/py400.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 08:57:47.000000 py400-0.2.0/py400.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-09 08:57:47.000000 py400-0.2.0/py400.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-09 08:57:47.000000 py400-0.2.0/py400.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 08:57:47.890922 py400-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      405 2024-04-09 08:55:04.000000 py400-0.2.0/setup.py
```

### Comparing `py400-0.1/py400/AS400.py` & `py400-0.2.0/py400/AS400.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,16 +331,16 @@
 
             for failedJob in result:
                 failedJob["TIME_STAMP"] = str(failedJob["TIME_STAMP"])
 
         self.itool.clear()
         return result
 
-    def getUsers(self, debug: bool = False):
-        self.itool.add(iSqlPrepare('UsersGet', """
+    def getUsers(self, limit: int = None, offset: int = 0, debug: bool = False):
+        self.itool.add(iSqlPrepare('UsersGet', f"""
 SELECT *
     FROM (
             SELECT
                    CASE GROUP_ID_NUMBER
                        WHEN 0 THEN 'USER'
                        ELSE 'GROUP'
                    END AS PROFILE_TYPE,
@@ -424,15 +424,15 @@
                    DAYS_USED_COUNT,
                    LAST_RESET_TIMESTAMP,
                    AUTHORITY_COLLECTION_ACTIVE,
                    AUTHORITY_COLLECTION_REPOSITORY_EXISTS,
                    PASE_SHELL_PATH
                 FROM QSYS2.USER_INFO
         )
-        LIMIT 2 OFFSET 0
+        {f"LIMIT {limit} OFFSET {offset}" if limit else None}
 """, {"error": "on" if debug else "fast"}))
 
         self.itool.add(
             iSqlExecute('exec', {"error": "on" if debug else "fast"})
         )
 
         self.itool.add(
```

