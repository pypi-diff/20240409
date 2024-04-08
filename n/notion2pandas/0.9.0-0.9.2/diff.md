# Comparing `tmp/notion2pandas-0.9.0-py3-none-any.whl.zip` & `tmp/notion2pandas-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6030 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      260 b- defN 24-Apr-06 12:14 notion2pandas/__init__.py
--rw-rw-rw-  2.0 fat    19469 b- defN 24-Mar-31 23:54 notion2pandas/notion2pandas.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-06 13:25 notion2pandas-0.9.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      727 b- defN 24-Apr-06 13:25 notion2pandas-0.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-06 13:25 notion2pandas-0.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-06 13:25 notion2pandas-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      584 b- defN 24-Apr-06 13:25 notion2pandas-0.9.0.dist-info/RECORD
-7 files, 22237 bytes uncompressed, 4988 bytes compressed:  77.6%
+Zip file size: 8135 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      215 b- defN 24-Apr-07 22:52 notion2pandas/__init__.py
+-rw-rw-rw-  2.0 fat    19012 b- defN 24-Apr-08 22:05 notion2pandas/notion2pandas.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6587 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      585 b- defN 24-Apr-08 23:00 notion2pandas-0.9.2.dist-info/RECORD
+7 files, 27596 bytes uncompressed, 7093 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: notion2pandas/__init__.py
 Comment: 
 
 Filename: notion2pandas/notion2pandas.py
 Comment: 
 
-Filename: notion2pandas-0.9.0.dist-info/LICENSE
+Filename: notion2pandas-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: notion2pandas-0.9.0.dist-info/METADATA
+Filename: notion2pandas-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: notion2pandas-0.9.0.dist-info/WHEEL
+Filename: notion2pandas-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: notion2pandas-0.9.0.dist-info/top_level.txt
+Filename: notion2pandas-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: notion2pandas-0.9.0.dist-info/RECORD
+Filename: notion2pandas-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## notion2pandas/__init__.py

```diff
@@ -2,10 +2,9 @@
 Package notion2pandas.
 
 Notion Client extension to import notion Database into pandas Dataframe.
 """
 
 from .notion2pandas import Notion2PandasClient
 
-__version__ = "0.9.0"
+__version__ = "0.9.2"
 __author__ = 'Andrea Rosati'
-__credits__ = 'Argonne National Laboratory'
```

## notion2pandas/notion2pandas.py

```diff
@@ -1,21 +1,17 @@
 import time
 import json
 from functools import reduce
-import threading
 
 import pandas as pd
 
 from notion_client import Client, APIErrorCode, APIResponseError
 from notion_client.errors import HTTPResponseError, RequestTimeoutError
 from notion_client.helpers import collect_paginated_api
 
-lock = threading.Lock()
-first_notion_API_execution_TS = None
-
 
 class NotionMaxAttempsException(Exception):
     def __init__(self, m):
         self.message = m
 
     def __str__(self):
         return self.message
@@ -29,20 +25,26 @@
         callsLimitThreshold: .
         maxAttempsExecutoner: .
     """
 
     _ROW_HASH_KEY = 'Row_Hash'
     _ROW_PAGEID_KEY = 'PageID'
 
-    def __init__(self, token_notion, o_secondsToRetry=150):
-        super().__init__(auth=token_notion)
-        self.secondsToRetry = o_secondsToRetry
-        self.callsLimitThreshold = 2700
-        self.rateLimitThreshold = 900
-        self.maxAttempsExecutoner = 5
+    # It's not in the official documentation, but it seems there is a limit of 2700 API calls in 15 minutes.
+    # https://notionmastery.com/pushing-notion-to-the-limits/#rate-limits
+    # WIP
+    _RATE_LIMIT_THRESHOLD = 900 #60 * 15
+    _CALLS_LIMIT_THRESHOLD = 2700
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        self.secondsToRetry = kwargs['secondsToRetry'] if 'secondsToRetry' in kwargs else 150
+        self.maxAttempsExecutioner = kwargs['maxAttempsExecutioner'] if 'maxAttempsExecutioner' in kwargs else 5
+        
         self.read_only_columns = {"last_edited_time", "last_edited_time",
                                   "files", "created_time", "rollup", "unique_id", "last_edited_by",
                                   "button", "formula", "created_by"}
 
         self.title_read_write_lambdas = (lambda notion_property:
                                          notion_property.get('title')[
                                              0].get("plain_text")
@@ -166,33 +168,21 @@
                                           lambda row_value: {"people": list(map(lambda notion_people: {"id": notion_people, 'object': 'user'}, eval(row_value)))
                                                              if row_value != '' else []})
         
     """Since Notion has introduced limits on requests to their APIs (https://developers.notion.com/reference/request-limits), 
        this method can repeat the request to the Notion APIs at predefined time intervals
        until a result is obtained or if the maximum limit of attempts is reached."""
     def _notionExecutor(self, api_to_call, **kwargs):
-        attempts = 5
+        attempts = self.maxAttempsExecutioner
         current_calls = 0
         while (attempts > 0):
             try:
-                with lock:
-                    global first_notion_API_execution_TS
-                    if first_notion_API_execution_TS is None:
-                        first_notion_API_execution_TS = time.time()
-                    if current_calls == (self.callsLimitThreshold - 1):
-                        timeFromFirstCall = time.time() - first_notion_API_execution_TS
-                        if timeFromFirstCall < self.rateLimitThreshold:
-                            time.sleep(self.rateLimitThreshold -
-                                       timeFromFirstCall)
-                        first_notion_API_execution_TS = time.time()
-                        current_calls = 0
-
-                    result = api_to_call(**kwargs)
-                    current_calls += 1
-                    return result
+                result = api_to_call(**kwargs)
+                current_calls += 1
+                return result
             except HTTPResponseError as error:
                 print('Catched exception: ' + str(error))
                 attempts -= 1
                 if isinstance(error, APIResponseError):
                     print('Error code: ' + error.code)
                     if error.code != APIErrorCode.InternalServerError and error.code != APIErrorCode.ServiceUnavailable:
                         print(error)
@@ -264,15 +254,15 @@
                         (columns.get('properties').get(notion_property).get('name'),
                          columns.get('properties').get(notion_property).get('type')),
                         columns.get('properties')))
 
     def from_notion_DB_to_dataframe(self, database_ID, filter_params={}):
         results = self._notionExecutor(
             collect_paginated_api,
-            **{'function': self.databases.query, **{}, "database_id": database_ID})
+            **{'function': self.databases.query, **filter_params, "database_id": database_ID})
         database_data = []
         for result in results:
             prop_dict = {}
             for notion_property in result.get("properties"):
                 prop_dict[str(notion_property)] = self.__readValueFromNotion(
                     result.get("properties").get(notion_property))
             prop_dict[self._ROW_PAGEID_KEY] = result.get("id")
```

## Comparing `notion2pandas-0.9.0.dist-info/LICENSE` & `notion2pandas-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

