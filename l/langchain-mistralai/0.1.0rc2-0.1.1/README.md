# Comparing `tmp/langchain_mistralai-0.1.0rc2.tar.gz` & `tmp/langchain_mistralai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.0rc2.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.1.tar", max compression
```

## Comparing `langchain_mistralai-0.1.0rc2.tar` & `langchain_mistralai-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0     1336 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/README.md
--rw-r--r--   0        0        0      173 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    23923 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     5890 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2317 2024-03-23 19:25:26.231204 langchain_mistralai-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2244 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1336 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/README.md
+-rw-r--r--   0        0        0      173 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    24784 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     5961 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2391 2024-04-09 21:54:38.281129 langchain_mistralai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.1/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.0rc2/LICENSE` & `langchain_mistralai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.0rc2/README.md` & `langchain_mistralai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.0rc2/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.1/langchain_mistralai/chat_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 
 class ChatMistralAI(BaseChatModel):
     """A chat model that uses the MistralAI API."""
 
     client: httpx.Client = Field(default=None)  #: :meta private:
     async_client: httpx.AsyncClient = Field(default=None)  #: :meta private:
-    mistral_api_key: Optional[SecretStr] = None
+    mistral_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     endpoint: str = "https://api.mistral.ai/v1"
     max_retries: int = 5
     timeout: int = 120
     max_concurrent_requests: int = 64
 
     model: str = "mistral-small"
     temperature: float = 0.7
@@ -198,14 +198,20 @@
     top_p: float = 1
     """Decode using nucleus sampling: consider the smallest set of tokens whose
        probability sum is at least top_p. Must be in the closed interval [0.0, 1.0]."""
     random_seed: Optional[int] = None
     safe_mode: bool = False
     streaming: bool = False
 
+    class Config:
+        """Configuration for this pydantic object."""
+
+        allow_population_by_field_name = True
+        arbitrary_types_allowed = True
+
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling the API."""
         defaults = {
             "model": self.model,
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
@@ -246,14 +252,30 @@
                 return iter_sse()
             else:
                 return self.client.post(url="/chat/completions", json=kwargs).json()
 
         rtn = _completion_with_retry(**kwargs)
         return rtn
 
+    def _combine_llm_outputs(self, llm_outputs: List[Optional[dict]]) -> dict:
+        overall_token_usage: dict = {}
+        for output in llm_outputs:
+            if output is None:
+                # Happens in streaming
+                continue
+            token_usage = output["token_usage"]
+            if token_usage is not None:
+                for k, v in token_usage.items():
+                    if k in overall_token_usage:
+                        overall_token_usage[k] += v
+                    else:
+                        overall_token_usage[k] = v
+        combined = {"token_usage": overall_token_usage, "model_name": self.model}
+        return combined
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate api key, python package exists, temperature, and top_p."""
 
         values["mistral_api_key"] = convert_to_secret_str(
             get_from_dict_or_env(
                 values, "mistral_api_key", "MISTRAL_API_KEY", default=""
```

### Comparing `langchain_mistralai-0.1.0rc2/langchain_mistralai/embeddings.py` & `langchain_mistralai-0.1.1/langchain_mistralai/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,34 +25,36 @@
     To use, set the environment variable `MISTRAL_API_KEY` is set with your API key or
     pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
 
             from langchain_mistralai import MistralAIEmbeddings
+
             mistral = MistralAIEmbeddings(
                 model="mistral-embed",
-                mistral_api_key="my-api-key"
+                api_key="my-api-key"
             )
     """
 
     client: httpx.Client = Field(default=None)  #: :meta private:
     async_client: httpx.AsyncClient = Field(default=None)  #: :meta private:
-    mistral_api_key: Optional[SecretStr] = None
+    mistral_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     endpoint: str = "https://api.mistral.ai/v1/"
     max_retries: int = 5
     timeout: int = 120
     max_concurrent_requests: int = 64
     tokenizer: Tokenizer = Field(default=None)
 
     model: str = "mistral-embed"
 
     class Config:
         extra = Extra.forbid
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate configuration."""
 
         values["mistral_api_key"] = convert_to_secret_str(
             get_from_dict_or_env(
```

### Comparing `langchain_mistralai-0.1.0rc2/pyproject.toml` & `langchain_mistralai-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.0rc2"
+version = "0.1.1"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.31"
+langchain-core = "^0.1.41"
 tokenizers = "^0.15.1"
 httpx = ">=0.25.2,<1"
 httpx-sse = ">=0.3.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
+langchain-standard-tests = { path = "../../standard-tests", develop = true }
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 
 [tool.poetry.group.codespell]
```

### Comparing `langchain_mistralai-0.1.0rc2/PKG-INFO` & `langchain_mistralai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.0rc2
+Version: 0.1.1
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.25.2,<1)
 Requires-Dist: httpx-sse (>=0.3.1,<1)
-Requires-Dist: langchain-core (>=0.1.31,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.41,<0.2.0)
 Requires-Dist: tokenizers (>=0.15.1,<0.16.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/mistralai
 Description-Content-Type: text/markdown
 
 # langchain-mistralai
```

