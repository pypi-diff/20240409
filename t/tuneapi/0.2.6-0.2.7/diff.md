# Comparing `tmp/tuneapi-0.2.6.tar.gz` & `tmp/tuneapi-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.6.tar", max compression
+gzip compressed data, was "tuneapi-0.2.7.tar", max compression
```

## Comparing `tuneapi-0.2.6.tar` & `tuneapi-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.6/README.md
--rw-r--r--   0        0        0      696 2024-04-07 20:01:39.573357 tuneapi-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-07 20:01:39.573422 tuneapi-0.2.6/tuneapi/__init__.py
--rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.6/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6703 2024-04-05 08:55:18.981956 tuneapi-0.2.6/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.6/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.6/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0      712 2024-04-07 06:28:34.060373 tuneapi-0.2.6/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.6/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.6/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1032 2024-04-07 05:56:12.541307 tuneapi-0.2.6/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.6/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.6/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.6/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.6/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.2.6/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.6/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.6/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.6/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.2.6/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.6/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.6/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.7/README.md
+-rw-r--r--   0        0        0      696 2024-04-09 05:56:27.169497 tuneapi-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-09 05:56:19.006229 tuneapi-0.2.7/tuneapi/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.7/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6712 2024-04-09 05:54:45.329815 tuneapi-0.2.7/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.7/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.7/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0      659 2024-04-07 20:07:56.771955 tuneapi-0.2.7/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.7/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.7/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1032 2024-04-07 05:56:12.541307 tuneapi-0.2.7/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.7/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.7/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.7/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.7/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.2.7/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.7/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.7/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.7/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.2.7/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.7/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.7/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.7/PKG-INFO
```

### Comparing `tuneapi-0.2.6/pyproject.toml` & `tuneapi-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.6"
+version = "0.2.7"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.2.6/tuneapi/apis/model_anthropic.py` & `tuneapi-0.2.7/tuneapi/apis/model_anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,15 @@
                                         {"delta": {"content": resp["delta"]["text"]}}
                                     ]
                                 },
                                 tight=True,
                             )
                         ).encode()
                 except:
-                    yield line
+                    yield line.encode()
                 continue
 
             # return token
             try:
                 resp = json.loads(line.replace("data:", "").strip())
                 if "delta" in resp:
                     yield resp["delta"]["text"]
```

### Comparing `tuneapi-0.2.6/tuneapi/apis/model_openai.py` & `tuneapi-0.2.7/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/apis/model_tune.py` & `tuneapi-0.2.7/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/apis/threads.py` & `tuneapi-0.2.7/tuneapi/apis/threads.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,10 +15,9 @@
         tune_org_id: Optional[str] = None,
         tune_api_key: Optional[str] = None,
     ):
         tune_api_key = tune_api_key or ENV.TUNE_API_KEY()
         tune_org_id = tune_org_id or ENV.TUNE_ORG_ID("")
         headers = {"x-tune-key": tune_api_key}
 
-        # "nbx_wwS8ZZnre62dhyZ5cOU0SWUHe01jfiWKPrl",
         if tune_org_id:
             headers["X-Organization-Id"] = tune_org_id
```

### Comparing `tuneapi-0.2.6/tuneapi/types/chats.py` & `tuneapi-0.2.7/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/__init__.py` & `tuneapi-0.2.7/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/fs.py` & `tuneapi-0.2.7/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/logger.py` & `tuneapi-0.2.7/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/mime.py` & `tuneapi-0.2.7/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/misc.py` & `tuneapi-0.2.7/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/networking.py` & `tuneapi-0.2.7/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/parallel.py` & `tuneapi-0.2.7/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/serdeser.py` & `tuneapi-0.2.7/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/subway.py` & `tuneapi-0.2.7/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/tuneapi/utils/terminal.py` & `tuneapi-0.2.7/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.6/PKG-INFO` & `tuneapi-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: Apache 2.0
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

