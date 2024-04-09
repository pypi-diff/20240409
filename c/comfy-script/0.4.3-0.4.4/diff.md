# Comparing `tmp/comfy_script-0.4.3.tar.gz` & `tmp/comfy_script-0.4.4.tar.gz`

## Comparing `comfy_script-0.4.3.tar` & `comfy_script-0.4.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.3/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.3/requirements.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.3/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.3/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/astutil.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    42190 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.3/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.3/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.3/LICENSE.txt
--rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 comfy_script-0.4.3/README.md
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 comfy_script-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    15825 2020-02-02 00:00:00.000000 comfy_script-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.4.4/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.4.4/requirements.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.4.4/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Latent/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Models/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.4.4/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    42450 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20430 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.4.4/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.4.4/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.4.4/LICENSE.txt
+-rw-r--r--   0        0        0    14265 2020-02-02 00:00:00.000000 comfy_script-0.4.4/README.md
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 comfy_script-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    15864 2020-02-02 00:00:00.000000 comfy_script-0.4.4/PKG-INFO
```

### Comparing `comfy_script-0.4.3/__init__.py` & `comfy_script-0.4.4/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/README.md` & `comfy_script-0.4.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/Runtime.md` & `comfy_script-0.4.4/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/Image/README.md` & `comfy_script-0.4.4/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/Latent/README.md` & `comfy_script-0.4.4/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/Nodes/README.md` & `comfy_script-0.4.4/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/auto-queue.png` & `comfy_script-0.4.4/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/diff.png` & `comfy_script-0.4.4/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/plot.png` & `comfy_script-0.4.4/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/select.png` & `comfy_script-0.4.4/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/type-stubs.png` & `comfy_script-0.4.4/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/type-stubs2.png` & `comfy_script-0.4.4/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/workflow.png` & `comfy_script-0.4.4/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/README/workflow2.png` & `comfy_script-0.4.4/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/docs/images/Runtime/load-api-format.png` & `comfy_script-0.4.4/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/astutil.py` & `comfy_script-0.4.4/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/client/__init__.py` & `comfy_script-0.4.4/src/comfy_script/client/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,58 @@
+from __future__ import annotations
 import json
 import os
 from pathlib import PurePath
 import sys
 import traceback
+from typing import Callable
 
 import asyncio
 import nest_asyncio
 import aiohttp
+from yarl import URL
 
 nest_asyncio.apply()
 
-endpoint = 'http://127.0.0.1:8188/'
+client: Client | None = None
+'''The global client object.'''
 
-def set_endpoint(api_endpoint: str):
-    global endpoint
-    if not api_endpoint.startswith('http://'):
-        api_endpoint = 'http://' + api_endpoint
-    if not api_endpoint.endswith('/'):
-        api_endpoint += '/'
-    endpoint = api_endpoint
+class Client:
+    def __init__(
+        self,
+        base_url: str | URL = 'http://127.0.0.1:8188/',
+        *,
+        session_factory: Callable[[], aiohttp.ClientSession] = aiohttp.ClientSession
+    ):
+        '''
+        - `base_url`: The base URL of the ComfyUI server API.
+
+          e.g. `'http://127.0.0.1:8188/'`
+
+        - `session_factory`: A callable factory that returns a new [`aiohttp.ClientSession`](https://docs.aiohttp.org/en/latest/client_reference.html#aiohttp.ClientSession) object. 
+
+          e.g. `lambda: aiohttp.ClientSession(auth=aiohttp.BasicAuth('Aladdin', 'open sesame'))`
+        '''
+        if base_url is None:
+            base_url = 'http://127.0.0.1:8188/'
+        elif not isinstance(base_url, str):
+            base_url = str(base_url)
+        
+        if not base_url.startswith('http://'):
+            base_url = 'http://' + base_url
+        if not base_url.endswith('/'):
+            base_url += '/'
+        self.base_url = base_url
+
+        # Do not pass base_url to ClientSession, as it only supports absolute URLs without path part
+        self._session_factory = session_factory
+    
+    def session(self) -> aiohttp.ClientSession:
+        '''Because `aiohttp.ClientSession` is not event-loop-safe (thread-safe), a new session should be created for each request to avoid potential issues. Also, `aiohttp.ClientSession` cannot be closed in a sync manner.'''
+        return self._session_factory()
 
 async def response_to_str(response: aiohttp.ClientResponse) -> str:
     try:
         msg = json.dumps(await response.json(), indent=2)
     except Exception as e:
         msg = str(e)
     return f'{response}{msg}'
@@ -60,34 +90,34 @@
             try:
                 out[x] = node_info(x)
             except Exception as e:
                 print(f"[ERROR] An error occurred while retrieving information for the '{x}' node.", file=sys.stderr)
                 traceback.print_exc()
         return out
 
-    async with aiohttp.ClientSession() as session:
-    # http://127.0.0.1:8188/object_info
-        async with session.get(f'{endpoint}object_info') as response:
+    async with client.session() as session:
+        # http://127.0.0.1:8188/object_info
+        async with session.get(f'{client.base_url}object_info') as response:
             if response.status == 200:
                 return await response.json()
             else:
                 raise Exception(f'ComfyScript: Failed to get nodes info: {await response_to_str(response)}')
 
 def get_nodes_info() -> dict:
     return asyncio.run(_get_nodes_info())
 
 async def _get_embeddings() -> list[str]:
     folder_paths = sys.modules.get('folder_paths')
     if folder_paths is not None and 'get_filename_list' in vars(folder_paths):
         embeddings = folder_paths.get_filename_list("embeddings")
         return list(map(lambda a: os.path.splitext(a)[0], embeddings))
     
-    async with aiohttp.ClientSession() as session:
-    # http://127.0.0.1:8188/embeddings
-        async with session.get(f'{endpoint}embeddings') as response:
+    async with client.session() as session:
+        # http://127.0.0.1:8188/embeddings
+        async with session.get(f'{client.base_url}embeddings') as response:
             if response.status == 200:
                 return await response.json()
             else:
                 raise Exception(f'ComfyScript: Failed to get embeddings: {await response_to_str(response)}')
 
 def get_embeddings() -> list[str]:
     return asyncio.run(_get_embeddings())
@@ -95,14 +125,14 @@
 class WorkflowJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if isinstance(o, PurePath):
             return str(o)
         return super().default(o)
 
 __all__ = [
-    'endpoint'
-    'set_endpoint',
+    'client',
+    'Client',
     '_get_nodes_info',
     'get_nodes_info',
     '_get_embeddings',
     'get_embeddings'
 ]
```

### Comparing `comfy_script-0.4.3/src/comfy_script/nodes/__init__.py` & `comfy_script-0.4.4/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/__init__.py` & `comfy_script-0.4.4/src/comfy_script/runtime/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,45 +13,47 @@
 import aiohttp
 
 nest_asyncio.apply()
 
 _client_id = str(uuid.uuid4())
 _save_script_source = True
 
-def load(comfyui: str | Path = None, args: ComfyUIArgs | None = None, vars: dict | None = None, watch: bool = True, save_script_source: bool = True):
+def load(comfyui: str | Client | Path = None, args: ComfyUIArgs | None = None, vars: dict | None = None, watch: bool = True, save_script_source: bool = True):
     '''
-    - `comfyui`: A URL of the ComfyUI server API, or a path to the ComfyUI directory, or `'comfyui'` to use the [`comfyui` package](https://github.com/comfyanonymous/ComfyUI/pull/298).
+    - `comfyui`: The base URL of the ComfyUI server API, or a `Client` object, or a path to the ComfyUI directory, or `'comfyui'` to use the [`comfyui` package](https://github.com/comfyanonymous/ComfyUI/pull/298).
 
       If not specified, the following ones will be tried in order:
       1. Local server API: http://127.0.0.1:8188/
       2. Parent ComfyUI directory: The default path is `ComfyScript/../..`, which only works if ComfyScript is installed at `ComfyUI/custom_nodes/ComfyScript`.
       3. `comfyui` package
     
     - `args`: CLI arguments to be passed to ComfyUI, if the value of `comfyui` is not an API. See `ComfyUIArgs` for details.
     '''
     asyncio.run(_load(comfyui, args, vars, watch, save_script_source))
 
-async def _load(comfyui: str | Path = None, args: ComfyUIArgs | None = None, vars: dict | None = None, watch: bool = True, save_script_source: bool = True):
+async def _load(comfyui: str | Client | Path = None, args: ComfyUIArgs | None = None, vars: dict | None = None, watch: bool = True, save_script_source: bool = True):
     global _save_script_source, queue
 
     _save_script_source = save_script_source
 
     nodes_info = None
     if comfyui is None:
         try:
             nodes_info = await client._get_nodes_info()
-            if comfyui_server != client.endpoint:
-                print(f'ComfyScript: Using ComfyUI from {client.endpoint}')
+            if comfyui_base_url != client.client.base_url:
+                print(f'ComfyScript: Using ComfyUI from {client.client.base_url}')
         except Exception as e:
             # To avoid "During handling of the above exception, another exception occurred"
             pass
         if nodes_info is None:
             start_comfyui(comfyui, args)
     elif isinstance(comfyui, str) and (comfyui.startswith('http://') or comfyui.startswith('https://')):
-        client.set_endpoint(comfyui)
+        client.client = client.Client(comfyui)
+    elif isinstance(comfyui, client.Client):
+        client.client = comfyui
     else:
         start_comfyui(comfyui, args)
     
     if nodes_info is None:
         nodes_info = await client._get_nodes_info()
     print(f'Nodes: {len(nodes_info)}')
 
@@ -151,15 +153,15 @@
                 raise TypeError(f'ComfyScript: Invalid argv type: {arg}')
         self.argv = list(argv)
 
     def to_argv(self) -> list[str]:
         return self.argv
 
 comfyui_started = False
-comfyui_server = None
+comfyui_base_url = None
 
 def start_comfyui(comfyui: Path | str = None, args: ComfyUIArgs | None = None, *, no_server: bool = False, join_at_exit: bool = True, autonomy: bool = False):
     '''
     Start ComfyUI. Immediately return if ComfyUI is already started.
 
     - `comfyui`: Path to ComfyUI directory.
     
@@ -171,19 +173,19 @@
 
     - `no_server`: Do not start the server.
 
     - `join_at_exit`: Join ComfyUI (wait for all tasks to be done) at process exit.
 
     - `autonomy`: If enabled, currently, the server will not be started even if `no_server=False`.
     '''
-    global comfyui_started, comfyui_server
-    if comfyui_started and (comfyui_server is not None or no_server):
+    global comfyui_started, comfyui_base_url
+    if comfyui_started and (comfyui_base_url is not None or no_server):
         return
     comfyui_started = False
-    comfyui_server = None
+    comfyui_base_url = None
     
     if comfyui is None:
         default_comfyui = Path(__file__).resolve().parents[5]
         if (default_comfyui / 'main.py').exists():
             comfyui = default_comfyui
         else:
             try:
@@ -341,16 +343,16 @@
             del main.exit
         
         asyncio.get_event_loop_policy().set_event_loop(original_loop)
         
         if not no_server:
             threading.Thread(target=main.server.loop.run_until_complete, args=(main.server.publish_loop(),), daemon=True).start()
 
-            comfyui_server = f'http://127.0.0.1:{main.args.port}/'
-            client.set_endpoint(comfyui_server)
+            comfyui_base_url = f'http://127.0.0.1:{main.args.port}/'
+            client.client = client.Client(comfyui_base_url)
     else:
         if comfyui != 'comfyui':
             print(f'ComfyScript: Importing ComfyUI from {comfyui}')
             sys.path.insert(0, str(comfyui))
             import main
         else:
             print(f'ComfyScript: Importing ComfyUI from comfyui package')
@@ -439,28 +441,28 @@
         self._queue_empty_callback = None
         self._queue_remaining_callbacks = [self._when_empty_callback]
         self._watch_display_node = None
         self._watch_display_task = None
         self.queue_remaining = 0
 
     async def _get_history(self, prompt_id: str) -> dict | None:
-        async with aiohttp.ClientSession() as session:
-            async with session.get(f'{client.endpoint}history/{prompt_id}') as response:
+        async with client.client.session() as session:
+            async with session.get(f'{client.client.base_url}history/{prompt_id}') as response:
                 if response.status == 200:
                     json = await response.json()
                     # print(json)
                     return json.get(prompt_id)
                 else:
                     print(f'ComfyScript: Failed to get history: {await client.response_to_str(response)}')
 
     async def _watch(self):
         while True:
             try:
-                async with aiohttp.ClientSession() as session:
-                    async with session.ws_connect(f'{client.endpoint}ws', params={'clientId': _client_id}) as ws:
+                async with client.client.session() as session:
+                    async with session.ws_connect(f'{client.client.base_url}ws', params={'clientId': _client_id}) as ws:
                         self.queue_remaining = 0
                         executing = False
                         async for msg in ws:
                             # print(msg.type)
                             if msg.type == aiohttp.WSMsgType.TEXT:
                                 msg = msg.json()
                                 # print(msg)
@@ -578,23 +580,23 @@
             prompt, id = Workflow(outputs=workflow)._get_prompt_and_id()
         elif isinstance(workflow, Workflow):
             prompt, id = workflow._get_prompt_and_id()
         else:
             raise TypeError(f'ComfyScript: Invalid workflow type: {workflow}')
         # print(prompt)
 
-        async with aiohttp.ClientSession() as session:
+        async with client.client.session() as session:
             extra_data = {}
             if _save_script_source:
                 extra_data = {
                     'extra_pnginfo': {
                         'ComfyScriptSource': source
                     }
                 }
-            async with session.post(f'{client.endpoint}prompt', json={
+            async with session.post(f'{client.client.base_url}prompt', json={
                 'prompt': prompt,
                 'extra_data': extra_data,
                 'client_id': _client_id,
             }) as response:
                 if response.status == 200:
                     response = await response.json()
                     # print(response)
@@ -644,27 +646,27 @@
         if self.queue_remaining == 0:
             f()
 
     def cancel_current(self):
         '''Interrupt the current task'''
         return asyncio.run(self._cancel_current())
     async def _cancel_current(self):
-        async with aiohttp.ClientSession() as session:
-            async with session.post(f'{client.endpoint}interrupt', json={
+        async with client.client.session() as session:
+            async with session.post(f'{client.client.base_url}interrupt', json={
                 'client_id': _client_id,
             }) as response:
                 if response.status != 200:
                     print(f'ComfyScript: Failed to interrupt current task: {await client.response_to_str(response)}')
 
     def cancel_remaining(self):
         '''Clear the queue'''
         return asyncio.run(self._cancel_remaining())
     async def _cancel_remaining(self):
-        async with aiohttp.ClientSession() as session:
-            async with session.post(f'{client.endpoint}queue', json={
+        async with client.client.session() as session:
+            async with session.post(f'{client.client.base_url}queue', json={
                 'clear': True,
                 'client_id': _client_id,
             }) as response:
                 if response.status != 200:
                     print(f'ComfyScript: Failed to clear queue: {await client.response_to_str(response)}')
 
     def cancel_all(self):
@@ -750,16 +752,16 @@
     
     def wait_result(self, output: data.NodeOutput) -> data.Result | None:
         return asyncio.run(self.result(output))
 
     # def wait(self):
     #     return asyncio.run(self._wait())
     # async def _wait(self):
-    #     async with aiohttp.ClientSession() as session:
-    #         async with session.ws_connect(f'{client.endpoint}ws?clientId={_client_id}') as ws:
+    #     async with client.client.session() as session:
+    #         async with session.ws_connect(f'{client.client.base_url}ws?clientId={_client_id}') as ws:
     #             async for msg in ws:
     #                 if msg.type == aiohttp.WSMsgType.TEXT:
     #                     msg = msg.json()
     #                     # print(msg)
     #                     if msg['type'] == 'status':
     #                         data = msg['data']
     #                         if data['status']['exec_info']['queue_remaining'] == 0:
@@ -892,20 +894,22 @@
         outer = inspect.currentframe().f_back
         source = ''.join(inspect.findsource(outer)[0])
         asyncio.run(self._exit(source))
 
 queue = TaskQueue()
 
 from .. import client
+from ..client import Client
 from . import nodes
 from . import data
 from .data import *
 
 __all__ = [
     'load',
+    'Client',
     'ComfyUIArgs',
     'start_comfyui',
     'TaskQueue',
     'queue',
     'Task',
     'Workflow',
 ]
```

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/factory.py` & `comfy_script-0.4.4/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/nodes.py` & `comfy_script-0.4.4/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.4.4/src/comfy_script/runtime/data/Images.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import aiohttp
 
 from . import Result
 
 class ImageBatchResult(Result):
     # TODO: Lazy cell
     async def _get_image(self, image: dict) -> Image.Image | None:
-        async with aiohttp.ClientSession() as session:
-            async with session.get(f'{client.endpoint}view', params=image) as response:
+        async with client.client.session() as session:
+            async with session.get(f'{client.client.base_url}view', params=image) as response:
                 if response.status == 200:
                     return Image.open(io.BytesIO(await response.read()))
                 else:
                     print(f'ComfyScript: Failed to get image: {await client.response_to_str(response)}')
                     return
     
     def __await__(self) -> list[Image.Image | None]:
```

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.4.4/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.4.4/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.4.4/src/comfy_script/runtime/real/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/transpile/__init__.py` & `comfy_script-0.4.4/src/comfy_script/transpile/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class WorkflowToScriptTranspiler:
     def __init__(self, workflow: str | dict, api_endpoint: str = None):
         '''
         - `workflow`: Can be in web UI format or API format.
         '''
         if api_endpoint is not None:
-            client.set_endpoint(api_endpoint)
+            client.client = client.Client(api_endpoint)
         self.nodes_info = client.get_nodes_info()
 
         if isinstance(workflow, str):
             workflow = json.loads(workflow)
         if 'version' not in workflow:
             # print('Converting prompt to workflow...')
             from . import prompt
```

### Comparing `comfy_script-0.4.3/src/comfy_script/transpile/prompt.py` & `comfy_script-0.4.4/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.4.4/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.4.4/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/tests/test_astutil.py` & `comfy_script-0.4.4/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/tests/transpile/bypass.json` & `comfy_script-0.4.4/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/tests/transpile/default.json` & `comfy_script-0.4.4/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/tests/transpile/test_transpiler.py` & `comfy_script-0.4.4/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/.gitignore` & `comfy_script-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/LICENSE.txt` & `comfy_script-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/README.md` & `comfy_script-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.4.3/pyproject.toml` & `comfy_script-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.4.3"
+version = "0.4.4"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
@@ -19,14 +19,16 @@
 
 [project.optional-dependencies]
 # There is no mandatory dependencies
 
 client = [
   # Already required by ComfyUI
   "aiohttp",
+  # Used by aiohttp
+  "yarl",
 
   # 1.5.9: https://github.com/erdewit/nest_asyncio/issues/87
   "nest_asyncio ~= 1.0, >= 1.5.9",
 ]
 
 # Transpiler
 transpile = [
```

### Comparing `comfy_script-0.4.3/PKG-INFO` & `comfy_script-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Requires-Dist: comfy-script[cli]; extra == 'all'
 Requires-Dist: comfy-script[default]; extra == 'all'
 Provides-Extra: cli
 Requires-Dist: click~=8.1; extra == 'cli'
 Provides-Extra: client
 Requires-Dist: aiohttp; extra == 'client'
 Requires-Dist: nest-asyncio>=1.5.9,~=1.0; extra == 'client'
+Requires-Dist: yarl; extra == 'client'
 Provides-Extra: default
 Requires-Dist: comfy-script[jupyter]; extra == 'default'
 Requires-Dist: comfy-script[no-ui]; extra == 'default'
 Provides-Extra: jupyter
 Requires-Dist: ipywidgets~=8.1; extra == 'jupyter'
 Requires-Dist: pillow; extra == 'jupyter'
 Provides-Extra: no-ui
```

